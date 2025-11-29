# RLHF 101: A Technical Tutorial on Reinforcement Learning from Human Feedback

**来源**: [https://blog.ml.cmu.edu/2025/06/01/rlhf-101-a-technical-tutorial-on-reinforcement-learning-from-human-feedback/](https://blog.ml.cmu.edu/2025/06/01/rlhf-101-a-technical-tutorial-on-reinforcement-learning-from-human-feedback/)

---

# RLHF 101: A Technical Tutorial on Reinforcement Learning from Human Feedback – Machine Learning Blog | ML@CMU | Carnegie Mellon University

原文链接: https://blog.ml.cmu.edu/2025/06/01/rlhf-101-a-technical-tutorial-on-reinforcement-learning-from-human-feedback/

# Machine Learning Blog | ML@CMU | Carnegie Mellon University

[![Machine Learning Blog | ML@CMU | Carnegie Mellon University](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/5690b9fcb49699fd5559d0dbf8d73920.png)](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/ab50e657dfa4ee33230b62907bd18d7b.jpg)
[![Machine Learning Blog | ML@CMU | Carnegie Mellon University]()](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/ab50e657dfa4ee33230b62907bd18d7b.jpg)

#### Statistics:

123 publications.
14 categories.
72 tags.



* [[ Home ]](https://blog.ml.cmu.edu/# "Homepage")
* [[ Submissions ]](https://blog.ml.cmu.edu/submissions/ "Submissions")
* [[ About ]](https://blog.ml.cmu.edu/about/ "About us")

* [Home](https://blog.ml.cmu.edu/# "Homepage")
* [Submissions](https://blog.ml.cmu.edu/submissions/ "Our Team")
* [About](https://blog.ml.cmu.edu/about/ "Contact us")

* [Home](https://blog.ml.cmu.edu/# "Homepage")
* [Submissions](https://blog.ml.cmu.edu/submissions/ "Our Team")
* [About](https://blog.ml.cmu.edu/about/ "Contact us")

Input your search keywords and press Enter.



## Categories:

* [Research](https://blog.ml.cmu.edu/category/research)
* [Educational](https://blog.ml.cmu.edu/category/educational/)

[Educational](https://blog.ml.cmu.edu/category/educational/ "View all posts in Educational") [machine learning](https://blog.ml.cmu.edu/category/machine-learning/ "View all posts in machine learning")

# RLHF 101: A Technical Tutorial on Reinforcement Learning from Human Feedback

#### Authors

[Zhaolin Gao](https://blog.ml.cmu.edu/author/zg292/ "Posts by Zhaolin Gao") and [Gokul Swamy](https://blog.ml.cmu.edu/author/gswamy/ "Posts by Gokul Swamy")

#### Affiliations

#### Published

June 1, 2025

#### DOI

![](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/1841404dbbcc19c5537d835ba8c78cce.jpg)

Reinforcement Learning from Human Feedback (RLHF) is a popular technique used to align AI systems with human preferences by training them using feedback from people, rather than relying solely on predefined reward functions. Instead of coding every desirable behavior manually (which is often infeasible in complex tasks) RLHF allows models, especially large language models (LLMs), to learn from examples of what humans consider good or bad outputs. This approach is particularly important for tasks where success is subjective or hard to quantify, such as generating helpful and safe text responses. RLHF has become a cornerstone in building more aligned and controllable AI systems, making it essential for developing AI that behaves in ways humans intend.

This blog dives into the full training pipeline of the RLHF framework. We will explore every stage — from data generation and reward model inference, to the final training of an LLM. Our goal is to ensure that everything is fully reproducible by providing all the necessary code and the exact specifications of the environments used. By the end of this post, you should know the general pipeline to train any model with any instruction dataset using the RLHF algorithm of your choice!

## Preliminary: Setup & Environment

We will use the following setup for this tutorial:

* **Dataset:** [UltraFeedback](https://huggingface.co/datasets/allenai/ultrafeedback_binarized_cleaned_train), a well-curated dataset consisting of general chat prompts. (While UltraFeedback also contains LLM-generated responses to the prompts, we won’t be using these.)
* **Base Model:** [Llama-3-8B-it](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct), a state-of-the-art instruction-tuned LLM. This is the model we will fine-tune.
* **Reward Model:** [Armo](https://huggingface.co/RLHFlow/ArmoRM-Llama3-8B-v0.1), a robust reward model optimized for evaluating the generated outputs. We will use Armo to assign scalar reward values to candidate responses, indicating how “good” or “aligned” a response is.
* **Training Algorithm:** [REBEL](https://arxiv.org/pdf/2404.16767), a state-of-the-art algorithm tailored for efficient RLHF optimization.

To get started, clone our repo, which contains all the resources required for this tutorial:

```
git clone https://github.com/ZhaolinGao/REBEL
cd REBEL
```

We use two separate environments for different stages of the pipeline:

* `vllm`: Handles data generation, leveraging the efficient [vllm](https://github.com/vllm-project/vllm) library.
* `rebel`: Used for training the RLHF model.

You can install both environments using the provided YAML files:

```
conda env create -f ./envs/rebel_env.yml
conda env create -f ./envs/vllm_env.yml
```

## Part 1: Data Generation

The first step in the RLHF pipeline is generating samples from the policy to receive feedback on. Concretely, in this section, we will load the base model using `vllm` for fast inference, prepare the dataset, and generate multiple responses for each prompt in the dataset. The complete code for this part is available [here](https://github.com/ZhaolinGao/REBEL/blob/main/src/ultrafeedback_largebatch/generate.py).

Activate the `vllm` environment:

```
conda activate vllm
```

First, load the base model and tokenizer using `vllm`:

```
from transformers import AutoTokenizer
from vllm import LLM
tokenizer = AutoTokenizer.from_pretrained("meta-llama/Meta-Llama-3-8B-Instruct")
llm = LLM(
    model="meta-llama/Meta-Llama-3-8B-Instruct",
    tensor_parallel_size=8,
)
```

Here, `tensor_parallel_size` specifies the number of GPUs to use.

Next, load the UltraFeedback dataset:

```
from datasets import load_dataset
dataset = load_dataset("allenai/ultrafeedback_binarized_cleaned_train", split='train')
```

You can select a subset of the dataset using `dataset.select`. For example, to select the first 10,000 rows:

```
dataset = dataset.select(range(10000))
```

Alternatively, you can split the dataset into chunks using `dataset.shard` for implementations like [SPPO](https://arxiv.org/pdf/2405.00675) where each iteration only trains on one of the chunks.

Now, let’s prepare the dataset for generation. The Llama model uses special tokens to distinguish prompts and responses. For example:

```
<|begin_of_text|><|start_header_id|>user<|end_header_id|>

What is France's capital?<|eot_id|><|start_header_id|>assistant<|end_header_id|>
```

Therefore, for every prompt in the dataset, we need to convert it from plain text into this format before generating:

```
def get_message(instruction):
    message = [
        {"role": "user", "content": instruction},
    ]
    return message
prompts = [tokenizer.apply_chat_template(get_message(row['prompt']), tokenize=False, add_generation_prompt=True) for row in dataset]
```

* `get_message` transforms the plain-text prompt into a dictionary indicating it is from the user.
* `tokenizer.apply_chat_template` adds the required special tokens and appends the response tokens (<|start\_header\_id|>assistant<|end\_header\_id|>\n\n} at the end with `add_generation_prompt=True`.

Finally, we can generate the responses using `vllm` with the prompts we just formatted. We are going to generate 5 responses per prompt:

```
import torch
import random
import numpy as np
from vllm import SamplingParams

def set_seed(seed=5775709):
    random.seed(seed)
    np.random.seed(seed)
    torch.manual_seed(seed)
    torch.cuda.manual_seed_all(seed)

for p in range(5):
    set_seed(p * 50)
    sampling_params = SamplingParams(
        temperature=0.8,
        top_p=0.9,
        max_tokens=2048,
        seed=p * 50,
    )
    response = llm.generate(prompts, sampling_params)
    output = list(map(lambda x: x.outputs[0].text, response))
    dataset = dataset.add_column(f"response_{p}", output)
```

* `temperature=0.8, top_p=0.9` are common settings to control diversity in generation.
* `set_seed` is used to ensure reproducibility and sets a different seed for each response.
* `llm.generate` generates the response, and the results are added to the dataset with `dataset.add_column`.

You could run the complete scipt with:

```
python ./src/ultrafeedback_largebatch/generate.py --world_size NUM_GPU --output_repo OUTPUT_REPO
```

## Part 2: Reward Model Inference

The second step in the RLHF pipeline is querying the reward model to tell us how good a generated sample was. Concretely, in this part, we will calculate reward scores for the responses generated in Part 1 what are later used for training. The complete code for this part is available [here](https://github.com/ZhaolinGao/REBEL/blob/main/src/ultrafeedback_largebatch/rank.py).

Activate the `rebel` environment:

```
conda activate rebel
```

To begin, we’ll initialize the Armo reward model pipeline. This reward model is a fine-tuned sequence classification model that assigns a scalar reward score to a given dialogue based on its quality.

```
rm = ArmoRMPipeline("RLHFlow/ArmoRM-Llama3-8B-v0.1", trust_remote_code=True)
```

Now, we can gather the reward scores:

```
def get_message(instruction, response):
    return [{"role": "user", "content": instruction}, {"role": "assistant", "content": response}]

rewards = {}
for i in range(5):
    rewards[f"response_{i}_reward"] = []
    for row in dataset:
        reward = rm(get_message(row['prompt'], row[f'response_{i}']))
        rewards[f"response_{i}_reward"].append(reward)
for k, v in rewards.items():
    dataset = dataset.add_column(k, v)
```

* `get_message` formats the user prompt and assistant response into a list of dictionaries.
* `rm` computes a reward score for each response in the dataset.

You can run the complete scipt with:

```
python ./src/ultrafeedback_largebatch/rank.py --input_repo INPUT_REPO
```

* `INPUT_REPO` is the saved repo from Part 1 that contains the generated responses.

## Part 3: Filter and Tokenize

While the preceding two parts are all we need in theory to do RLHF, it is often advisable in practice to perform a filtering process to ensure training runs smoothly. Concretely, in this part, we’ll walk through the process of preparing a dataset for training by filtering excessively long prompts and responses to prevent out-of-memory (OOM) issues, selecting the best and worst responses for training, and removing duplicate responses. The complete code for this part is available [here](https://github.com/ZhaolinGao/REBEL/blob/main/src/ultrafeedback_largebatch/filter_tokenize.py).

Let’s first initialize two different tokenizers where one pads from the right and one pads from the left:

```
tokenizer = AutoTokenizer.from_pretrained("meta-llama/Meta-Llama-3-8B-Instruct")
tokenizer.add_special_tokens({"pad_token": "[PAD]"})
tokenizer_left = AutoTokenizer.from_pretrained("meta-llama/Meta-Llama-3-8B-Instruct", padding_side='left')
tokenizer_left.add_special_tokens({"pad_token": "[PAD]"})
```

These two different tokenizers allow us to pad the prompt from left and the response from the right such that they meet in the middle. By combining left-padded prompts with right-padded responses, we ensure that:

* Prompts and responses meet at a consistent position.
* Relative position embeddings remain correct for model training.

Here’s an example format:

```
[PAD] ... [PAD] <|begin_of_text|><|start_header_id|>user<|end_header_id|>

PROMPT<|eot_id|><|start_header_id|>assistant<|end_header_id|>


RESPONSE<|eot_id|>[PAD] ... [PAD]
```

We want to ensure that the length of

```
[PAD] ... [PAD] <|begin_of_text|><|start_header_id|>user<|end_header_id|>

PROMPT<|eot_id|><|start_header_id|>assistant<|end_header_id|>
```

is the same for all prompts, and the length of

```
RESPONSE<|eot_id|>[PAD] ... [PAD]
```

is the same for all responses.

We filter out prompts longer than 1,024 tokens and responses exceeding 2,048 tokens to prevent OOM during training:

```
dataset = dataset.filter(lambda row: tokenizer.apply_chat_template(get_message(row['prompt']), tokenize=True, add_generation_prompt=True, return_tensors='pt').shape[-1] <= 1024)
for i in range(5):
    dataset = dataset.filter(lambda row: tokenizer.apply_chat_template(get_message(response=row[f'response_{i}']), tokenize=True, add_generation_prompt=False, return_tensors='pt')[:, 5:].shape[-1] <= 2048)
```

Note that we skip the first five tokens of responses when counting lengths to exclude special tokens (e.g. <|begin\_of\_text|><|start\_header\_id|>assistant<|end\_header\_id|>\n\n) and only count the actual length of the response plus the EOS token (<|eot\_id|>) at the end.

Now we could tokenize the prompt with left padding to a maximum length of 1,024 tokens:

```
llama_prompt_tokens = []
for row in dataset:
    llama_prompt_token = tokenizer_left.apply_chat_template(
            get_message(row['prompt']), 
            add_generation_prompt=True,
            tokenize=True,
            padding='max_length',
            max_length=1024,
    )
    assert len(llama_prompt_token) == 1024
    assert (llama_prompt_token[0] == 128000 or llama_prompt_token[0] == 128256) and llama_prompt_token[-1] == 271
    llama_prompt_tokens.append(llama_prompt_token)
dataset = dataset.add_column("llama_prompt_tokens", llama_prompt_tokens)
```

The assertions are used to ensure that the length is always 1,024 and the tokenized prompt either starts with `[pad]` token or `<|begin_of_text|>` token and ends with `\n\n` token.

Then, we select the responses with the highest and lowest rewards for each prompt as the chosen and reject responses, and tokenize them with right padding:

```
chosen, reject, llama_chosen_tokens, llama_reject_tokens, chosen_reward, reject_reward = [], [], [], [], [], []

for row in dataset:

    all_rewards = [row[f"response_{i}_reward"] for i in range(5)]
    chosen_idx, reject_idx = np.argmax(all_rewards), np.argmin(all_rewards)

    chosen.append(row[f"response_{chosen_idx}"])
    reject.append(row[f"response_{reject_idx}"])

    llama_chosen_token = tokenizer.apply_chat_template(
            get_message(response=row[f"response_{chosen_idx}"]),
            add_generation_prompt=False,
            tokenize=True,
            padding='max_length',
            max_length=2048+5,
    )[5:]
    llama_chosen_tokens.append(llama_chosen_token)
    chosen_reward.append(row[f"response_{chosen_idx}_reward"])
    assert len(llama_chosen_token) == 2048
    assert llama_chosen_token[-1] == 128009 or llama_chosen_token[-1] == 128256

    llama_reject_token = tokenizer.apply_chat_template(
            get_message(response=row[f"response_{reject_idx}"]),
            add_generation_prompt=False,
            tokenize=True,
            padding='max_length',
            max_length=2048+5,
    )[5:]
    llama_reject_tokens.append(llama_reject_token)
    reject_reward.append(row[f"response_{reject_idx}_reward"])
    assert len(llama_reject_token) == 2048
    assert llama_reject_token[-1] == 128009 or llama_reject_token[-1] == 128256

dataset = dataset.add_column("chosen", chosen)
dataset = dataset.add_column("chosen_reward", chosen_reward)
dataset = dataset.add_column("llama_chosen_tokens", llama_chosen_tokens)
dataset = dataset.add_column("reject", reject)
dataset = dataset.add_column("reject_reward", reject_reward)
dataset = dataset.add_column("llama_reject_tokens", llama_reject_tokens)
```

Again the assertions are used to ensure that the lengths of the tokenized responses are always 2,048 and the tokenized responses either end with `[pad]` token or `<|eot_id|>` token.

Finally, we filter out rows where the chosen and reject responses are the same:

```
dataset = dataset.filter(lambda row: row['chosen'] != row['reject'])
```

and split the dataset into a training set and a test set with 1,000 prompts:

```
dataset = dataset.train_test_split(test_size=1000, shuffle=True)
```

You could run the complete scipt with:

```
python ./src/ultrafeedback_largebatch/filter_tokenize.py --input_repo INPUT_REPO
```

* `INPUT_REPO` is the saved repo from Part 2 that contains the rewards for each response.

## Part 4: Training with REBEL

Finally, we’re now ready to update the parameters of our model using an RLHF algorithm! We will now use our curated dataset and the REBEL algorithm to fine-tune our base model.

At each iteration \(t\) of REBEL, we aim to solve the following square loss regression problem:  
$$\theta\_{t+1}=\arg\min\_{\theta\in\Theta}\sum\_{(x, y, y’)\in \mathcal{D}\_t}\left(\frac{1}{\eta} \left(\ln \frac{\pi\_\theta(y|x)}{\pi\_{\theta\_t}(y|x)} – \ln \frac{\pi\_\theta(y’|x)}{\pi\_{\theta\_t}(y’|x)}\right) – \left(r(x, y) – r(x, y’)\right)\right)^2$$

where \(\eta\) is a hyperparameter, \(\theta\) is the parameter of the model, \(x\) is the prompt, \(\mathcal{D}\_t\) is the dataset we collected from the previous three parts, \(y\) and \(y’\) are the responses for \(x\), \(\pi\_\theta(y|x)\) is the probability of generation response \(y\) given prompt \(x\) under the parameterized policy \(\pi\_\theta\), and \(r(x, y)\) is the reward of response \(y\) for prompt \(x\) which is obtained from Part 2. The detailed derivations of the algorithm are shown in our [paper](https://arxiv.org/pdf/2404.16767). In short REBEL lets us avoid the complexity (e.g. clipping, critic models, …) of other RLHF algorithms like PPO while having stronger theoretical guarantees!

In this tutorial, we demonstrate a single iteration of REBEL (\(t=0\)) using the base model \(\pi\_{\theta\_0}\). For multi-iteration training, you can repeat Parts 1 through 4, initializing each iteration with the model trained in the previous iteration.

The complete code for this part is available [here](https://github.com/ZhaolinGao/REBEL/blob/main/src/ultrafeedback_largebatch/rebel.py). To enable full parameter training using 8 GPUs, we use the [Accelerate](https://huggingface.co/docs/accelerate/en/index) library with [Deepspeed](https://github.com/microsoft/DeepSpeed) Stage 3 by running:

```
accelerate launch --config_file accelerate_cfgs/deepspeed_config_stage_3.yaml --main-process-port 29080 --num_processes 8 src/ultrafeedback_largebatch/rebel.py --task.input_repo INPUT_REPO --output_dir OUTPUT_DIR
```

* `INPUT_REPO` is the saved repo from Part 3 that contains the tokenized prompts and responses.
* `OUTPUT_DIR` is the directory to save the models.

#### Step 1: Initialization & Loading

We start by initializing the batch size for distributed training:

```
args.world_size = accelerator.num_processes
args.batch_size = args.world_size * args.per_device_train_batch_size * args.gradient_accumulation_steps
args.local_batch_size = args.per_device_train_batch_size * args.gradient_accumulation_steps
args.rebel.num_updates = args.total_episodes // args.batch_size
```

* `args.world_size` is the number of GPUs we are using.
* `args.local_batch_size` is the batch size for each GPU.
* `args.batch_size` is the actual batch size for training.
* `args.rebel.num_updates` is the total number of updates to perform and `args.total_episodes` is the number of data points to train for. Typically, we set `args.total_episodes` to be the size of the training set for one epoch.

Next, we load the model and tokenizer, ensuring dropout layers are disabled such that the logprobs of the generations are computed without randomness:

```
tokenizer = AutoTokenizer.from_pretrained(
                args.base_model, 
                padding_side='right',
                trust_remote_code=True,
            )
tokenizer.add_special_tokens({"pad_token": "[PAD]"})
policy = AutoModelForCausalLM.from_pretrained(
            args.base_model,
            trust_remote_code=True,
            torch_dtype=torch.bfloat16,
            attn_implementation="flash_attention_2",
        )
disable_dropout_in_model(policy)
```

#### Step 2: Training

Looking again at the REBEL objective, the only things we need now to train is to compute \(\pi\_\theta(y|x)\) and \(\pi\_{\theta\_0}(y|x)\). We can compute each of them with:

```
output = policy(
    input_ids=input_ids, 
    attention_mask=attention_mask,
    return_dict=True,
    output_hidden_states=True,
)
logits = output.logits[:, args.task.maxlen_prompt - 1 : -1]
logits /= args.task.temperature + 1e-7
all_logprobs = F.log_softmax(logits, dim=-1)
logprobs = torch.gather(all_logprobs, 2, input_ids[:, args.task.maxlen_prompt:].unsqueeze(-1)).squeeze(-1)
logprobs = (logprobs * seq_mask).sum(-1)
```

* `output.logits` contains the logits of all tokens in the vocabulary for the sequence of `input_ids`.
* `output.logits[:, args.task.maxlen_prompt - 1 : -1]` is the logits of all tokens in the vocabulary for the sequence of response only. It is shifted by 1 since the logits at position \(p\) are referring to the logits at position \(p+1\).
* We divide `logits` by `args.task.temperature` to obtain the actual probability during generation.
* `torch.gather` is used to gather the perspective token in the response.
* `mb_seq_mask` masks out the paddings.

#### Step 4: Loss Computation

Finally, we could compute the loss by:

```
reg_diff = ((pi_logprobs_y - pi_0_logprobs_y) - (pi_logprobs_y_prime - pi_0_logprobs_y_prime)) / eta - (chosen_reward - reject_reward)
loss = (reg_diff ** 2).mean()
```

## Performance

With only one iteration of the above 4 parts, we can greatly enhance the performance of the base model on AlpacaEval, MT-Bench, and ArenaHard, three benchmarks commonly used to evaluate the quality, alignment, and helpfulness of responses generated by LLMs.

| Model | AlpacaEval 2.0 LC Win Rate | AlpacaEval 2.0 Win Rate | MT-Bench Average | ArenaHard |
| --- | --- | --- | --- | --- |
| [Llama-3-8B-it](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct) | 22.9 | 22.6 | 8.10 | 22.3 |
| [REBEL-Llama-3-Armo-iter\_1](https://huggingface.co/Cornell-AGI/REBEL-Llama-3-Armo-iter_1) | 48.3 | 41.8 | 8.13 | 34.5 |

## Takeaway

In this post, we outlined the pipeline for implementing RLHF, covering the entire process from data generation to the actual training phase. While we focused specifically on the REBEL algorithm, this pipeline is versatile and can be readily adapted to other methods such as [DPO](https://arxiv.org/pdf/2305.18290) or [SimPO](https://arxiv.org/pdf/2405.14734). The necessary components for these methods are already included except for the specific loss formulation. There’s also a natural extension of the above pipeline to *multi-turn* RLHF where we optimize for performance over an entire conversation (rather than a single generation) — check out our follow-up paper [here](https://arxiv.org/pdf/2410.04612) for more information!

If you find this implementation useful, please consider citing our work:

```
@misc{gao2024rebel,
      title={REBEL: Reinforcement Learning via Regressing Relative Rewards}, 
      author={Zhaolin Gao and Jonathan D. Chang and Wenhao Zhan and Owen Oertell and Gokul Swamy and Kianté Brantley and Thorsten Joachims and J. Andrew Bagnell and Jason D. Lee and Wen Sun},
      year={2024},
      eprint={2404.16767},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}
```

* [♥719](https://blog.ml.cmu.edu/wp-admin/admin-ajax.php?action=process_simple_like&post_id=20919&nonce=fc8e41b9c0&is_comment=0&disabled=true "Like")
   32856
* [Read More](https://blog.ml.cmu.edu/2025/06/01/rlhf-101-a-technical-tutorial-on-reinforcement-learning-from-human-feedback/)

* ![](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/6a475d6263e6f97730dfd28b6ddcfde9.png) [Unlearning or Obfuscating? Jogging the Memory of Unlearned LLMs via Benign Relearning](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/7b8181462b586a8dd69120e2e1ac3559.jpg)
* ![](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/3487518ab205b33aa7aec503f3ad28f7.jpg) [Carnegie Mellon University at ICML 2025](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/59492fc397bbdf54481505c50b181b30.jpg)

#### You Might Also Like

[![](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/2369beccefc67cbe209e710c7c28ef5c.png)](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/714a43aa2f34e764ab44b4d71e6caec8.jpg)

###### [Inductive biases of neural network modularity in spatial navigation](https://blog.ml.cmu.edu/2025/01/02/inductive-biases-of-neural-network-modularity-in-spatial-navigation/)

January 2, 2025

[![](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/90796c538ad2c677cf53a4f41de60b02.jpg)](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/165d2c69787650c811fb98e8cd791404.jpg)

###### [Carnegie Mellon University at ICML 2020](https://blog.ml.cmu.edu/2020/07/13/carnegie-mellon-university-at-icml-2020/)

July 13, 2020

[![flat landscape](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/e3567d7f8f387511304bc8a98339613d.png)](ai-leaders-insights/安全治理与未来/对齐问题/RLHF技术/images/5dc6eba1d219fde9143ea44e8b43f02b.jpg)

###### [Analyzing and Improving the Optimization Landscape of Noise-Contrastive Estimation](https://blog.ml.cmu.edu/2021/11/05/analyzing-and-improving-the-optimization-landscape-of-noise-contrastive-estimation/)

November 5, 2021

#### No Comments

### Leave a Reply [Cancel Reply](/2025/06/01/rlhf-101-a-technical-tutorial-on-reinforcement-learning-from-human-feedback/#respond)

Name \*

Email \*

Website

Save my name, email, and website in this browser for the next time I comment.

---

[instagram-feed num=6 cols=6 imagepadding=0 disablemobile=true showbutton=false showheader=false followtext=”Follow @Mint\_Theme”]

---

*爬取时间: 2025-11-28 21:57:46*
