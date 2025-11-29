# A systematic evaluation of large language models of code

**来源**: [https://dl.acm.org/doi/abs/10.1145/3520312.3534862](https://dl.acm.org/doi/abs/10.1145/3520312.3534862)

---

# A systematic evaluation of large language models of code | Proceedings of the 6th ACM SIGPLAN International Symposium on Machine Programming

原文链接: https://dl.acm.org/doi/abs/10.1145/3520312.3534862

research-article

Open access

Share on

# A systematic evaluation of large language models of code

Authors: [![](/pb-assets/icons/DOs/default-profile-1543932446943.svg)Frank F. Xu](# "Frank F. Xu")

![](/pb-assets/icons/DOs/default-profile-1543932446943.svg)

Frank F. Xu

Carnegie Mellon University, USA

[View Profile](/profile/99659242096)

, [![](/pb-assets/icons/DOs/default-profile-1543932446943.svg)Uri Alon](# "Uri Alon")

![](/pb-assets/icons/DOs/default-profile-1543932446943.svg)

Uri Alon

Carnegie Mellon University, USA

[View Profile](/profile/81100302881)

, [![](/pb-assets/icons/DOs/default-profile-1543932446943.svg)Graham Neubig](# "Graham Neubig")

![](/pb-assets/icons/DOs/default-profile-1543932446943.svg)

Graham Neubig

Carnegie Mellon University, USA

[View Profile](/profile/81486654903)

, [![](/pb-assets/icons/DOs/default-profile-1543932446943.svg)Vincent Josua Hellendoorn](# "Vincent Josua Hellendoorn")

![](/pb-assets/icons/DOs/default-profile-1543932446943.svg)

Vincent Josua Hellendoorn

Carnegie Mellon University, USA

[View Profile](/profile/99658746287)

[Authors Info & Claims](#tab-contributors)

[MAPS 2022: Proceedings of the 6th ACM SIGPLAN International Symposium on Machine Programming](/doi/proceedings/10.1145/3520312)

Pages 1 - 10

<https://doi.org/10.1145/3520312.3534862>

Published: 13 June 2022 [Publication History](#core-history)

333citation16,458Downloads

Metrics

[Total Citations333](#tab-citations "See Citations pane")[Total Downloads16,458](#tab-metrics-inner "See Bibliometrics pane")

Last 12 Months4,141

Last 6 weeks278

Get Citation Alerts

[PDF](https://dl.acm.org/doi/pdf/10.1145/3520312.3534862 "View PDF")[eReader](/doi/epdf/10.1145/3520312.3534862 "View online with eReader")

Contents

## Abstract

Large language models (LMs) of code have recently shown tremendous promise in completing code and synthesizing code from natural language descriptions. However, the current state-of-the-art code LMs (e.g., Codex) are not publicly available, leaving many questions about their model and data design decisions. We aim to fill in some of these blanks through a systematic evaluation of the largest existing models: Codex, GPT-J, GPT-Neo, GPT-NeoX-20B, and CodeParrot, across various programming languages. Although Codex itself is not open-source, we find that existing opensource models do achieve close results in some programming languages, although targeted mainly for natural language modeling. We further identify an important missing piece in the form of a large open-source model trained exclusively on a multi-lingual corpus of code. We release a new model, PolyCoder, with 2.7B parameters based on the GPT-2 architecture, that was trained on 249GB of code across 12 programming languages on a single machine. In the C programming language, PolyCoder outperforms all models including Codex. Our trained models are open-source and publicly available at https://github.com/VHellendoorn/Code-LMs, which enables future research and application in this area. We have an online appendix at https://arxiv.org/abs/2202.13169.

## Formats available

You can view the full content in the following formats:

[PDF](https://dl.acm.org/doi/pdf/10.1145/3520312.3534862 "View PDF")

## References

[1]

Wasi Ahmad, Saikat Chakraborty, Baishakhi Ray, and Kai-Wei Chang. 2021. Unified Pre-training for Program Understanding and Generation. In Proceedings of the 2021 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies. Association for Computational Linguistics, Online. 2655–2668. https://www.aclweb.org/anthology/2021.naacl-main.211

[Crossref](https://doi.org/10.18653/v1/2021.naacl-main.211)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.18653%2Fv1%2F2021.naacl-main.211)

[2]

Miltiadis Allamanis. 2019. The adverse effects of code duplication in machine learning models of code. In Proceedings of the 2019 ACM SIGPLAN International Symposium on New Ideas, New Paradigms, and Reflections on Programming and Software. 143–153.

[Digital Library](/doi/10.1145/3359591.3359735)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F3359591.3359735)

[3]

Uri Alon, Roy Sadaka, Omer Levy, and Eran Yahav. 2020. Structural language models of code. In International Conference on Machine Learning. 245–256.

[Google Scholar](https://scholar.google.com/scholar?q=Uri+Alon%2C+Roy+Sadaka%2C+Omer+Levy%2C+and+Eran+Yahav.+2020.+Structural+language+models+of+code.+In+International+Conference+on+Machine+Learning.+245%E2%80%93256.)

[4]

Jacob Austin, Augustus Odena, Maxwell Nye, Maarten Bosma, Henryk Michalewski, David Dohan, Ellen Jiang, Carrie Cai, Michael Terry, and Quoc Le. 2021. Program synthesis with large language models. arXiv preprint arXiv:2108.07732.

[Google Scholar](https://scholar.google.com/scholar?q=Jacob+Austin%2C+Augustus+Odena%2C+Maxwell+Nye%2C+Maarten+Bosma%2C+Henryk+Michalewski%2C+David+Dohan%2C+Ellen+Jiang%2C+Carrie+Cai%2C+Michael+Terry%2C+and+Quoc+Le.+2021.+Program+synthesis+with+large+language+models.+arXiv+preprint+arXiv%3A2108.07732.)

[5]

Alexei Baevski and Michael Auli. 2018. Adaptive input representations for neural language modeling. arXiv preprint arXiv:1809.10853.

[Google Scholar](https://scholar.google.com/scholar?q=Alexei+Baevski+and+Michael+Auli.+2018.+Adaptive+input+representations+for+neural+language+modeling.+arXiv+preprint+arXiv%3A1809.10853.)

[6]

Yoshua Bengio, Réjean Ducharme, Pascal Vincent, and Christian Jauvin. 2003. A neural probabilistic language model. Journal of machine learning research, 3, Feb (2003), 1137–1155.

[Google Scholar](https://scholar.google.com/scholar?q=Yoshua+Bengio%2C+R%C3%A9jean+Ducharme%2C+Pascal+Vincent%2C+and+Christian+Jauvin.+2003.+A+neural+probabilistic+language+model.+Journal+of+machine+learning+research%2C+3%2C+Feb+%282003%29%2C+1137%E2%80%931155.)

[7]

Sid Black, Stella Biderman, Eric Hallahan, Quentin Anthony, Leo Gao, Laurence Golding, Horace He, Connor Leahy, Kyle McDonell, Jason Phang, Michael Pieler, USVSN Sai Prashanth, Shivanshu Purohit, Laria Reynolds, Jonathan Tow, Ben Wang, and Samuel Weinbach. 2022. GPT-NeoX-20B: An Open-Source Autoregressive Language Model.

[Google Scholar](https://scholar.google.com/scholar?q=Sid+Black%2C+Stella+Biderman%2C+Eric+Hallahan%2C+Quentin+Anthony%2C+Leo+Gao%2C+Laurence+Golding%2C+Horace+He%2C+Connor+Leahy%2C+Kyle+McDonell%2C+Jason+Phang%2C+Michael+Pieler%2C+USVSN+Sai+Prashanth%2C+Shivanshu+Purohit%2C+Laria+Reynolds%2C+Jonathan+Tow%2C+Ben+Wang%2C+and+Samuel+Weinbach.+2022.+GPT-NeoX-20B%3A+An+Open-Source+Autoregressive+Language+Model.)

[8]

Sid Black, Leo Gao, Phil Wang, Connor Leahy, and Stella Biderman. 2021. GPT-Neo: Large Scale Autoregressive Language Modeling with Mesh-Tensorflow. https://doi.org/10.5281/zenodo.5297715 If you use this software, please cite it using these metadata.

[Crossref](https://doi.org/10.5281/zenodo.5297715)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.5281%2Fzenodo.5297715)

[9]

Tom B Brown, Benjamin Mann, Nick Ryder, Melanie Subbiah, Jared Kaplan, Prafulla Dhariwal, Arvind Neelakantan, Pranav Shyam, Girish Sastry, and Amanda Askell. 2020. Language models are few-shot learners. arXiv preprint arXiv:2005.14165.

[Google Scholar](https://scholar.google.com/scholar?q=Tom+B+Brown%2C+Benjamin+Mann%2C+Nick+Ryder%2C+Melanie+Subbiah%2C+Jared+Kaplan%2C+Prafulla+Dhariwal%2C+Arvind+Neelakantan%2C+Pranav+Shyam%2C+Girish+Sastry%2C+and+Amanda+Askell.+2020.+Language+models+are+few-shot+learners.+arXiv+preprint+arXiv%3A2005.14165.)

[10]

Mark Chen, Jerry Tworek, Heewoo Jun, Qiming Yuan, Henrique Ponde, Jared Kaplan, Harri Edwards, Yura Burda, Nicholas Joseph, and Greg Brockman. 2021. Evaluating large language models trained on code. arXiv preprint arXiv:2107.03374.

[Google Scholar](https://scholar.google.com/scholar?q=Mark+Chen%2C+Jerry+Tworek%2C+Heewoo+Jun%2C+Qiming+Yuan%2C+Henrique+Ponde%2C+Jared+Kaplan%2C+Harri+Edwards%2C+Yura+Burda%2C+Nicholas+Joseph%2C+and+Greg+Brockman.+2021.+Evaluating+large+language+models+trained+on+code.+arXiv+preprint+arXiv%3A2107.03374.)

[11]

Alexis Conneau and Guillaume Lample. 2019. Cross-lingual language model pretraining. Advances in Neural Information Processing Systems, 32 (2019), 7059–7069.

[Google Scholar](https://scholar.google.com/scholar?q=Alexis+Conneau+and+Guillaume+Lample.+2019.+Cross-lingual+language+model+pretraining.+Advances+in+Neural+Information+Processing+Systems%2C+32+%282019%29%2C+7059%E2%80%937069.)

[12]

Aditya Desai, Sumit Gulwani, Vineet Hingorani, Nidhi Jain, Amey Karkare, Mark Marron, and Subhajit Roy. 2016. Program synthesis using natural language. In Proceedings of the 38th International Conference on Software Engineering. 345–356.

[Digital Library](/doi/10.1145/2884781.2884786)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F2884781.2884786)

[13]

Jacob Devlin, Ming-Wei Chang, Kenton Lee, and Kristina Toutanova. 2018. BERT: Pre-training of deep bidirectional transformers for language understanding. arXiv preprint arXiv:1810.04805.

[Google Scholar](https://scholar.google.com/scholar?q=Jacob+Devlin%2C+Ming-Wei+Chang%2C+Kenton+Lee%2C+and+Kristina+Toutanova.+2018.+BERT%3A+Pre-training+of+deep+bidirectional+transformers+for+language+understanding.+arXiv+preprint+arXiv%3A1810.04805.)

[14]

Zhangyin Feng, Daya Guo, Duyu Tang, Nan Duan, Xiaocheng Feng, Ming Gong, Linjun Shou, Bing Qin, Ting Liu, and Daxin Jiang. 2020. Codebert: A pre-trained model for programming and natural languages. arXiv preprint arXiv:2002.08155.

[Google Scholar](https://scholar.google.com/scholar?q=Zhangyin+Feng%2C+Daya+Guo%2C+Duyu+Tang%2C+Nan+Duan%2C+Xiaocheng+Feng%2C+Ming+Gong%2C+Linjun+Shou%2C+Bing+Qin%2C+Ting+Liu%2C+and+Daxin+Jiang.+2020.+Codebert%3A+A+pre-trained+model+for+programming+and+natural+languages.+arXiv+preprint+arXiv%3A2002.08155.)

[15]

Leo Gao, Stella Biderman, Sid Black, Laurence Golding, Travis Hoppe, Charles Foster, Jason Phang, Horace He, Anish Thite, and Noa Nabeshima. 2020. The pile: An 800gb dataset of diverse text for language modeling. arXiv preprint arXiv:2101.00027.

[Google Scholar](https://scholar.google.com/scholar?q=Leo+Gao%2C+Stella+Biderman%2C+Sid+Black%2C+Laurence+Golding%2C+Travis+Hoppe%2C+Charles+Foster%2C+Jason+Phang%2C+Horace+He%2C+Anish+Thite%2C+and+Noa+Nabeshima.+2020.+The+pile%3A+An+800gb+dataset+of+diverse+text+for+language+modeling.+arXiv+preprint+arXiv%3A2101.00027.)

[16]

Xu Han, Zhengyan Zhang, Ning Ding, Yuxian Gu, Xiao Liu, Yuqi Huo, Jiezhong Qiu, Liang Zhang, Wentao Han, and Minlie Huang. 2021. Pre-trained models: Past, present and future. AI Open.

[Google Scholar](https://scholar.google.com/scholar?q=Xu+Han%2C+Zhengyan+Zhang%2C+Ning+Ding%2C+Yuxian+Gu%2C+Xiao+Liu%2C+Yuqi+Huo%2C+Jiezhong+Qiu%2C+Liang+Zhang%2C+Wentao+Han%2C+and+Minlie+Huang.+2021.+Pre-trained+models%3A+Past%2C+present+and+future.+AI+Open.)

[17]

Vincent J Hellendoorn and Premkumar Devanbu. 2017. Are deep neural networks the best choice for modeling source code? In Proceedings of the 2017 11th Joint Meeting on Foundations of Software Engineering. 763–773.

[Digital Library](/doi/10.1145/3106237.3106290)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F3106237.3106290)

[18]

Vincent J. Hellendoorn and Anand Ashok Sawant. 2021. The Growing Cost of Deep Learning for Source Code. Commun. ACM, 65, 1 (2021), dec, 31–33. issn:0001-0782 https://doi.org/10.1145/3501261

[Digital Library](/doi/10.1145/3501261)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F3501261)

[19]

Abram Hindle, Earl T Barr, Mark Gabel, Zhendong Su, and Premkumar Devanbu. 2016. On the naturalness of software. Commun. ACM, 59, 5 (2016), 122–131.

[Digital Library](/doi/10.1145/2902362)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F2902362)

[20]

Ari Holtzman, Jan Buys, Li Du, Maxwell Forbes, and Yejin Choi. 2019. The curious case of neural text degeneration. arXiv preprint arXiv:1904.09751.

[Google Scholar](https://scholar.google.com/scholar?q=Ari+Holtzman%2C+Jan+Buys%2C+Li+Du%2C+Maxwell+Forbes%2C+and+Yejin+Choi.+2019.+The+curious+case+of+neural+text+degeneration.+arXiv+preprint+arXiv%3A1904.09751.)

[21]

Hamel Husain, Ho-Hsiang Wu, Tiferet Gazit, Miltiadis Allamanis, and Marc Brockschmidt. 2019. Codesearchnet challenge: Evaluating the state of semantic code search. arXiv preprint arXiv:1909.09436.

[Google Scholar](https://scholar.google.com/scholar?q=Hamel+Husain%2C+Ho-Hsiang+Wu%2C+Tiferet+Gazit%2C+Miltiadis+Allamanis%2C+and+Marc+Brockschmidt.+2019.+Codesearchnet+challenge%3A+Evaluating+the+state+of+semantic+code+search.+arXiv+preprint+arXiv%3A1909.09436.)

[22]

Aditya Kanade, Petros Maniatis, Gogul Balakrishnan, and Kensen Shi. 2020. Learning and evaluating contextual embedding of source code. In International Conference on Machine Learning. 5110–5121.

[Google Scholar](https://scholar.google.com/scholar?q=Aditya+Kanade%2C+Petros+Maniatis%2C+Gogul+Balakrishnan%2C+and+Kensen+Shi.+2020.+Learning+and+evaluating+contextual+embedding+of+source+code.+In+International+Conference+on+Machine+Learning.+5110%E2%80%935121.)

[23]

Rafael-Michael Karampatsis, Hlib Babii, Romain Robbes, Charles Sutton, and Andrea Janes. 2020. Big code!= big vocabulary: Open-vocabulary models for source code. In 2020 IEEE/ACM 42nd International Conference on Software Engineering (ICSE). 1073–1085.

[Digital Library](/doi/10.1145/3377811.3380342)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F3377811.3380342)

[24]

Mike Lewis, Yinhan Liu, Naman Goyal, Marjan Ghazvininejad, Abdelrahman Mohamed, Omer Levy, Ves Stoyanov, and Luke Zettlemoyer. 2019. Bart: Denoising sequence-to-sequence pre-training for natural language generation, translation, and comprehension. arXiv preprint arXiv:1910.13461.

[Google Scholar](https://scholar.google.com/scholar?q=Mike+Lewis%2C+Yinhan+Liu%2C+Naman+Goyal%2C+Marjan+Ghazvininejad%2C+Abdelrahman+Mohamed%2C+Omer+Levy%2C+Ves+Stoyanov%2C+and+Luke+Zettlemoyer.+2019.+Bart%3A+Denoising+sequence-to-sequence+pre-training+for+natural+language+generation%2C+translation%2C+and+comprehension.+arXiv+preprint+arXiv%3A1910.13461.)

[25]

Shuai Lu, Daya Guo, Shuo Ren, Junjie Huang, Alexey Svyatkovskiy, Ambrosio Blanco, Colin Clement, Dawn Drain, Daxin Jiang, Duyu Tang, Ge Li, Lidong Zhou, Linjun Shou, Long Zhou, Michele Tufano, MING GONG, Ming Zhou, Nan Duan, Neel Sundaresan, Shao Kun Deng, Shengyu Fu, and Shujie LIU. 2021. CodeXGLUE: A Machine Learning Benchmark Dataset for Code Understanding and Generation. In Thirty-fifth Conference on Neural Information Processing Systems Datasets and Benchmarks Track (Round 1). https://openreview.net/forum?id=6lE4dQXaUcb

[Google Scholar](https://scholar.google.com/scholar?q=Shuai+Lu%2C+Daya+Guo%2C+Shuo+Ren%2C+Junjie+Huang%2C+Alexey+Svyatkovskiy%2C+Ambrosio+Blanco%2C+Colin+Clement%2C+Dawn+Drain%2C+Daxin+Jiang%2C+Duyu+Tang%2C+Ge+Li%2C+Lidong+Zhou%2C+Linjun+Shou%2C+Long+Zhou%2C+Michele+Tufano%2C+MING+GONG%2C+Ming+Zhou%2C+Nan+Duan%2C+Neel+Sundaresan%2C+Shao+Kun+Deng%2C+Shengyu+Fu%2C+and+Shujie+LIU.+2021.+CodeXGLUE%3A+A+Machine+Learning+Benchmark+Dataset+for+Code+Understanding+and+Generation.+In+Thirty-fifth+Conference+on+Neural+Information+Processing+Systems+Datasets+and+Benchmarks+Track+%28Round+1%29.+https%3A%2F%2Fopenreview.net%2Fforum%3Fid%3D6lE4dQXaUcb)

[26]

Hammond Pearce, Baleegh Ahmad, Benjamin Tan, Brendan Dolan-Gavitt, and Ramesh Karri. 2021. An Empirical Cybersecurity Evaluation of GitHub Copilot’s Code Contributions. arXiv preprint arXiv:2108.09293.

[Google Scholar](https://scholar.google.com/scholar?q=Hammond+Pearce%2C+Baleegh+Ahmad%2C+Benjamin+Tan%2C+Brendan+Dolan-Gavitt%2C+and+Ramesh+Karri.+2021.+An+Empirical+Cybersecurity+Evaluation+of+GitHub+Copilot%E2%80%99s+Code+Contributions.+arXiv+preprint+arXiv%3A2108.09293.)

[27]

Alec Radford, Jeffrey Wu, Rewon Child, David Luan, Dario Amodei, and Ilya Sutskever. 2019. Language models are unsupervised multitask learners. OpenAI blog, 1, 8 (2019), 9.

[Google Scholar](https://scholar.google.com/scholar?q=Alec+Radford%2C+Jeffrey+Wu%2C+Rewon+Child%2C+David+Luan%2C+Dario+Amodei%2C+and+Ilya+Sutskever.+2019.+Language+models+are+unsupervised+multitask+learners.+OpenAI+blog%2C+1%2C+8+%282019%29%2C+9.)

[28]

Colin Raffel, Noam Shazeer, Adam Roberts, Katherine Lee, Sharan Narang, Michael Matena, Yanqi Zhou, Wei Li, and Peter J Liu. 2019. Exploring the limits of transfer learning with a unified text-to-text transformer. arXiv preprint arXiv:1910.10683.

[Google Scholar](https://scholar.google.com/scholar?q=Colin+Raffel%2C+Noam+Shazeer%2C+Adam+Roberts%2C+Katherine+Lee%2C+Sharan+Narang%2C+Michael+Matena%2C+Yanqi+Zhou%2C+Wei+Li%2C+and+Peter+J+Liu.+2019.+Exploring+the+limits+of+transfer+learning+with+a+unified+text-to-text+transformer.+arXiv+preprint+arXiv%3A1910.10683.)

[29]

Veselin Raychev, Martin Vechev, and Eran Yahav. 2014. Code completion with statistical language models. In Proceedings of the 35th ACM SIGPLAN Conference on Programming Language Design and Implementation. 419–428.

[Digital Library](/doi/10.1145/2594291.2594321)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F2594291.2594321)

[30]

Rico Sennrich, Barry Haddow, and Alexandra Birch. 2015. Neural machine translation of rare words with subword units. arXiv preprint arXiv:1508.07909.

[Google Scholar](https://scholar.google.com/scholar?q=Rico+Sennrich%2C+Barry+Haddow%2C+and+Alexandra+Birch.+2015.+Neural+machine+translation+of+rare+words+with+subword+units.+arXiv+preprint+arXiv%3A1508.07909.)

[31]

Emma Strubell, Ananya Ganesh, and Andrew McCallum. 2019. Energy and policy considerations for deep learning in NLP. arXiv preprint arXiv:1906.02243.

[Google Scholar](https://scholar.google.com/scholar?q=Emma+Strubell%2C+Ananya+Ganesh%2C+and+Andrew+McCallum.+2019.+Energy+and+policy+considerations+for+deep+learning+in+NLP.+arXiv+preprint+arXiv%3A1906.02243.)

[32]

Lewis Tunstall, Leandro von Werra, and Thomas Wolf. 2022. Natural Language Processing with Transformers. " O’Reilly Media, Inc.".

[Google Scholar](https://scholar.google.com/scholar?q=Lewis+Tunstall%2C+Leandro+von+Werra%2C+and+Thomas+Wolf.+2022.+Natural+Language+Processing+with+Transformers.+%22+O%E2%80%99Reilly+Media%2C+Inc.%22.)

[33]

Morteza Verdi, Ashkan Sami, Jafar Akhondali, Foutse Khomh, Gias Uddin, and Alireza Karami Motlagh. 2020. An empirical study of c++ vulnerabilities in crowd-sourced code examples. IEEE Transactions on Software Engineering.

[Google Scholar](https://scholar.google.com/scholar?q=Morteza+Verdi%2C+Ashkan+Sami%2C+Jafar+Akhondali%2C+Foutse+Khomh%2C+Gias+Uddin%2C+and+Alireza+Karami+Motlagh.+2020.+An+empirical+study+of+c%2B%2B+vulnerabilities+in+crowd-sourced+code+examples.+IEEE+Transactions+on+Software+Engineering.)

[34]

Eric Wallace, Tony Z Zhao, Shi Feng, and Sameer Singh. 2020. Concealed data poisoning attacks on NLP models. arXiv preprint arXiv:2010.12563.

[Google Scholar](https://scholar.google.com/scholar?q=Eric+Wallace%2C+Tony+Z+Zhao%2C+Shi+Feng%2C+and+Sameer+Singh.+2020.+Concealed+data+poisoning+attacks+on+NLP+models.+arXiv+preprint+arXiv%3A2010.12563.)

[35]

Ben Wang and Aran Komatsuzaki. 2021. GPT-J-6B: A 6 Billion Parameter Autoregressive Language Model. https://github.com/kingoflolz/mesh-transformer-jax

[Google Scholar](https://scholar.google.com/scholar?q=Ben+Wang+and+Aran+Komatsuzaki.+2021.+GPT-J-6B%3A+A+6+Billion+Parameter+Autoregressive+Language+Model.+https%3A%2F%2Fgithub.com%2Fkingoflolz%2Fmesh-transformer-jax)

[36]

Yue Wang, Weishi Wang, Shafiq Joty, and Steven CH Hoi. 2021. Codet5: Identifier-aware unified pre-trained encoder-decoder models for code understanding and generation. arXiv preprint arXiv:2109.00859.

[Google Scholar](https://scholar.google.com/scholar?q=Yue+Wang%2C+Weishi+Wang%2C+Shafiq+Joty%2C+and+Steven+CH+Hoi.+2021.+Codet5%3A+Identifier-aware+unified+pre-trained+encoder-decoder+models+for+code+understanding+and+generation.+arXiv+preprint+arXiv%3A2109.00859.)

[37]

Daniel Zügner, Tobias Kirschstein, Michele Catasta, Jure Leskovec, and Stephan Günnemann. 2021. Language-Agnostic Representation Learning of Source Code from Structure and Context. In International Conference on Learning Representations. https://openreview.net/forum?id=Xh5eMZVONGF

[Google Scholar](https://scholar.google.com/scholar?q=Daniel+Z%C3%BCgner%2C+Tobias+Kirschstein%2C+Michele+Catasta%2C+Jure+Leskovec%2C+and+Stephan+G%C3%BCnnemann.+2021.+Language-Agnostic+Representation+Learning+of+Source+Code+from+Structure+and+Context.+In+International+Conference+on+Learning+Representations.+https%3A%2F%2Fopenreview.net%2Fforum%3Fid%3DXh5eMZVONGF)

Show all references

## Cited By

[View all](/action/ajaxShowCitedBy?doi=10.1145/3520312.3534862 "View all cited by in new tab")

* Durán FMartinez MLago PMartínez-Fernández S(2025)Insights into resource utilization of code small language models serving with runtime engines and execution providersJournal of Systems and Software10.1016/j.jss.2025.112574**230**(112574)Online publication date: Dec-2025

  <https://doi.org/10.1016/j.jss.2025.112574>
* Bui TVu TNguyen TNguyen SVo H(2025)Correctness assessment of code generated by Large Language Models using internal representationsJournal of Systems and Software10.1016/j.jss.2025.112570**230**(112570)Online publication date: Dec-2025

  <https://doi.org/10.1016/j.jss.2025.112570>
* Da Silva LSamhi JKhomh F(2025)LLMs and Stack Overflow discussions: Reliability, impact, and challengesJournal of Systems and Software10.1016/j.jss.2025.112541**230**(112541)Online publication date: Dec-2025

  <https://doi.org/10.1016/j.jss.2025.112541>
* [Show More Cited By](javascript:void(0))

## Index Terms

1. A systematic evaluation of large language models of code

   1. [Computing methodologies](/topic/ccs2012/10010147?ContentGroupKey=10.1145%2F3520312&expand=all)

      1. [Artificial intelligence](/topic/ccs2012/10010147.10010178?ContentGroupKey=10.1145%2F3520312&expand=all)

         1. [Natural language processing](/topic/ccs2012/10010147.10010178.10010179?ContentGroupKey=10.1145%2F3520312&expand=all)
   2. [Software and its engineering](/topic/ccs2012/10011007?ContentGroupKey=10.1145%2F3520312&expand=all)

## Recommendations

* [### Hard400: A Bilingual Code Generation Evaluation Benchmark for Large Language Models](/doi/10.1007/978-981-96-9812-7_42 "Hard400: A Bilingual Code Generation Evaluation Benchmark for Large Language Models")

  Advanced Intelligent Computing Technology and Applications

  Abstract

  With the continuous development of large language models (LLMs), researchers have
  created and introduced a significant number of various code generation models. Existing
  code generation evaluation benchmarks, such as HumanEval, HumanEVAL-X, MBPP, ...

  [Read More](/doi/10.1007/978-981-96-9812-7_42 "Read More")
* [### Large Language Models for Code Translation: An In-Depth Analysis of Code Smells and Functional Correctness](/doi/10.1145/3777383 "Large Language Models for Code Translation: An In-Depth Analysis of Code Smells and Functional Correctness")

  The conversion of program code from a given source programming language (PL) to another
  target PL is known as code translation, and has a wide applicability. Since Large
  Language Models (LLMs) have shown remarkable performance across different application
  ...

  [Read More](/doi/10.1145/3777383 "Read More")
* [### Beyond Functional Correctness: Investigating Coding Style Inconsistencies in Large Language Models](/doi/10.1145/3715749 "Beyond Functional Correctness: Investigating Coding Style Inconsistencies in Large Language Models")

  Large language models (LLMs) have brought a paradigm shift to the field of code generation,
  offering the potential to enhance the software development process. However, previous
  research mainly focuses on the accuracy of code generation, while coding ...

  [Read More](/doi/10.1145/3715749 "Read More")

## Comments

Please enable JavaScript to view the[comments powered by Disqus.](https://disqus.com/?ref_noscript)

## Information & Contributors

InformationContributors

### Information

#### Published In

![cover image ACM Conferences](/cms/asset/df903b08-926e-4633-bfd3-c5eb6b74cf18/3520312.cover.jpg)

MAPS 2022: Proceedings of the 6th ACM SIGPLAN International Symposium on Machine Programming

June 2022

79 pages

ISBN:9781450392730

DOI:10.1145/3520312

* **General Chairs:**
* [![Author Picture](/pb-assets/icons/DOs/default-profile-1543932446943.svg)Swarat Chaudhuri](/profile/81309496839 "Swarat Chaudhuri")

  University of Texas at Austin, USA

  ,
* [![Author Picture](/pb-assets/icons/DOs/default-profile-1543932446943.svg)Charles Sutton](/profile/81100539852 "Charles Sutton")

  Google Research, USA

Copyright © 2022 ACM.

Permission to make digital or hard copies of all or part of this work for personal or classroom use is granted without fee provided that copies are not made or distributed for profit or commercial advantage and that copies bear this notice and the full citation on the first page. Copyrights for components of this work owned by others than the author(s) must be honored. Abstracting with credit is permitted. To copy otherwise, or republish, to post on servers or to redistribute to lists, requires prior specific permission and/or a fee. Request permissions from Permissions@acm.org.

#### Sponsors

* [SIGPLAN: ACM Special Interest Group on Programming Languages](/sig/sigplan)

#### Publisher

Association for Computing Machinery

New York, NY, United States

#### Publication History

**Published**: 13 June 2022

#### Permissions

Request permissions for this article.

[Request permissions](https://marketplace.copyright.com/rs-ui-web/mp/search/all/10.1145%2F3520312.3534862)

#### Check for updates

#### Author Tags

1. [code generation](/keyword/code+generation?expand=all)
2. [code language model](/keyword/code+language+model?expand=all)
3. [evaluation](/keyword/evaluation?expand=all)
4. [open-source](/keyword/open-source?expand=all)
5. [pretraining](/keyword/pretraining?expand=all)

#### Qualifiers

* Research-article

#### Conference

MAPS '22

Sponsor:

* [SIGPLAN](/sig/sigplan)

[MAPS '22: 6th ACM SIGPLAN International Symposium on Machine Programming](https://pldi22.sigplan.org/home/maps-2022)

June 13, 2022

CA, San Diego, USA

#### Upcoming Conference

PLDI '26

* **Sponsor:**
* [sigplan](/sig/sigplan "Special Interest Group on Programming Languages")

[ACM SIGPLAN Conference on Programming Language Design and Implementation](/conference/pldi "ACM SIGPLAN Conference on Programming Language Design and Implementation")

June 15 - 19, 2026

Boulder ,
CO ,
USA

### Contributors

![](/specs/products/acm/releasedAssets/images/loader-7e60691fbe777356dc81ff6d223a82a6.gif)

#### Other Metrics

[View Article Metrics](#tab-metrics-inner)

## Bibliometrics & Citations

BibliometricsCitations333

### Bibliometrics

#### Article Metrics

* 333

  Total Citations

  [View Citations](#tab-citations)
* 16,458

  Total Downloads

* Downloads (Last 12 months)4,141
* Downloads (Last 6 weeks)278

Reflects downloads up to 25 Nov 2025

#### Other Metrics

[View Author Metrics](#tab-contributors)

### Citations

## Cited By

[View all](/action/ajaxShowCitedBy?doi=10.1145/3520312.3534862 "View all cited by in new tab")

* Durán FMartinez MLago PMartínez-Fernández S(2025)Insights into resource utilization of code small language models serving with runtime engines and execution providersJournal of Systems and Software10.1016/j.jss.2025.112574**230**(112574)Online publication date: Dec-2025

  <https://doi.org/10.1016/j.jss.2025.112574>
* Bui TVu TNguyen TNguyen SVo H(2025)Correctness assessment of code generated by Large Language Models using internal representationsJournal of Systems and Software10.1016/j.jss.2025.112570**230**(112570)Online publication date: Dec-2025

  <https://doi.org/10.1016/j.jss.2025.112570>
* Da Silva LSamhi JKhomh F(2025)LLMs and Stack Overflow discussions: Reliability, impact, and challengesJournal of Systems and Software10.1016/j.jss.2025.112541**230**(112541)Online publication date: Dec-2025

  <https://doi.org/10.1016/j.jss.2025.112541>
* Xu HLiang Zvan Genabith JXiong DZan HLiu QZhang T(2025)Very-Long-Distance Dependency Capturing Evaluation via Language Modeling Based on Gender ConsistencyNatural Language Processing and Chinese Computing10.1007/978-981-95-3352-7\_3(27-38)Online publication date: 17-Nov-2025

  <https://doi.org/10.1007/978-981-95-3352-7_3>
* Shaon MAkter M(2025)Modern Approaches to Software Vulnerability Detection: A Survey of Machine Learning, Deep Learning, and Large Language ModelsElectronics10.3390/electronics14224449**14**:22(4449)Online publication date: 14-Nov-2025

  <https://doi.org/10.3390/electronics14224449>
* Shang XFu ZCheng SChen GLi GHu LZhang WYu N(2025)An empirical study on the effectiveness of large language models for binary code understandingEmpirical Software Engineering10.1007/s10664-025-10748-5**31**:1Online publication date: 13-Nov-2025

  <https://doi.org/10.1007/s10664-025-10748-5>
* Dietrich FZhou YWasner TKrusche SAcosta M(2025)LLM-Based Multi-Artifact Consistency Verification for Programming Exercise Quality AssuranceProceedings of the 25th Koli Calling International Conference on Computing Education Research10.1145/3769994.3770042(1-11)Online publication date: 11-Nov-2025

  <https://dl.acm.org/doi/10.1145/3769994.3770042>
* Zhu ZPeng LWang YLi YLong XCha MPark CPark NYang CBasu Roy SLi JKamps JShin KHooi BHe L(2025)FunLoc: A Novel Function-level Bug Localization Framework Enhanced by Contrastive and Active Learning StrategiesProceedings of the 34th ACM International Conference on Information and Knowledge Management10.1145/3746252.3761420(4550-4559)Online publication date: 10-Nov-2025

  <https://dl.acm.org/doi/10.1145/3746252.3761420>
* Honarvar SRei MDonaldson A(2025)The “Question Neighbourhood” Approach for Systematic Evaluation of Code-Generating LLMsIEEE Transactions on Software Engineering10.1109/TSE.2025.3612251**51**:11(3138-3167)Online publication date: Nov-2025

  <https://doi.org/10.1109/TSE.2025.3612251>
* Duan ZBian CYang S(2025)Zero-shot Forecasting of Volatile Wind Power against Data Missing with Large Language Model through Attentive Residual Prompt TuningRenewable Energy10.1016/j.renene.2025.124808(124808)Online publication date: Nov-2025

  <https://doi.org/10.1016/j.renene.2025.124808>
* [Show More Cited By](javascript:void(0))

## View Options

### View options

#### PDF

View or Download as a PDF file.

[PDF](https://dl.acm.org/doi/pdf/10.1145/3520312.3534862 "View PDF")

#### eReader

View online with eReader.

[eReader](/doi/epdf/10.1145/3520312.3534862 "View online with eReader")

## Figures

## Tables

## Media

## Share

### Share

#### Share this Publication link

https://dl.acm.org/doi/abs/10.1145/3520312.3534862

Copy Link

Copied!

Copying failed.

#### Share on social media

[X](/#twitter "Share on X")[LinkedIn](/#linkedin "Share on LinkedIn")[Reddit](/#reddit "Share on Reddit")[Facebook](/#facebook "Share on Facebook")[email](/#email "Share on email")

## References

### References

[1]

Wasi Ahmad, Saikat Chakraborty, Baishakhi Ray, and Kai-Wei Chang. 2021. Unified Pre-training for Program Understanding and Generation. In Proceedings of the 2021 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies. Association for Computational Linguistics, Online. 2655–2668. https://www.aclweb.org/anthology/2021.naacl-main.211

[Crossref](https://doi.org/10.18653/v1/2021.naacl-main.211)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.18653%2Fv1%2F2021.naacl-main.211)

[2]

Miltiadis Allamanis. 2019. The adverse effects of code duplication in machine learning models of code. In Proceedings of the 2019 ACM SIGPLAN International Symposium on New Ideas, New Paradigms, and Reflections on Programming and Software. 143–153.

[Digital Library](/doi/10.1145/3359591.3359735)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F3359591.3359735)

[3]

Uri Alon, Roy Sadaka, Omer Levy, and Eran Yahav. 2020. Structural language models of code. In International Conference on Machine Learning. 245–256.

[Google Scholar](https://scholar.google.com/scholar?q=Uri+Alon%2C+Roy+Sadaka%2C+Omer+Levy%2C+and+Eran+Yahav.+2020.+Structural+language+models+of+code.+In+International+Conference+on+Machine+Learning.+245%E2%80%93256.)

[4]

Jacob Austin, Augustus Odena, Maxwell Nye, Maarten Bosma, Henryk Michalewski, David Dohan, Ellen Jiang, Carrie Cai, Michael Terry, and Quoc Le. 2021. Program synthesis with large language models. arXiv preprint arXiv:2108.07732.

[Google Scholar](https://scholar.google.com/scholar?q=Jacob+Austin%2C+Augustus+Odena%2C+Maxwell+Nye%2C+Maarten+Bosma%2C+Henryk+Michalewski%2C+David+Dohan%2C+Ellen+Jiang%2C+Carrie+Cai%2C+Michael+Terry%2C+and+Quoc+Le.+2021.+Program+synthesis+with+large+language+models.+arXiv+preprint+arXiv%3A2108.07732.)

[5]

Alexei Baevski and Michael Auli. 2018. Adaptive input representations for neural language modeling. arXiv preprint arXiv:1809.10853.

[Google Scholar](https://scholar.google.com/scholar?q=Alexei+Baevski+and+Michael+Auli.+2018.+Adaptive+input+representations+for+neural+language+modeling.+arXiv+preprint+arXiv%3A1809.10853.)

[6]

Yoshua Bengio, Réjean Ducharme, Pascal Vincent, and Christian Jauvin. 2003. A neural probabilistic language model. Journal of machine learning research, 3, Feb (2003), 1137–1155.

[Google Scholar](https://scholar.google.com/scholar?q=Yoshua+Bengio%2C+R%C3%A9jean+Ducharme%2C+Pascal+Vincent%2C+and+Christian+Jauvin.+2003.+A+neural+probabilistic+language+model.+Journal+of+machine+learning+research%2C+3%2C+Feb+%282003%29%2C+1137%E2%80%931155.)

[7]

Sid Black, Stella Biderman, Eric Hallahan, Quentin Anthony, Leo Gao, Laurence Golding, Horace He, Connor Leahy, Kyle McDonell, Jason Phang, Michael Pieler, USVSN Sai Prashanth, Shivanshu Purohit, Laria Reynolds, Jonathan Tow, Ben Wang, and Samuel Weinbach. 2022. GPT-NeoX-20B: An Open-Source Autoregressive Language Model.

[Google Scholar](https://scholar.google.com/scholar?q=Sid+Black%2C+Stella+Biderman%2C+Eric+Hallahan%2C+Quentin+Anthony%2C+Leo+Gao%2C+Laurence+Golding%2C+Horace+He%2C+Connor+Leahy%2C+Kyle+McDonell%2C+Jason+Phang%2C+Michael+Pieler%2C+USVSN+Sai+Prashanth%2C+Shivanshu+Purohit%2C+Laria+Reynolds%2C+Jonathan+Tow%2C+Ben+Wang%2C+and+Samuel+Weinbach.+2022.+GPT-NeoX-20B%3A+An+Open-Source+Autoregressive+Language+Model.)

[8]

Sid Black, Leo Gao, Phil Wang, Connor Leahy, and Stella Biderman. 2021. GPT-Neo: Large Scale Autoregressive Language Modeling with Mesh-Tensorflow. https://doi.org/10.5281/zenodo.5297715 If you use this software, please cite it using these metadata.

[Crossref](https://doi.org/10.5281/zenodo.5297715)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.5281%2Fzenodo.5297715)

[9]

Tom B Brown, Benjamin Mann, Nick Ryder, Melanie Subbiah, Jared Kaplan, Prafulla Dhariwal, Arvind Neelakantan, Pranav Shyam, Girish Sastry, and Amanda Askell. 2020. Language models are few-shot learners. arXiv preprint arXiv:2005.14165.

[Google Scholar](https://scholar.google.com/scholar?q=Tom+B+Brown%2C+Benjamin+Mann%2C+Nick+Ryder%2C+Melanie+Subbiah%2C+Jared+Kaplan%2C+Prafulla+Dhariwal%2C+Arvind+Neelakantan%2C+Pranav+Shyam%2C+Girish+Sastry%2C+and+Amanda+Askell.+2020.+Language+models+are+few-shot+learners.+arXiv+preprint+arXiv%3A2005.14165.)

[10]

Mark Chen, Jerry Tworek, Heewoo Jun, Qiming Yuan, Henrique Ponde, Jared Kaplan, Harri Edwards, Yura Burda, Nicholas Joseph, and Greg Brockman. 2021. Evaluating large language models trained on code. arXiv preprint arXiv:2107.03374.

[Google Scholar](https://scholar.google.com/scholar?q=Mark+Chen%2C+Jerry+Tworek%2C+Heewoo+Jun%2C+Qiming+Yuan%2C+Henrique+Ponde%2C+Jared+Kaplan%2C+Harri+Edwards%2C+Yura+Burda%2C+Nicholas+Joseph%2C+and+Greg+Brockman.+2021.+Evaluating+large+language+models+trained+on+code.+arXiv+preprint+arXiv%3A2107.03374.)

[11]

Alexis Conneau and Guillaume Lample. 2019. Cross-lingual language model pretraining. Advances in Neural Information Processing Systems, 32 (2019), 7059–7069.

[Google Scholar](https://scholar.google.com/scholar?q=Alexis+Conneau+and+Guillaume+Lample.+2019.+Cross-lingual+language+model+pretraining.+Advances+in+Neural+Information+Processing+Systems%2C+32+%282019%29%2C+7059%E2%80%937069.)

[12]

Aditya Desai, Sumit Gulwani, Vineet Hingorani, Nidhi Jain, Amey Karkare, Mark Marron, and Subhajit Roy. 2016. Program synthesis using natural language. In Proceedings of the 38th International Conference on Software Engineering. 345–356.

[Digital Library](/doi/10.1145/2884781.2884786)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F2884781.2884786)

[13]

Jacob Devlin, Ming-Wei Chang, Kenton Lee, and Kristina Toutanova. 2018. BERT: Pre-training of deep bidirectional transformers for language understanding. arXiv preprint arXiv:1810.04805.

[Google Scholar](https://scholar.google.com/scholar?q=Jacob+Devlin%2C+Ming-Wei+Chang%2C+Kenton+Lee%2C+and+Kristina+Toutanova.+2018.+BERT%3A+Pre-training+of+deep+bidirectional+transformers+for+language+understanding.+arXiv+preprint+arXiv%3A1810.04805.)

[14]

Zhangyin Feng, Daya Guo, Duyu Tang, Nan Duan, Xiaocheng Feng, Ming Gong, Linjun Shou, Bing Qin, Ting Liu, and Daxin Jiang. 2020. Codebert: A pre-trained model for programming and natural languages. arXiv preprint arXiv:2002.08155.

[Google Scholar](https://scholar.google.com/scholar?q=Zhangyin+Feng%2C+Daya+Guo%2C+Duyu+Tang%2C+Nan+Duan%2C+Xiaocheng+Feng%2C+Ming+Gong%2C+Linjun+Shou%2C+Bing+Qin%2C+Ting+Liu%2C+and+Daxin+Jiang.+2020.+Codebert%3A+A+pre-trained+model+for+programming+and+natural+languages.+arXiv+preprint+arXiv%3A2002.08155.)

[15]

Leo Gao, Stella Biderman, Sid Black, Laurence Golding, Travis Hoppe, Charles Foster, Jason Phang, Horace He, Anish Thite, and Noa Nabeshima. 2020. The pile: An 800gb dataset of diverse text for language modeling. arXiv preprint arXiv:2101.00027.

[Google Scholar](https://scholar.google.com/scholar?q=Leo+Gao%2C+Stella+Biderman%2C+Sid+Black%2C+Laurence+Golding%2C+Travis+Hoppe%2C+Charles+Foster%2C+Jason+Phang%2C+Horace+He%2C+Anish+Thite%2C+and+Noa+Nabeshima.+2020.+The+pile%3A+An+800gb+dataset+of+diverse+text+for+language+modeling.+arXiv+preprint+arXiv%3A2101.00027.)

[16]

Xu Han, Zhengyan Zhang, Ning Ding, Yuxian Gu, Xiao Liu, Yuqi Huo, Jiezhong Qiu, Liang Zhang, Wentao Han, and Minlie Huang. 2021. Pre-trained models: Past, present and future. AI Open.

[Google Scholar](https://scholar.google.com/scholar?q=Xu+Han%2C+Zhengyan+Zhang%2C+Ning+Ding%2C+Yuxian+Gu%2C+Xiao+Liu%2C+Yuqi+Huo%2C+Jiezhong+Qiu%2C+Liang+Zhang%2C+Wentao+Han%2C+and+Minlie+Huang.+2021.+Pre-trained+models%3A+Past%2C+present+and+future.+AI+Open.)

[17]

Vincent J Hellendoorn and Premkumar Devanbu. 2017. Are deep neural networks the best choice for modeling source code? In Proceedings of the 2017 11th Joint Meeting on Foundations of Software Engineering. 763–773.

[Digital Library](/doi/10.1145/3106237.3106290)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F3106237.3106290)

[18]

Vincent J. Hellendoorn and Anand Ashok Sawant. 2021. The Growing Cost of Deep Learning for Source Code. Commun. ACM, 65, 1 (2021), dec, 31–33. issn:0001-0782 https://doi.org/10.1145/3501261

[Digital Library](/doi/10.1145/3501261)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F3501261)

[19]

Abram Hindle, Earl T Barr, Mark Gabel, Zhendong Su, and Premkumar Devanbu. 2016. On the naturalness of software. Commun. ACM, 59, 5 (2016), 122–131.

[Digital Library](/doi/10.1145/2902362)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F2902362)

[20]

Ari Holtzman, Jan Buys, Li Du, Maxwell Forbes, and Yejin Choi. 2019. The curious case of neural text degeneration. arXiv preprint arXiv:1904.09751.

[Google Scholar](https://scholar.google.com/scholar?q=Ari+Holtzman%2C+Jan+Buys%2C+Li+Du%2C+Maxwell+Forbes%2C+and+Yejin+Choi.+2019.+The+curious+case+of+neural+text+degeneration.+arXiv+preprint+arXiv%3A1904.09751.)

[21]

Hamel Husain, Ho-Hsiang Wu, Tiferet Gazit, Miltiadis Allamanis, and Marc Brockschmidt. 2019. Codesearchnet challenge: Evaluating the state of semantic code search. arXiv preprint arXiv:1909.09436.

[Google Scholar](https://scholar.google.com/scholar?q=Hamel+Husain%2C+Ho-Hsiang+Wu%2C+Tiferet+Gazit%2C+Miltiadis+Allamanis%2C+and+Marc+Brockschmidt.+2019.+Codesearchnet+challenge%3A+Evaluating+the+state+of+semantic+code+search.+arXiv+preprint+arXiv%3A1909.09436.)

[22]

Aditya Kanade, Petros Maniatis, Gogul Balakrishnan, and Kensen Shi. 2020. Learning and evaluating contextual embedding of source code. In International Conference on Machine Learning. 5110–5121.

[Google Scholar](https://scholar.google.com/scholar?q=Aditya+Kanade%2C+Petros+Maniatis%2C+Gogul+Balakrishnan%2C+and+Kensen+Shi.+2020.+Learning+and+evaluating+contextual+embedding+of+source+code.+In+International+Conference+on+Machine+Learning.+5110%E2%80%935121.)

[23]

Rafael-Michael Karampatsis, Hlib Babii, Romain Robbes, Charles Sutton, and Andrea Janes. 2020. Big code!= big vocabulary: Open-vocabulary models for source code. In 2020 IEEE/ACM 42nd International Conference on Software Engineering (ICSE). 1073–1085.

[Digital Library](/doi/10.1145/3377811.3380342)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F3377811.3380342)

[24]

Mike Lewis, Yinhan Liu, Naman Goyal, Marjan Ghazvininejad, Abdelrahman Mohamed, Omer Levy, Ves Stoyanov, and Luke Zettlemoyer. 2019. Bart: Denoising sequence-to-sequence pre-training for natural language generation, translation, and comprehension. arXiv preprint arXiv:1910.13461.

[Google Scholar](https://scholar.google.com/scholar?q=Mike+Lewis%2C+Yinhan+Liu%2C+Naman+Goyal%2C+Marjan+Ghazvininejad%2C+Abdelrahman+Mohamed%2C+Omer+Levy%2C+Ves+Stoyanov%2C+and+Luke+Zettlemoyer.+2019.+Bart%3A+Denoising+sequence-to-sequence+pre-training+for+natural+language+generation%2C+translation%2C+and+comprehension.+arXiv+preprint+arXiv%3A1910.13461.)

[25]

Shuai Lu, Daya Guo, Shuo Ren, Junjie Huang, Alexey Svyatkovskiy, Ambrosio Blanco, Colin Clement, Dawn Drain, Daxin Jiang, Duyu Tang, Ge Li, Lidong Zhou, Linjun Shou, Long Zhou, Michele Tufano, MING GONG, Ming Zhou, Nan Duan, Neel Sundaresan, Shao Kun Deng, Shengyu Fu, and Shujie LIU. 2021. CodeXGLUE: A Machine Learning Benchmark Dataset for Code Understanding and Generation. In Thirty-fifth Conference on Neural Information Processing Systems Datasets and Benchmarks Track (Round 1). https://openreview.net/forum?id=6lE4dQXaUcb

[Google Scholar](https://scholar.google.com/scholar?q=Shuai+Lu%2C+Daya+Guo%2C+Shuo+Ren%2C+Junjie+Huang%2C+Alexey+Svyatkovskiy%2C+Ambrosio+Blanco%2C+Colin+Clement%2C+Dawn+Drain%2C+Daxin+Jiang%2C+Duyu+Tang%2C+Ge+Li%2C+Lidong+Zhou%2C+Linjun+Shou%2C+Long+Zhou%2C+Michele+Tufano%2C+MING+GONG%2C+Ming+Zhou%2C+Nan+Duan%2C+Neel+Sundaresan%2C+Shao+Kun+Deng%2C+Shengyu+Fu%2C+and+Shujie+LIU.+2021.+CodeXGLUE%3A+A+Machine+Learning+Benchmark+Dataset+for+Code+Understanding+and+Generation.+In+Thirty-fifth+Conference+on+Neural+Information+Processing+Systems+Datasets+and+Benchmarks+Track+%28Round+1%29.+https%3A%2F%2Fopenreview.net%2Fforum%3Fid%3D6lE4dQXaUcb)

[26]

Hammond Pearce, Baleegh Ahmad, Benjamin Tan, Brendan Dolan-Gavitt, and Ramesh Karri. 2021. An Empirical Cybersecurity Evaluation of GitHub Copilot’s Code Contributions. arXiv preprint arXiv:2108.09293.

[Google Scholar](https://scholar.google.com/scholar?q=Hammond+Pearce%2C+Baleegh+Ahmad%2C+Benjamin+Tan%2C+Brendan+Dolan-Gavitt%2C+and+Ramesh+Karri.+2021.+An+Empirical+Cybersecurity+Evaluation+of+GitHub+Copilot%E2%80%99s+Code+Contributions.+arXiv+preprint+arXiv%3A2108.09293.)

[27]

Alec Radford, Jeffrey Wu, Rewon Child, David Luan, Dario Amodei, and Ilya Sutskever. 2019. Language models are unsupervised multitask learners. OpenAI blog, 1, 8 (2019), 9.

[Google Scholar](https://scholar.google.com/scholar?q=Alec+Radford%2C+Jeffrey+Wu%2C+Rewon+Child%2C+David+Luan%2C+Dario+Amodei%2C+and+Ilya+Sutskever.+2019.+Language+models+are+unsupervised+multitask+learners.+OpenAI+blog%2C+1%2C+8+%282019%29%2C+9.)

[28]

Colin Raffel, Noam Shazeer, Adam Roberts, Katherine Lee, Sharan Narang, Michael Matena, Yanqi Zhou, Wei Li, and Peter J Liu. 2019. Exploring the limits of transfer learning with a unified text-to-text transformer. arXiv preprint arXiv:1910.10683.

[Google Scholar](https://scholar.google.com/scholar?q=Colin+Raffel%2C+Noam+Shazeer%2C+Adam+Roberts%2C+Katherine+Lee%2C+Sharan+Narang%2C+Michael+Matena%2C+Yanqi+Zhou%2C+Wei+Li%2C+and+Peter+J+Liu.+2019.+Exploring+the+limits+of+transfer+learning+with+a+unified+text-to-text+transformer.+arXiv+preprint+arXiv%3A1910.10683.)

[29]

Veselin Raychev, Martin Vechev, and Eran Yahav. 2014. Code completion with statistical language models. In Proceedings of the 35th ACM SIGPLAN Conference on Programming Language Design and Implementation. 419–428.

[Digital Library](/doi/10.1145/2594291.2594321)

[Google Scholar](https://scholar.google.com/scholar_lookup?doi=10.1145%2F2594291.2594321)

[30]

Rico Sennrich, Barry Haddow, and Alexandra Birch. 2015. Neural machine translation of rare words with subword units. arXiv preprint arXiv:1508.07909.

[Google Scholar](https://scholar.google.com/scholar?q=Rico+Sennrich%2C+Barry+Haddow%2C+and+Alexandra+Birch.+2015.+Neural+machine+translation+of+rare+words+with+subword+units.+arXiv+preprint+arXiv%3A1508.07909.)

[31]

Emma Strubell, Ananya Ganesh, and Andrew McCallum. 2019. Energy and policy considerations for deep learning in NLP. arXiv preprint arXiv:1906.02243.

[Google Scholar](https://scholar.google.com/scholar?q=Emma+Strubell%2C+Ananya+Ganesh%2C+and+Andrew+McCallum.+2019.+Energy+and+policy+considerations+for+deep+learning+in+NLP.+arXiv+preprint+arXiv%3A1906.02243.)

[32]

Lewis Tunstall, Leandro von Werra, and Thomas Wolf. 2022. Natural Language Processing with Transformers. " O’Reilly Media, Inc.".

[Google Scholar](https://scholar.google.com/scholar?q=Lewis+Tunstall%2C+Leandro+von+Werra%2C+and+Thomas+Wolf.+2022.+Natural+Language+Processing+with+Transformers.+%22+O%E2%80%99Reilly+Media%2C+Inc.%22.)

[33]

Morteza Verdi, Ashkan Sami, Jafar Akhondali, Foutse Khomh, Gias Uddin, and Alireza Karami Motlagh. 2020. An empirical study of c++ vulnerabilities in crowd-sourced code examples. IEEE Transactions on Software Engineering.

[Google Scholar](https://scholar.google.com/scholar?q=Morteza+Verdi%2C+Ashkan+Sami%2C+Jafar+Akhondali%2C+Foutse+Khomh%2C+Gias+Uddin%2C+and+Alireza+Karami+Motlagh.+2020.+An+empirical+study+of+c%2B%2B+vulnerabilities+in+crowd-sourced+code+examples.+IEEE+Transactions+on+Software+Engineering.)

[34]

Eric Wallace, Tony Z Zhao, Shi Feng, and Sameer Singh. 2020. Concealed data poisoning attacks on NLP models. arXiv preprint arXiv:2010.12563.

[Google Scholar](https://scholar.google.com/scholar?q=Eric+Wallace%2C+Tony+Z+Zhao%2C+Shi+Feng%2C+and+Sameer+Singh.+2020.+Concealed+data+poisoning+attacks+on+NLP+models.+arXiv+preprint+arXiv%3A2010.12563.)

[35]

Ben Wang and Aran Komatsuzaki. 2021. GPT-J-6B: A 6 Billion Parameter Autoregressive Language Model. https://github.com/kingoflolz/mesh-transformer-jax

[Google Scholar](https://scholar.google.com/scholar?q=Ben+Wang+and+Aran+Komatsuzaki.+2021.+GPT-J-6B%3A+A+6+Billion+Parameter+Autoregressive+Language+Model.+https%3A%2F%2Fgithub.com%2Fkingoflolz%2Fmesh-transformer-jax)

[36]

Yue Wang, Weishi Wang, Shafiq Joty, and Steven CH Hoi. 2021. Codet5: Identifier-aware unified pre-trained encoder-decoder models for code understanding and generation. arXiv preprint arXiv:2109.00859.

[Google Scholar](https://scholar.google.com/scholar?q=Yue+Wang%2C+Weishi+Wang%2C+Shafiq+Joty%2C+and+Steven+CH+Hoi.+2021.+Codet5%3A+Identifier-aware+unified+pre-trained+encoder-decoder+models+for+code+understanding+and+generation.+arXiv+preprint+arXiv%3A2109.00859.)

[37]

Daniel Zügner, Tobias Kirschstein, Michele Catasta, Jure Leskovec, and Stephan Günnemann. 2021. Language-Agnostic Representation Learning of Source Code from Structure and Context. In International Conference on Learning Representations. https://openreview.net/forum?id=Xh5eMZVONGF

[Google Scholar](https://scholar.google.com/scholar?q=Daniel+Z%C3%BCgner%2C+Tobias+Kirschstein%2C+Michele+Catasta%2C+Jure+Leskovec%2C+and+Stephan+G%C3%BCnnemann.+2021.+Language-Agnostic+Representation+Learning+of+Source+Code+from+Structure+and+Context.+In+International+Conference+on+Learning+Representations.+https%3A%2F%2Fopenreview.net%2Fforum%3Fid%3DXh5eMZVONGF)

#### Affiliations

---

*爬取时间: 2025-11-28 21:55:17*
