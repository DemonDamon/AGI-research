# Are aligned neural networks adversarially aligned?

**来源**: [https://proceedings.neurips.cc/paper_files/paper/2023/hash/c1f0b856a35986348ab3414177266f75-Abstract-Conference.html](https://proceedings.neurips.cc/paper_files/paper/2023/hash/c1f0b856a35986348ab3414177266f75-Abstract-Conference.html)

---

# Are aligned neural networks adversarially aligned?

原文链接: https://proceedings.neurips.cc/paper_files/paper/2023/hash/c1f0b856a35986348ab3414177266f75-Abstract-Conference.html

#### Are aligned neural networks adversarially aligned?

Part of
[Advances in Neural Information Processing Systems 36 (NeurIPS 2023)](/paper_files/paper/2023)
Main Conference Track

[Bibtex](/paper_files/paper/22761-/bibtex) [Paper](/paper_files/paper/2023/file/c1f0b856a35986348ab3414177266f75-Paper-Conference.pdf) [Supplemental](/paper_files/paper/2023/file/c1f0b856a35986348ab3414177266f75-Supplemental-Conference.pdf)

  

#### Authors

*Nicholas Carlini, Milad Nasr, Christopher A. Choquette-Choo, Matthew Jagielski, Irena Gao, Pang Wei W Koh, Daphne Ippolito, Florian Tramer, Ludwig Schmidt*

#### Abstract

Large language models are now tuned to align with the goals of their creators, namely to be "helpful and harmless." These models should respond helpfully to user questions, but refuse to answer requests that could cause harm. However, adversarial users can construct inputs which circumvent attempts at alignment. In this work, we study adversarial alignment, and ask to what extent these models remain aligned when interacting with an adversarial user who constructs worst-case inputs (adversarial examples). These inputs are designed to cause the model to emit harmful content that would otherwise be prohibited.We show that existing NLP-based optimization attacks are insufficiently powerful to reliably attack aligned text models: even when current NLP-based attacks fail, we can find adversarial inputs with brute force. As a result, the failure of current attacks should not be seen as proof that aligned text models remain aligned under adversarial inputs. However the recent trend in large-scale ML models is multimodal models that allow users to provide images that influence the text that is generated. We show these models can be easily attacked, i.e., induced to perform arbitrary un-aligned behavior through adversarial perturbation of the input image. We conjecture that improved NLP attacks may demonstrate this same level of adversarial control over text-only models.

  

#### Name Change Policy

×

Requests for name changes in the electronic proceedings will be accepted with no questions asked. However name changes may cause bibliographic tracking issues. Authors are asked to consider this carefully and discuss it with their co-authors prior to requesting a name change in the electronic proceedings.

Use the "Report an Issue" link to request a name change.

Do not remove: This comment is monitored to verify that the site is working properly

---

*爬取时间: 2025-11-28 21:56:28*
