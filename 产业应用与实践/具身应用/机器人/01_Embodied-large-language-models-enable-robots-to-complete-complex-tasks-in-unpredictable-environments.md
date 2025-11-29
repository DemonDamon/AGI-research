# Embodied large language models enable robots to complete complex tasks in unpredictable environments

**来源**: [https://www.nature.com/articles/s42256-025-01005-x](https://www.nature.com/articles/s42256-025-01005-x)

---

# Embodied large language models enable robots to complete complex tasks in unpredictable environments | Nature Machine Intelligence

原文链接: https://www.nature.com/articles/s42256-025-01005-x

[Download PDF](/articles/s42256-025-01005-x.pdf)

* Article
* [Open access](https://www.springernature.com/gp/open-science/about/the-fundamentals-of-open-access-and-open-research)
* Published: 19 March 2025

# Embodied large language models enable robots to complete complex tasks in unpredictable environments

* [Ruaridh Mon-Williams](#auth-Ruaridh-Mon_Williams-Aff1-Aff2-Aff3) 
  [ORCID: orcid.org/0009-0001-3583-8247](https://orcid.org/0009-0001-3583-8247)[1](#Aff1),[2](#Aff2),[3](#Aff3),
* [Gen Li](#auth-Gen-Li-Aff1) 
  [ORCID: orcid.org/0000-0001-6636-1106](https://orcid.org/0000-0001-6636-1106)[1](#Aff1),
* [Ran Long](#auth-Ran-Long-Aff1) 
  [ORCID: orcid.org/0000-0002-2094-0652](https://orcid.org/0000-0002-2094-0652)[1](#Aff1),
* [Wenqian Du](#auth-Wenqian-Du-Aff1-Aff4) 
  [ORCID: orcid.org/0000-0002-3352-0809](https://orcid.org/0000-0002-3352-0809)[1](#Aff1),[4](#Aff4) &
* …
* [Christopher G. Lucas](#auth-Christopher_G_-Lucas-Aff1)[1](#Aff1)

Show authors

[*Nature Machine Intelligence*](/natmachintell)
**volume 7**, pages 592–601 (2025)[Cite this article](#citeas)

* 60k Accesses
* 31 Citations
* 1334 Altmetric
* [Metrics details](/articles/s42256-025-01005-x/metrics)

### Subjects

* [Computer science](/subjects/computer-science)
* [Engineering](/subjects/engineering)

## Abstract

Completing complex tasks in unpredictable settings challenges robotic systems, requiring a step change in machine intelligence. Sensorimotor abilities are considered integral to human intelligence. Thus, biologically inspired machine intelligence might usefully combine artificial intelligence with robotic sensorimotor capabilities. Here we report an embodied large-language-model-enabled robot (ELLMER) framework, utilizing GPT-4 and a retrieval-augmented generation infrastructure, to enable robots to complete long-horizon tasks in unpredictable settings. The method extracts contextually relevant examples from a knowledge base, producing action plans that incorporate force and visual feedback and enabling adaptation to changing conditions. We tested ELLMER on a robot tasked with coffee making and plate decoration; these tasks consist of a sequence of sub-tasks from drawer opening to pouring, each benefiting from distinct feedback types and methods. We show that the ELLMER framework allows the robot to complete the tasks. This demonstration marks progress towards scalable, efficient and ‘intelligent robots’ able to complete complex tasks in uncertain environments.

### Similar content being viewed by others

![](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/ca34c517d2269caebce9855cc5c3888d.png)

### [Hierarchical generative modelling for autonomous robots](https://www.nature.com/articles/s42256-023-00752-z?fromPaywallRec=false)

Article
Open access
02 November 2023

![](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/7e912e040a2847ce119a0ffdde5ebf51.png)

### [LLM-based robot personality simulation and cognitive system](https://www.nature.com/articles/s41598-025-01528-8?fromPaywallRec=false)

Article
Open access
16 May 2025

![](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/35cd943c1e5c4fd43ba1ef65e0cc97df.png)

### [Exploration-based model learning with self-attention for risk-sensitive robot control](https://www.nature.com/articles/s44182-023-00006-5?fromPaywallRec=false)

Article
Open access
07 December 2023

## Main

If Deep Blue (the first computer to win a chess match against a reigning world champion) was truly intelligent, then should it not be able to move its own pieces when playing chess? Intelligence is a multifaceted construct and, thus, difficult to define. Consequently, human intelligence and its assessment is a controversial topic[1](/articles/s42256-025-01005-x#ref-CR1 "Intelligence research should not be held back by its past. Nature 545, 385–386 (2017)."). However, there is a growing consensus that human intelligence is best understood as ‘embodied cognition’, where attention, language, learning, memory and perception are not abstract cognitive processes constrained to the brain but intrinsically linked with how the body interacts with its surrounding environment[2](/articles/s42256-025-01005-x#ref-CR2 "Friston, K. Embodied inference and spatial cognition. Cogn. Process. 13, 497–514 (2012)."),[3](/articles/s42256-025-01005-x#ref-CR3 "Wilson, M. Six views of embodied cognition. Psychon. Bull. Rev. 9, 625–636 (2002)."). Indeed, there is growing evidence that human intelligence has its ontological and phylogenetic foundations in sensorimotor processes[4](/articles/s42256-025-01005-x#ref-CR4 "Clark, A. An embodied cognitive science. Trends Cogn. Sci. 3, 345–351 (1999).").

Embodied cognition has theoretical implications for ‘machine intelligence’ as it suggests that machines will be unable to demonstrate some aspects of intelligence if ‘cognitive’ processes are not embedded in a robotic device. This is a conjecture that is still to be tested, but ‘intelligent robots’ provide an effective way of exploring various hypotheses concerning human intelligence and advancing the field of machine intelligence. More practically, effective human–robot collaboration will ultimately require robots to at least approximate ‘human-like’ capabilities. Thus, a reasonable expectation of future ‘intelligent machines’ is that they will have the potential to perform abstract cognitive computations as they skilfully interact with objects and humans within their environment[5](/articles/s42256-025-01005-x#ref-CR5 "Stella, F., Della Santina, C. & Hughes, J. How can LLMs transform the robotic design process? Nat. Mach. Intell. 5, 561–564 (2023).").

So far, parallel streams of activity have advanced: (1) the sensorimotor abilities of robots and (2) artificial intelligence[6](/articles/s42256-025-01005-x#ref-CR6 "Miriyev, A. & Kovac, M. Skills for physical artificial intelligence. Nat. Mach. Intell. 2, 658–660 (2020)."). We set out to test the hypothesis that these approaches can now be combined to create a step change in the ability of robots to show human-like intelligence. We further hypothesized that integrating (1) and (2) would allow robots to undertake the type of complex tasks that are practically useful in a wide range of settings but currently outwith the capability of robotic systems. Consider a scenario in which someone returns home feeling fatigued and thirsty. A robot with a sophisticated manipulation system is situated in the homeowner’s kitchen and is instructed to prepare a drink. The robot decides that a reinvigorating cup of coffee needs to be made and handed to their carbon companion. This task—straightforward for humans—encompasses a series of challenges that test the limits of current robotic capabilities[7](#ref-CR7 "Cui, J. & Trinkle, J. Toward next-generation learned robot manipulation. Sci. Robot. 6, eabd9461 (2021)."),[8](#ref-CR8 "Arents, J. & Greitans, M. Smart industrial robot control trends, challenges and opportunities within manufacturing. Appl. Sci. 12, 937 (2022)."),[9](#ref-CR9 "Billard, A. & Kragic, D. Trends and challenges in robot manipulation. Science 364, eaat8414 (2019)."),[10](#ref-CR10 "Yang, G.-Z. et al. The grand challenges of Science Robotics. Sci. Robot. 3, eaar7650 (2018)."),[11](/articles/s42256-025-01005-x#ref-CR11 "Buchanan, R., Rofer, A., Moura, J., Valada, A. & Vijayakumar, S. Online estimation of articulated objects with factor graphs using vision and proprioceptive sensing. In 2024 IEEE International Conference on Robotics and Automation (ICRA) 16111–16117 (IEEE, 2024)."). First, the robot must interpret the information it receives and analyse its surroundings. Next, it may need to search the environment to locate a mug. This could involve opening drawers with unspecified opening mechanisms. Then, the robot must measure and mix the precise ratio of water to coffee. This requires fine-grained force control and adaptation to uncertainty if, for example, the human moves the location of the mug unexpectedly[9](/articles/s42256-025-01005-x#ref-CR9 "Billard, A. & Kragic, D. Trends and challenges in robot manipulation. Science 364, eaat8414 (2019)."),[12](/articles/s42256-025-01005-x#ref-CR12 "Nikolaidis, S., Ramakrishnan, R., Gu, K. & Shah, J. Efficient model learning from joint-action demonstrations for human-robot collaborative tasks. In 2015 10th ACM/IEEE International Conference on Human-Robot Interaction (HRI) 189–196 (IEEE, 2015)."). This scenario is a canonical example of the multifaceted nature of complex tasks in dynamic environments. Robotic systems have traditionally struggled with these tasks because they have been unable to follow high-level commands, have relied on preprogrammed responses and lack the flexibility to adapt seamlessly to perturbations[13](/articles/s42256-025-01005-x#ref-CR13 "Saveriano, M., Abu-Dakka, F. J., Kramberger, A. & Peternel, L. Dynamic movement primitives in robotics: a tutorial survey. Int. J. Robot. Res. 42, 1133–1184 (2023)."),[14](/articles/s42256-025-01005-x#ref-CR14 "Kober, J. et al. Movement templates for learning of hitting and batting. In 2010 IEEE International Conference on Robotics and Automation 853–858 (IEEE, 2010).").

Reinforcement learning and imitation learning have demonstrated the effectiveness of interaction and demonstration in teaching robots to perform complex tasks. These approaches are promising[15](/articles/s42256-025-01005-x#ref-CR15 "Huang, W. et al. VoxPoser: composable 3D value maps for robotic manipulation with language models. In Proc. 7th Conference on Robot Learning 540–562 (PMLR, 2023)."), but often struggle with adaptation to novel tasks and coping with diverse scenarios. Imitation learning also faces challenges when a robot needs to adapt to new contexts[16](#ref-CR16 "Zhang, D. et al. Explainable hierarchical imitation learning for robotic drink pouring. In IEEE Transactions on Automation Science and Engineering 3871–3887 (2022)."),[17](#ref-CR17 "Hussein, A., Gaber, M. M., Elyan, E. & Jayne, C. Imitation learning: a survey of learning methods. ACM Comput. Surv. 50, 21:1–21:35 (2017)."),[18](#ref-CR18 "Di Palo, N. & Johns, E. DINOBot: robot manipulation via retrieval and alignment with vision foundation models. In International Conference on Robotics and Automation (ICRA) 2798–805 (IEEE, 2024)."),[19](#ref-CR19 "Shridhar, M., Manuelli, L. & Fox, D. CLIPort: what and where pathways for robotic manipulation. In Proc. 5th Conference on Robot Learning 894–906 (PMLR, 2022)."),[20](#ref-CR20 "Shridhar, M., Manuelli, L. & Fox, D. Perceiver-Actor: a multi-task transformer for robotic manipulation. In Proc. 6th Conference on Robot Learning 785–799 (PMLR, 2023)."),[21](#ref-CR21 "Mees, O., Hermann, L. & Burgard, W. What matters in language conditioned robotic imitation learning over unstructured data. IEEE Robot. Autom. Lett. 7, 11205–11212 (2022)."),[22](#ref-CR22 "Mees, O., Borja-Diaz, J. & Burgard, W. Grounding language with visual affordances over unstructured data. In 2023 IEEE International Conference on Robotics and Automation (ICRA) 11576–11582 (IEEE, 2023)."),[23](/articles/s42256-025-01005-x#ref-CR23 "Shao, L., Migimatsu, T., Zhang, Q., Yang, K. & Bohg, J. Concept2Robot: learning manipulation concepts from instructions and human demonstrations. Int. J. Robot. Res. 40, 1419–1434 (2021)."). Nature-inspired machine intelligence provides a potential solution to these challenges. The sophistication of human manipulation is due, in part, to the type of cognitive processes that are captured artificially by large language models (LLMs)[24](#ref-CR24 "Ichter, B. et al. Do as I can, not as I say: grounding language in robotic affordances. In Proc. 6th Conference on Robot Learning 287–318 (PMLR, 2023)."),[25](#ref-CR25 "Driess, D. et al. PaLM-E: an embodied multimodal language model. In Proc. 40th International Conference on Machine Learning 8469–8488 (PMLR, 2023)."),[26](/articles/s42256-025-01005-x#ref-CR26 "Peng, A. et al. Preference-conditioned language-guided abstraction. In Proc. 2024 ACM/IEEE International Conference on Human-Robot Interaction, HRI ’24 572–581 (Association for Computing Machinery, 2024)."). LLMs offer a way to process complex instructions and adapt actions accordingly because of their advanced contextual understanding and generalization abilities[27](/articles/s42256-025-01005-x#ref-CR27 "Huang, W., Abbeel, P., Pathak, D. & Mordatch, I. Language models as zero-shot planners: extracting actionable knowledge for embodied agents. In Proc. 39th International Conference on Machine Learning 9118–9147 (PMLR, 2022)."),[28](/articles/s42256-025-01005-x#ref-CR28 "Huang, J. & Chang, K. C.-C. Towards reasoning in large language models: a survey. In Findings of the Association for Computational Linguistics: ACL 2023 1049–1065 (Association for Computational Linguistics, 2023).").

A large body of recent research has used LLMs for short-horizon tasks[15](/articles/s42256-025-01005-x#ref-CR15 "Huang, W. et al. VoxPoser: composable 3D value maps for robotic manipulation with language models. In Proc. 7th Conference on Robot Learning 540–562 (PMLR, 2023)."),[27](/articles/s42256-025-01005-x#ref-CR27 "Huang, W., Abbeel, P., Pathak, D. & Mordatch, I. Language models as zero-shot planners: extracting actionable knowledge for embodied agents. In Proc. 39th International Conference on Machine Learning 9118–9147 (PMLR, 2022)."),[29](/articles/s42256-025-01005-x#ref-CR29 "Zitkovich, B. et al. RT-2: vision-language-action models transfer web knowledge to robotic control. In Proc. 7th Conference on Robot Learning 2165–2183 (PMLR, 2023)."). For instance, VoxPoser utilizes LLMs to perform a variety of everyday manipulation tasks[15](/articles/s42256-025-01005-x#ref-CR15 "Huang, W. et al. VoxPoser: composable 3D value maps for robotic manipulation with language models. In Proc. 7th Conference on Robot Learning 540–562 (PMLR, 2023)."). Similarly, Robotics Transformer (RT-2) leverages large-scale web and robotic learning data, enabling robots to perform tasks beyond the training scenario with remarkable adaptability[29](/articles/s42256-025-01005-x#ref-CR29 "Zitkovich, B. et al. RT-2: vision-language-action models transfer web knowledge to robotic control. In Proc. 7th Conference on Robot Learning 2165–2183 (PMLR, 2023)."). Hierarchical diffusion policy introduces a model structure to generate context-aware motion trajectories, which enhances task-specific motions from high-level LLM decision inputs[30](/articles/s42256-025-01005-x#ref-CR30 "Ma, X., Patidar, S., Haughton, I. & James, S. Hierarchical diffusion policy for kinematics-aware multi-task robotic manipulation. In Proc. IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 18081–18090 (IEEE, 2024)."). However, challenges remain in effectively integrating LLMs into robotic manipulation. These challenges include complex prompting requirements, a lack of real-time interacting feedback, a dearth of LLM-driven work exploiting the use of force feedback and inefficient pipelines that hinder the seamless execution of tasks[15](/articles/s42256-025-01005-x#ref-CR15 "Huang, W. et al. VoxPoser: composable 3D value maps for robotic manipulation with language models. In Proc. 7th Conference on Robot Learning 540–562 (PMLR, 2023)."),[31](/articles/s42256-025-01005-x#ref-CR31 "Zhang, C., Chen, J., Li, J., Peng, Y. & Mao, Z. Large language models for human-robot interaction: a review. Biomimetic Intell. Robot. 3, 100131 (2023)."). Moreover, current approaches have neglected the application of retrieval-augmented generation (RAG)[32](/articles/s42256-025-01005-x#ref-CR32 "Lewis, P. et al. Retrieval-augmented generation for knowledge-intensive NLP tasks. In Advances in Neural Information Processing Systems 9459–9474 (Curran Associates, 2020).") in robotics despite RAG’s potential to continually update and refine robot knowledge with relevant and accurate examples (and increase the knowledge base without impacting performance). Robot capacity is also limited because force and visual feedback are typically not integrated in robot sensorimotor control[15](/articles/s42256-025-01005-x#ref-CR15 "Huang, W. et al. VoxPoser: composable 3D value maps for robotic manipulation with language models. In Proc. 7th Conference on Robot Learning 540–562 (PMLR, 2023)."),[33](/articles/s42256-025-01005-x#ref-CR33 "Raiaan, M. et al. A review on large language models: architectures, applications, taxonomies, open issues and challenges. IEEE Access 12, 26839–26874 (2024)."). This integration is crucial in scenarios such as pouring water into a moving cup, where vision is necessary to track the cup and force feedback is needed for pouring the desired amount of water when vision is occluded[16](/articles/s42256-025-01005-x#ref-CR16 "Zhang, D. et al. Explainable hierarchical imitation learning for robotic drink pouring. In IEEE Transactions on Automation Science and Engineering 3871–3887 (2022)."),[34](/articles/s42256-025-01005-x#ref-CR34 "Rozo, L., Jimenez, P. & Torras, C. Force-based robot learning of pouring skills using parametric hidden Markov models. In 9th International Workshop on Robot Motion and Control 227–232 (IEEE, 2013)."),[35](/articles/s42256-025-01005-x#ref-CR35 "Huang, Y., Wilches, J. & Sun, Y. Robot gaining accurate pouring skills through self-supervised learning and generalization. Robot. Auton. Syst. 136, 103692 (2021)."). Thus, there is a need for an innovative approach in robot manipulation that combines the latest artificial ‘cognition’ with integrated ‘sensorimotor’ visual and force feedback capabilities to effectively execute actions in the face of uncertainty. Supplementary Section [1](/articles/s42256-025-01005-x#MOESM1) provides more background on state-of-the-art approaches and their current limitations[36](#ref-CR36 "Mon-Williams, R., Stouraitis, T. & Vijayakumar, S. A behavioural transformer for effective collaboration between a robot and a non-stationary human. In 2023 32nd IEEE International Conference on Robot and Human Interactive Communication (RO-MAN) 1150–1157 (IEEE, 2023)."),[37](#ref-CR37 "Belkhale, S., Cui, Y. & Sadigh, D. Data quality in imitation learning. In Advances in Neural Information Processing Systems (NeurIPS) 80375–80395 (Curran Associates, 2024)."),[38](#ref-CR38 "Khazatsky, A. et al. DROID: a large-scale in-the-wild robot manipulation dataset. Robotics: Science and Systems; 
                  https://www.roboticsproceedings.org/rss20/p120.pdf
                  
                 (2024)."),[39](#ref-CR39 "Acosta, B., Yang, W. & Posa, M. Validating robotics simulators on real-world impacts. IEEE Robot. Autom. Lett. 7, 6471–6478 (2022)."),[40](#ref-CR40 "Alomar, A. et al. CausalSim: a causal framework for unbiased trace-driven simulation. In 20th USENIX Symposium on Networked Systems Design and Implementation (NSDI 23) 1115–1147 (USENIX Association, 2023)."),[41](#ref-CR41 "Choi, H. et al. On the use of simulation in robotics: opportunities, challenges, and suggestions for moving forward. Proc. Natl Acad. Sci. USA 118, e190785611 (2021)."),[42](#ref-CR42 "Del Aguila Ferrandis, J., Moura, J. & Vijayakumar, S. Nonprehensile planar manipulation through reinforcement learning with multimodal categorical exploration. In 2023 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS) 5606–5613 (IEEE, 2023)."),[43](#ref-CR43 "Kirk, R., Zhang, A., Grefenstette, E. & Rocktäschel, T. A survey of zero-shot generalisation in deep reinforcement learning. J. Artific. Intell. Res. 76, 201–264 (2023)."),[44](#ref-CR44 "Dai, T. et al. Analysing deep reinforcement learning agents trained with domain randomisation. Neurocomputing 493, 143–165 (2022)."),[45](#ref-CR45 "Chang, J., Uehara, M., Sreenivas, D., Kidambi, R. & Sun, W. Mitigating covariate shift in imitation learning via offline data with partial coverage. In Advances in Neural Information Processing Systems 965–979 (Curran Associates, 2021)."),[46](#ref-CR46 "Huang, W. et al. Inner monologue: embodied reasoning through planning with language models. In Proc. 6th Conference on Robot Learning 1769–1782 (PMLR, 2023)."),[47](#ref-CR47 "Nair, S., Rajeswaran, A., Kumar, V., Finn, C. & Gupta, A. R3M: a universal visual representation for robot manipulation. In Proc. 6th Conference on Robot Learning Vol. 205, 892–909 (PMLR, 2022)."),[48](#ref-CR48 "Singh, I. et al. ProgPrompt: generating situated robot task plans using large language models. In Proc. IEEE/CVF International Conference on Robotics and Automation (ICRA) 11523–11530 (IEEE, 2023)."),[49](#ref-CR49 "Song, C. H. et al. LLM-Planner: few-shot grounded planning for embodied agents with large language models. In Proc. IEEE/CVF International Conference on Computer Vision (ICCV) 2998–3009 (IEEE/CVF, 2023)."),[50](#ref-CR50 "Vemprala, S. H., Bonatti, R., Bucker, A. & Kapoor, A. ChatGPT for robotics: design principles and model abilities. IEEE Access 12, 55682–55696 (2024)."),[51](#ref-CR51 "Ding, Y., Zhang, X., Paxton, C. & Zhang, S. Task and motion planning with large language models for object rearrangement. In 2023 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS) 2086–2092 (IEEE, 2023)."),[52](#ref-CR52 "Kwon, M. et al. Toward grounded commonsense reasoning. In Proc. International Conference on Robotics and Automation (ICRA) 5463–5470 (IEEE, 2024)."),[53](/articles/s42256-025-01005-x#ref-CR53 "Hong, J., Levine, S. & Dragan, A. Learning to influence human behavior with offline reinforcement learning. In Advances in Neural Information Processing Systems (NeurIPS) 36094–36105 (Curran Associates, 2024).").

Embodied LLM-enabled robot (ELLMER) is a framework that integrates approaches in artificial intelligence and sensorimotor control to create a step change in robotic capabilities. Its usefulness arises from its combined use of vision and force for sensorimotor feedback control uniquely coupled with the cognitive capabilities afforded through an integrated LLM combined with RAG and a curated knowledge base. We hypothesized that ELLMER would allow a robot to make a cup of coffee for a human. We tested this hypothesis using a seven-degrees-of-freedom Kinova robotic arm to execute the complex, force-intensive task in an uncertain environment, leveraging integrated force and vision feedback. The overall system diagram is presented in Fig. [1](/articles/s42256-025-01005-x#Fig1).

**Fig. 1: Schematic of the system framework.**

[![figure 1](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/138d13159c21185ce28101bba0fee1dd.png)](/articles/s42256-025-01005-x/figures/1)

The schematic illustrates the system framework, showing the high-level (above the blue dashed horizontal line) and low-level (below the blue dashed horizontal line) system architecture. User queries are fed into a transformer via voice recognition software. The transformer (GPT-4) takes this input and integrates it with (i) an image (*C*) of the environment (via an azure Kinect depth camera); (ii) knowledge base of code examples, including various functions stored in a database. The transformer can decompose the higher-order abstracted task into actionable high-level sub-tasks, retrieve relevant code examples from the knowledge base, adapt them and write Python (v.3.8) code tailored to these tasks. The resultant code is then sent to the robot controller (A). The controller processes the code and sends control signals (*λ*) to the robot. The actions (*a*) are controlled with force (*F*) and vision (*V*) feedback. The model uses vision to identify the properties of different objects (for example, pose *X* of a coffee cup), so it can grasp objects accurately. The robot uses force (*f*) and torque (*τ*) feedback (available via an ATI force transducer) to manipulate objects skilfully (for example, determine how much water to pour). Feedback is necessary due to noise within the vision signal (*η*vision), the robot joint angles (*η*angle) and the force transducer signal (*η*force). The feedback updates the motion in the ROS to achieve the desired goal through velocity commands of both linear (*v**x**y**z*) and angular (*v**r**p**y*) velocities. These commands generate trajectories based on appropriate forces and spatiotemporal patterns to achieve the sub-goals. The use of feedback loops, including 40-Hz updates of the end-effector position (*p*) and orientation (*q*), allow the robot to respond to disturbance (for example, the robot tracking a cup to determine its new position after it is moved by the user).

[Full size image](/articles/s42256-025-01005-x/figures/1)

## Results

### Language integration for abstract reasoning

We found that our approach allowed the robot to respond to an abstract high-order verbal prompt (‘I’m tired, with friends due for cake soon. Can you make me a hot beverage, and decorate the plate with a random animal of your choice’) and complete the desired task of making a hot drink and drawing a shape on a plate. The video demonstrating this interaction is provided in Supplementary Video [1](/articles/s42256-025-01005-x#MOESM2). The robot responded to the prompt with the following sound output: ‘I’m setting things up to make a hot beverage, and also to decorate the plate with a random animal drawing. First, I’ll find a mug then scoop coffee and pour hot water. After that I’ll take an item, likely a pen, to draw a random animal on the plate. It sounds like a fun and cosy time with cake soon.’. In particular, the robot chose to make a cup of coffee when it responded to the request for a hot beverage for a tired human, and was able to decompose the higher-order behaviour into a series of sub-tasks.

The integration of GPT-4 (ref. [54](/articles/s42256-025-01005-x#ref-CR54 "OpenAI. GPT-4 technical report. Preprint at 
                  http://arxiv.org/abs/2303.08774
                  
                 (2024).")) was found to equip the robot with the desired capacity for abstract reasoning. GPT-4 is a language model that enables a robot to process user queries and environmental data to break down tasks into actionable steps. Our system was able to generate code and execute actions with force and vision feedback, effectively providing the robot with a form of intelligence. Our methodology was successful in creating a custom GPT-4 (refs. [54](/articles/s42256-025-01005-x#ref-CR54 "OpenAI. GPT-4 technical report. Preprint at 
                  http://arxiv.org/abs/2303.08774
                  
                 (2024)."),[55](/articles/s42256-025-01005-x#ref-CR55 "OpenAI. Custom models program: fine-tuning GPT-4 for specific domains (2023); 
                  https://platform.openai.com/docs/guides/fine-tuning/
                  
                ")) with a comprehensive database of flexible motion examples. The database successfully incorporated pouring, scooping, drawing, handovers, pick and place, and opening doors.

We found that the robot could identify and extract relevant examples for the downstream task using RAG. We explored various approaches to determine how intelligent machines could make the best use of RAG via our framework. These approaches included customizable open-source methods, such as Haystack[56](/articles/s42256-025-01005-x#ref-CR56 "Pietsch, M. et al. Haystack: the end-to-end nlp framework for pragmatic builders. GitHub 
                  https://github.com/deepset-ai/haystack
                  
                 (2019).") and Vebra[57](/articles/s42256-025-01005-x#ref-CR57 "Weaviate. Verba: the golden RAGtriever. GitHub 
                  https://github.com/weaviate/Verba
                  
                 (2023)."), as well as proprietary technologies such as Azure Cloud AI. We found that all of these approaches were viable. In our experiment, we chose the simplest method: logically organizing our curated knowledge base in a markdown file and uploading it to the custom GPT API via the ‘Knowledge’ feature in the GPT’s platform. This allowed the platform to automatically handle the retrieval processes and select between semantic search (returning relevant text chunks) or document review (providing complete documents or sections from larger texts). We chose this solution as it provided a state-of-the-art embedder and model, gave ease of use and was able to consistently produce good performance in our task. However, our framework allows the incorporation of a range of RAG techniques and ensures that the ‘intelligent robot’ is able to efficiently complete complex tasks. The curated knowledge base, combined with RAG, allowed the language model to access a large selection of low- and high-order functions, each with known uncertainties. Our tests showed that this capability enabled the robot to handle numerous scenarios effectively.

### Completing a complex task

The robot was found to skilfully execute the high-level task specified by the user and was able to access a comprehensive motion primitive database. The database included a variety of flexible examples of specific motions and these were successfully carried out by the robotic arm (Fig. [2](/articles/s42256-025-01005-x#Fig2)). Included in the database were examples of pouring liquids; scooping powders; opening doors with unknown mechanisms; picking up and placing objects; drawing any requested shape; conducting handovers; and moving in various directions, orientations or relative to specified objects. The robot was able to replicate and adapt the motions needed to execute the complex tasks requested by the user. The system enabled the robot to dynamically adjust to environmental variables and uncertainties. This enhanced the robot’s effectiveness in unpredictable conditions, and improved its flexibility and adaptability in the real-world setting.

**Fig. 2: Kinova robot in action.**

[![figure 2](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/5f737810ffd2d07f6a8882063964a9a7.png)](/articles/s42256-025-01005-x/figures/2)

**a**–**f**, Action shots of the Kinova Gen3 robot preparing coffee (**a**–**e**) and decorating a plate (**f**).

[Full size image](/articles/s42256-025-01005-x/figures/2)

### Zero-shot pose detection

We found that an Azure Kinect DK Depth Camera, set to a resolution of 640 × 576 px2 with a sample rate of 30 fps for depth sensing, was able to provide sufficient visual input for our method. We achieved calibration using a 14-cm AprilTag, and found that this allowed alignment between the camera and the robot’s base to an accuracy of less than 10−6. This setup enabled accurate object position detection within the scene. Grounded-Segment-Anything[58](/articles/s42256-025-01005-x#ref-CR58 "Kirillov, A. et al. Segment anything. In Proc. IEEE/CVF International Conference on Computer Vision (ICCV) 4015–4026 (IEEE, 2023).") was successfully deployed for our language-to-vision module.

The vision system generated a three-dimensional (3D) Voxel representation that was effective at identifying object poses in our setup (the used Grounding DINO detection module achieved an average precision of 52.5 on the COCO zero-shot transfer benchmark). For example, we found that the module was able to correctly identify the white cup we used 100% of the time under our experimental conditions.

The 3D Voxel representation contained the meshes of various objects. From these meshes, target poses were extracted at a frequency of 1/3 Hz. In principle, the system should have been able to detect any object. In the pilot work, however, we established that the system would not always accurately identify the different objects associated with making hot beverages. This was often due to confusion between objects with similar shapes or objects absent from the training dataset. We also found that occlusion caused by the robot’s end-effector could sometimes result in inaccuracies in object detection and lead to errors when we used highly cluttered environments. For example, the mean successful identification rate for a white cup was ~90% at occlusion ratios between 20% and 30%, but decreased substantially at higher occlusion ratios (for example, to ~20% for occlusion ratios between 80% and 90%). We anticipate that improvements in computer vision will enhance the ability of robots to deal with even the most visually complex environments. However, the performance of the vision system was impressive, and we found that our system could cope well with relatively unconstrained environments if the identified issues (for example, using out-of-distribution objects) were avoided (Fig. [3](/articles/s42256-025-01005-x#Fig3)).

**Fig. 3: Vision detection module.**

[![figure 3](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/64a5c98197d4315bbaee8a45a003d357.png)](/articles/s42256-025-01005-x/figures/3)

Illustration of the zero-shot vision detection module identifying a hand, white mug and black kettle, as well as extracting target poses for robotic grasping.

[Full size image](/articles/s42256-025-01005-x/figures/3)

### Force feedback

We found that an ATI multiaxis force and torque sensor provided sufficient force feedback for skilful object interaction. The sensor provided six components of force and torque, and the forces exerted by the robot’s end-effector during task execution were successfully measured. We found that the sensor’s accuracy was within ~2% of the full scale at a sampling rate of 100 Hz.

The robot was found to demonstrate a variety of motion dynamics accompanied by distinct types of force feedback during task execution. Figure [4](/articles/s42256-025-01005-x#Fig4) illustrates the forces experienced as the robot was preparing coffee and handing over a pen. As shown in Fig. [4](/articles/s42256-025-01005-x#Fig4), a diverse spectrum of external forces was handled across various tasks. For example, when putting down a mug, the peak upward force was used as an indicator of successful placement. By contrast, during drawer manipulation, the forces and torques along the *x* and *y* axes were critical, highlighting their importance for successful task execution. The variability in force feedback exemplifies the advantages of our scalable approach that adapts to the requirements of diverse motions.

**Fig. 4: Force, velocity and position feedback.**

[![figure 4](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/be823cd8dee2c4ffd58610bd7370a47b.png)](/articles/s42256-025-01005-x/figures/4)

Force (N), velocity (m s–1) and position (m) plots during the robot’s coffee preparation, illustrating the diverse force feedback across the different motions. The drawing component has been omitted for clarity.

[Full size image](/articles/s42256-025-01005-x/figures/4)

The pouring accuracy achieved was ~5.4 g per 100 g at a pitch velocity of 4 m s–1. We assumed a quasi-static equilibrium to estimate the volume of water poured at any given moment. However, as the pitch velocity increased, the accuracy decreased, with errors approaching ~20 g s–1 at a pitch velocity of 30 m s–1. This decrease in accuracy can be attributed to the breakdown of the quasi-static assumption and the impact of the mass distribution of both pouring medium and container on measurement accuracy.

### Generating art

DALL-E[59](/articles/s42256-025-01005-x#ref-CR59 "Ramesh, A. et al. Zero-shot text-to-image generation. In Proc. 38th International Conference on Machine Learning 8821–8831 (PMLR, 2021).") was found to successfully produce an image from which we could derive a drawing trajectory. It was found that this enabled the robot to draw any design specified by the user. We found that DALL-E was able to create silhouettes based on keywords extracted from the user, such as ‘random bird’ or ‘random plant’. The silhouette’s outline was extracted and transformed to match the dimensions of the target surface. This allowed the robot to replicate the design on various physical objects (Fig. [5](/articles/s42256-025-01005-x#Fig5)). We found that force feedback applied an even pen pressure when drawing, and this allowed control over the *z* component (Supplementary Section [2](/articles/s42256-025-01005-x#MOESM1)).

**Fig. 5: Drawing process visualization.**

[![figure 5](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/6e32184c09e23477b8eba2c4579e7319.png)](/articles/s42256-025-01005-x/figures/5)

Illustration of the drawing process across different queries. The top row shows the generated image, contour plot and drawing produced when instructed to create a ‘random animal’. The second row displays the corresponding outputs for a ‘random food’ and the third row illustrates the results for a ‘random plant’.

[Full size image](/articles/s42256-025-01005-x/figures/5)

### Evaluation

We evaluated our method for generating robotic plans against VoxPoser, which does not utilize RAG or force feedback. To compare the methods, we prompted an LLM to generate 80 human-like queries, reflecting the range of tasks specified in the knowledge base. These queries were then used to generate robot plans. We compared the performance outcomes from using RAG (our method)—in which the knowledge base is dynamically integrated into the LLM’s decision-making process—to a baseline (VoxPoser) in which the knowledge base was statically incorporated into the LLM’s context window. It is important to note that the second approach lacks scalability and becomes impractical as the knowledge base expands.

We evaluated the results based on answer faithfulness, which assesses an answer’s truthfulness and accuracy (ensuring factual representation without fabrication or ‘hallucination’ errors). In our findings, using RAG improved the faithfulness of responses. For GPT-4 (gpt-4-0613), the faithfulness score increased from 0.74 to 0.88 with RAG. Similarly, GPT-3.5-turbo (gpt-3.5-turbo-0125) achieved 0.86 with RAG compared with 0.78 without it, and Zephyr-7B-beta saw an increase from 0.37 to 0.44. The improvement in faithfulness is particularly key for robotic applications, where accurate execution during physical interactions is essential.

## Discussion

We tested our methodology—the ELLMER framework—that combines techniques from artificial intelligence and robot manipulation to create an intelligent robot. Our approach successfully combined the cognitive abilities of LLMs with the sensorimotor skills of robots, enabling our robot to interpret a high-order verbal command and execute a complex long-horizon task while adeptly managing uncertainties. We used the LLM, augmented with feedback loops and RAG, to write expressive code and facilitate the manipulation sub-tasks required by the robot to achieve the high-level goal (making a hot beverage). ELLMER allowed real-time adaptation to environmental changes and leveraged a repository of precise solutions via RAG. This ensured accurate task execution and broad adaptability[32](/articles/s42256-025-01005-x#ref-CR32 "Lewis, P. et al. Retrieval-augmented generation for knowledge-intensive NLP tasks. In Advances in Neural Information Processing Systems 9459–9474 (Curran Associates, 2020).").

ELLMER encoded known constraints into the code examples (‘motion functions’) and enabled rapid accommodation to numerous uncertainties, such as fluctuating ingredient quantities or opening unknown drawers—capabilities that other methods lack without extensive additional training[29](/articles/s42256-025-01005-x#ref-CR29 "Zitkovich, B. et al. RT-2: vision-language-action models transfer web knowledge to robotic control. In Proc. 7th Conference on Robot Learning 2165–2183 (PMLR, 2023)."),[33](/articles/s42256-025-01005-x#ref-CR33 "Raiaan, M. et al. A review on large language models: architectures, applications, taxonomies, open issues and challenges. IEEE Access 12, 26839–26874 (2024)."),[60](/articles/s42256-025-01005-x#ref-CR60 "Zeng, A. et al. Socratic models: composing zero-shot multimodal reasoning with language. In Proc. International Conference on Learning Representations (ICLR, 2023)."),[61](/articles/s42256-025-01005-x#ref-CR61 "Cui, Y. et al. No, to the right: online language corrections for robotic manipulation via shared autonomy. In Proc. 2023 ACM/IEEE International Conference on Human-Robot Interaction, HRI ’23 93–101 (Association for Computing Machinery, 2023)."). The integration of vision, force and language modalities enhanced the manipulation performance. The force sensors improved task precision (for example, pouring a precise and accurate amount of liquid when vision was occluded), whereas the vision system identified object positions and movements. The language capabilities enabled the system to produce feedback within the code, which is critical for adjusting to new tasks. The curated knowledge base improved the LLM’s performance by tailoring information retrieval to the specific task specifications, and this ensured high-quality contextually relevant outputs. A curated knowledge base is a pragmatic element that enhances controllability, accuracy and scalability. In this context, RAG can be seen as providing a cultural milieu of knowledge from which a robot can draw. In particular, this mirrors the ‘intelligence’ afforded to humans through the cultural transmission of knowledge. Thus, our work shows that integrating advanced language models and sensorimotor control strategies allows robots to leverage the exponential advancements in LLMs, enabling more sophisticated interactions. This will usher in the next age of automation with unprecedented levels of autonomy and precision, accentuating the need to manage these advancements safely[62](/articles/s42256-025-01005-x#ref-CR62 "Bengio, Y. et al. Managing extreme AI risks amid rapid progress. Science 384, 842–845 (2024).").

ELLMER’s potential extends to creating intricate and artistic movements. For instance, a model like DALL-E allows trajectories to be derived from visual inputs and opens new avenues for robotic trajectory generation. This method can be widely applied in tasks such as cake decoration or latte art. In future work, incorporating queries and images will enable novel trajectory generation, allowing for increased versatility. Moreover, recent LLM enhancements are set to notably improve the fluidity and effectiveness of human–robot interactions. Our examples of coffee making and plate decoration represent only a subset of the complex task types that a sophisticated robot might be required to undertake. ELLMER is conducive to being scaled up, so it includes a wide range of possible long-horizon tasks. Thus, ELLMER could incorporate a database of feedback loops or ‘learning-from-demonstration’ examples to facilitate a wide variety of complex robotic manipulations.

ELLMER is based on two assumptions concerning computer vision: (1) the vision module accurately identifies and classifies objects within the scene and (2) a comprehensive affordance map of the utensils is available. We endowed our model with prior knowledge of the kettle, spoon and door handle affordances, but recent work suggests that affordances can be learned with minimal data[63](/articles/s42256-025-01005-x#ref-CR63 "Li, G., Jampani, V., Sun, D. & Sevilla-Lara, L. Locate: localize and transfer object parts for weakly supervised affordance grounding. In Proc. IEEE/CVF Conference on Computer Vision and Pattern Recognition 10922–10931 (IEEE, 2023)."),[64](/articles/s42256-025-01005-x#ref-CR64 "Li, G., Sun, D., Sevilla-Lara, L. & Jampani, V. One-shot open affordance learning with foundation models. In Proc. IEEE/CVF Conference on Computer Vision and Pattern Recognition 3086–3096 (IEEE, 2024)."). Our focus was not on object detection, but we noted that detection response times hindered optimal performance. In addition, ELLMER could adjust to real-time changes but struggled with proactive adaptations (for example, task switching midway without prior programming). In future iterations, more frequent querying of the language model would allow the reassessment and modification of overall plans based on new inputs. We also note that there are still challenges that need to be addressed, such as the sophisticated modelling of complex force dynamics (for example, the forces on the end-effector as a function of the flow rate, container size and liquid viscosity) and the integration of spatial awareness tools (such as OctoMaps, a robotic library for a 3D occupancy map). Incorporating tactile sensors and using soft robotic techniques would improve the robot’s ability to apply appropriate forces without causing damage. ELLMER provides a flexible platform for incorporating these research developments, enabling robots to use ‘sensory’ feedback to interpret material properties and precisely tailor the forces they apply.

The current iteration of ELLMER allowed the robot to successfully complete a complex task in ‘one shot’. This provides a compelling picture of the capabilities of intelligent machines that combine sensorimotor capabilities with the abstract reasoning provided by LLMs. Nevertheless, we anticipate that the robot capacity will increase exponentially as the components combined within ELLMER become ever more refined. Our framework is hardware agnostic and can be easily customized with open-source RAG solutions like Haystack, supporting quick adjustments to embedders, retrievers, chunking techniques and LLMs. ELLMER offers a flexible framework for researchers to collaboratively develop intelligent machines. Supplementary Section [3](/articles/s42256-025-01005-x#MOESM1) provides more information on ELLMER and future research.

The power of our approach lies in the embodiment of cognition through a framework that combines enhanced sensorimotor abilities with the cognitive reasoning capabilities of LLMs. Through this combination, ELLMER enables robots to explore and interact with their environment more effectively, emulating aspects of the connection between experience and action observed in human intelligence. This opens up opportunities for robots to gain a form of ‘physical intelligence’, where their exploration of the environment drives the sensorimotor learning process. In conclusion, ELLMER integrates language processing, RAG, force and vision to enable robots to adapt to complex tasks. It combines the following features: (1) interpreting high-level human commands, (2) completing long-horizon tasks and (3) utilizing integrated force and vision signals to manage noise and disturbances in changing environments. ELLMER allows methods such as reinforcement learning, imitation learning and flexible motion primitives to be combined holistically for enhanced adaptability and ‘robot intelligence’ in diverse and dynamic scenarios. It demonstrates that integrating the cognitive reasoning capabilities of LLMs with robots’ sensorimotor skills allows them to interpret and manipulate their environment and complete complex tasks through embodied machine intelligence.

## Methods

### Overview

The goal of the robot was to respond to high-level human commands in a dynamic environment, such as a home kitchen. We designed a realistic setting featuring items including a kettle, white mug, drawers, kitchen paraphernalia and a coffee pot. The scenario was designed to test the robot’s ability to perform diverse tasks in a realistic, although reasonably constrained, environment as it interacts with a human present. We assumed that robotic low-level control mechanisms managed obstacle avoidance. The pipeline consisted of a language-processing component for task execution, a vision system for pose detection and a force module for object manipulation. All of this was integrated within a robotic operating system (ROS) process.

Specifically, our approach built on the ‘code for dynamic policies’ approach[65](/articles/s42256-025-01005-x#ref-CR65 "Liang, J. et al. Code as policies: language model programs for embodied control. In 2023 IEEE International Conference on Robotics and Automation (ICRA) 9493–9500 (IEEE, 2023).") that can facilitate adaptable robotic actions. In our implementation, we utilized GPT-4 and OpenAI’s RAG infrastructure. We leveraged LLMs’ capabilities using RAG[32](/articles/s42256-025-01005-x#ref-CR32 "Lewis, P. et al. Retrieval-augmented generation for knowledge-intensive NLP tasks. In Advances in Neural Information Processing Systems 9459–9474 (Curran Associates, 2020).") to dynamically select and adapt the most suitable policy from a database or generate its own code based on relevant examples. In contrast to existing pure LLM-driven methods[25](/articles/s42256-025-01005-x#ref-CR25 "Driess, D. et al. PaLM-E: an embodied multimodal language model. In Proc. 40th International Conference on Machine Learning 8469–8488 (PMLR, 2023)."),[27](/articles/s42256-025-01005-x#ref-CR27 "Huang, W., Abbeel, P., Pathak, D. & Mordatch, I. Language models as zero-shot planners: extracting actionable knowledge for embodied agents. In Proc. 39th International Conference on Machine Learning 9118–9147 (PMLR, 2022)."),[29](/articles/s42256-025-01005-x#ref-CR29 "Zitkovich, B. et al. RT-2: vision-language-action models transfer web knowledge to robotic control. In Proc. 7th Conference on Robot Learning 2165–2183 (PMLR, 2023)."), we integrated force and vision into the framework, allowing the system to adapt to a variety of complex tasks in dynamic settings. This approach equips the robotic system with the capacity for high-level contextual understanding[25](/articles/s42256-025-01005-x#ref-CR25 "Driess, D. et al. PaLM-E: an embodied multimodal language model. In Proc. 40th International Conference on Machine Learning 8469–8488 (PMLR, 2023).") and the proficiency to execute complex tasks with real-time feedback, ensuring accuracy and precision. The approach ensures that each action is aligned with the specific demands of the task and the environmental conditions (Fig. [6](/articles/s42256-025-01005-x#Fig6)).

**Fig. 6: Coffee and plate decoration.**

[![figure 6](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/7329f405660284699b46279db5b1b78a.png)](/articles/s42256-025-01005-x/figures/6)

Kinova Gen3 robot having prepared the coffee and decorated a plate.

[Full size image](/articles/s42256-025-01005-x/figures/6)

### Hardware and software

A Kinova seven-degrees-of-freedom robot was used. An Azure Kinect Sensor was used at a resolution of 640 × 576 px2 and 30 fps, along with an ATI multiaxis force sensor. A 140-mm Robotiq gripper was attached to the end of the robot. The force sensor was attached to the Robotiq gripper and Kinova arm using a 3D printed flange. A small cylinder was placed on the force sensor on the side closest to the gripper so that the movements of the gripper would not touch the force sensor, leading to readings being inaccurate. A Dell desktop computer with an Intel Core i9 processor with an NVIDIA RTX 2080 graphics-processing unit was used and connected to the robot with an Ethernet cable. Similarly, both Azure cameras were attached to the desktop. Ubuntu 20.04 and the ROS were used. Our code relied on the Kinova ROS Kortex library. The NVIDIA RTX 2080 utilizes ~225 W under typical load conditions[66](/articles/s42256-025-01005-x#ref-CR66 "Hong, S. & Kim, H. An integrated GPU power and performance model. In Proc. 37th Annual International Symposium on Computer Architecture 280–289 (Association for Computing Machinery, 2010)."), whereas the Kinova robotic arm consumes ~36 W (ref. [67](/articles/s42256-025-01005-x#ref-CR67 "Kinova Robotics. Kinova Gen3 Ultra-Lightweight Robotic Arm User Guide (2023); 
                  https://assets.iqr-robot.com/wp-content/uploads/2023/08/20230814163651088831.pdf
                  
                ")). In our scenarios, each task runs for up to 4 min. Utilizing the EPA’s average conversion factor of ~0.4 kg of CO2 per kWh for mixed energy sources[68](/articles/s42256-025-01005-x#ref-CR68 "US Environmental Protection Agency. GHG emission factors hub (2024); 
                  https://www.epa.gov/climateleadership/ghg-emission-factors-hub
                  
                "), the carbon emission for each task comes to ~0.007 kg (7 g) of CO2.

### Language processing

The LLM processes an image and the user’s query, systematically breaking down the complex task *L**T* into a sequence of steps {*L*1, *L*2,…, *L**N*}, where each step *L**i* may depend on the completion of the preceding steps. The sequence of steps is critical, and dependencies exist between steps; for example, if an object (for example, a mug) is required but not found, then potentially a cupboard should be opened.

The environmental data gathered from the initial image input are key in decomposing the abstract task. For instance, when asked to make a beverage, the ingredients present in the environment are critical in deciding which drink to make, and the visual information can help identify possible locations. The interface was facilitated by GPT-4, which ran under the instruction to write and dispatch code to a robot via the server platform. The process was assisted by a knowledge base containing code examples and allowed continuous communication with the robot. The curated knowledge base contained validated examples of low- and high-order actions that incorporate known uncertainties. Including these motion examples is key to enabling the robot to handle numerous scenarios and complete long-horizon tasks. High-level motion primitives or policies can compress multiple known uncertainties into a single function, reducing the need for extensive code writing. RAG allowed the knowledge base to be comprehensive without sacrificing performance. The system interacted with the ROS and communicated via a low-latency connection provided by the EC2 server through JSON action queries and responses.

The dependency among tasks is expressed through conditional probabilities such as *P*(*L*2*A*, *L*2*B*∣*L*1), which specifies the likelihood of progressing to tasks *L*2*A* or *L*2*B* following the successful execution of task *L*1. This helps in planning the sequence of steps, ensuring the robot can adapt its actions based on real-time feedback. The LLM generates executable code that is sent to the server, based on the instructions (prompt) and a knowledge base containing examples. The code is run on the ROS in a secure environment that only has access to predefined functions, thereby ensuring safety in task execution.

### RAG

A key feature of our system is the deployment of RAG. RAG integrates user queries with information from a continually updated, curated knowledge base, optimizing the output of the LLM. This approach allows the model to follow code examples provided in the database, ensuring accuracy, reliability and scalability as the knowledge base evolves.

We used vector RAG, which involves using an encoder to embed the query (*q*) and segments of the knowledge base ({*s*1, *s*2,…, *s**m*}), known as chunks, into vector representations. Chunks were then compared with the query based on cosine similarity, and the top *k* chunks were selected as contextually relevant information for generating responses. Alternative retrieval techniques that can be used within our framework include traditional RAG (keyword-/rule-based RAG) or hybrid retrieval methods.

The RAG pipeline can be customized by selecting different document stores (the medium in which the knowledge base is stored and organized). In our experimental test, we used the inbuilt OpenAI RAG process and organized our curated knowledge base in a markdown file as the document store. However, a range of other RAG approaches can be used in our framework, utilizing tools like Haystack[56](/articles/s42256-025-01005-x#ref-CR56 "Pietsch, M. et al. Haystack: the end-to-end nlp framework for pragmatic builders. GitHub 
                  https://github.com/deepset-ai/haystack
                  
                 (2019).") and Vebra[57](/articles/s42256-025-01005-x#ref-CR57 "Weaviate. Verba: the golden RAGtriever. GitHub 
                  https://github.com/weaviate/Verba
                  
                 (2023)."). These tools allow users to select a range of document stores—from ‘markdown files’ for simple text-based knowledge to ‘Elasticsearch’ for complex, indexed data—along with specific embedders, retrievers and chunking techniques, as well as the LLM itself.

### Vision system

Grounded-Segment-Anything was used as the language-to-vision model to create a 3D voxel that highlighted the positions of all objects and allowed their poses to be extracted for robotic grasping[58](/articles/s42256-025-01005-x#ref-CR58 "Kirillov, A. et al. Segment anything. In Proc. IEEE/CVF International Conference on Computer Vision (ICCV) 4015–4026 (IEEE, 2023)."),[69](/articles/s42256-025-01005-x#ref-CR69 "Liu, S. et al. Grounding DINO: marrying DINO with grounded pre-training for open-set object detection. In 2024 European Conference on Computer Vision (eds Leonardis, A. et al.) Vol. 15105 (Springer, 2023)."). This enabled (1) the generation of object-specific bounding boxes, (2) the manufacture of segmented masks via MobileSAM and (3) the creation of voxels that encapsulate the detected objects. The voxels allowed target object poses to be extracted.

### Force module

To ensure accurate measurements in force-rich applications, we calibrated the ATI force sensor to compensate for gravitational forces, ensuring it registered zero in the absence of external forces. This calibration is key for accurately predicting the external forces applied to the end-effector. The process involved sequentially zeroing the force sensor on one axis, rotating the sensor and then zeroing on the next axis. The local forces were transformed into the global plane to estimate the upward force at different rotations *F*global = *T*end\_effector\_to\_robot\_base × *F*local, where *F*global is the force vector in the global (robot base) coordinate frame, *T*end\_effector\_to\_robot\_base is the transformation matrix from the end-effector’s frame to the robot’s base frame and *F*local is the force vector in the local coordinate frame of the end-effector. We explored various methods, such as moving the sensor’s position and orientation and using polynomial functions for calibration. However, the simpler calibration method was found to be the most effective.

To estimate the flow rates, we assumed a condition of static equilibrium and maintain slow operational speeds during pouring. Mathematically, this is represented as *F*up ≈ *m**g* and Δ*F*up ≈ Δ*m**g*. In situations involving variable acceleration, the relationship between forces and flow rates becomes more complex. It necessitates a dynamic model that accounts for varying inputs, such as flow rates, container’s centre of mass and inertia of the end-effector, to map dynamic force inputs to the pouring flow rates.

The system continuously manages force vectors along three axes, adjusting the applied force based on the criteria within its knowledge base. The LLM dynamically selects the necessary force magnitudes and directions tailored to meet specific downstream task requirements. For example, the knowledge base may specify varying force magnitudes to be applied depending on the object characteristics or task demands. This approach enables the system to adjust its actions autonomously to align with a broad range of operational criteria.

### ROS operation

In this work, we initiated the robotic processes by launching a Kinova ROS Kortex driver. This established a node that enables communication within the ROS network and the Kinova Gen3 robot. The node publishes several topics that subscribers can access, and it provides services that can be called to modify the robot’s configuration. The base joints are updated at a frequency of 40 Hz. Concurrently, the Robotiq 2F-140 mm gripper node is activated at 50 Hz. The node sets up a communication link with the gripper via a USB connection, and it initiates an action server that enables precise control of the gripper and facilitates the exchange of operating data.

A vital element of our robotic system is the vision module node. A ‘classes’ variable is used to identify the target pose of selected objects within the environment. This variable can be dynamically updated, thereby allowing the system to adapt to changes in the scene. The pose coordinates of the objects, as established by the ‘classes’ variable, are published approximately at every \(\sim \frac{1}{3}\) Hz. This is largely due to the processing time of Grounding DINO in detecting objects and establishing the bounding boxes. Moreover, we used an AprilTag to determine the position of the camera relative to the robot’s base. This is represented as *P*R = *T*AR × (*T*CA × *P*C), where *P*C is the point in the camera frame, *T*CA is the transformation matrix from the camera frame to the AprilTag, *T*AR is the transformation matrix from the AprilTag to the robot’s base and PR is the point in the robot’s base frame.

In parallel, a force node is launched at a frequency of 100 Hz and provides multiaxis force and torque readings, localized to the ATI force transducer. The readings are transformed using a quaternion-based 3 × 3 rotation matrix to align with the global base frame of the robot, providing raw and averaged values over the last five time steps across fixed degrees of freedom. It calculates forces in the global frame of the robot base using the rotational matrix, calculated from the kinematic data.

ROS facilitates the continuous processing of multimodal feedback data from the language processing, vision systems, force metrics and joint end-effector positions. The motions operate on a foundational six-degrees-of-freedom twist command, which controls velocity and the variable speed and force gripper procedures for opening and closing. This enables the integration of hard-coded safety constraints, such as maximum velocity and force limits, as well as workspace boundaries.

The linear velocities were clamped within ±0.05 m s–1 and the angular velocities were clamped within ±60° s–1. End-effector forces were also limited to 20 N. This is coded into the fundamental motion primitives; therefore, error in the language model will not override this. The end-effector is also clamped within the predefined workspace bounds of *x* = [0.0, 1.1], *y* = [–0.3, 0.3] and *z* = [0, 1.0]. This is checked in future time steps by a publisher at a frequency of 10 Hz.

## Data availability

The dataset used in this work is available in an open-source GitHub repository at <https://github.com/ruaridhmon/ELLMER>.

## Code availability

The code supporting this study is available via GitHub at <https://github.com/ruaridhmon/ELLMER> and has been archived in Zenodo at <https://doi.org/10.5281/zenodo.14483539> (ref. [70](/articles/s42256-025-01005-x#ref-CR70 "ruaridhmon. ruaridhmon/ELLMER: v1.0.0: Initial Release. Zenodo 
                  https://doi.org/10.5281/zenodo.14483539
                  
                 (2024).")).

## References

1. Intelligence research should not be held back by its past. *Nature* **545**, 385–386 (2017).
2. Friston, K. Embodied inference and spatial cognition. *Cogn. Process.* **13**, 497–514 (2012).

   [Article](https://link.springer.com/doi/10.1007/s10339-012-0519-z) 
   [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Embodied%20inference%20and%20spatial%20cognition&journal=Cogn.%20Process.&doi=10.1007%2Fs10339-012-0519-z&volume=13&pages=497-514&publication_year=2012&author=Friston%2CK)
3. Wilson, M. Six views of embodied cognition. *Psychon. Bull. Rev.* **9**, 625–636 (2002).

   [Article](https://doi.org/10.3758%2FBF03196322) 
   [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Six%20views%20of%20embodied%20cognition&journal=Psychon.%20Bull.%20Rev.&doi=10.3758%2FBF03196322&volume=9&pages=625-636&publication_year=2002&author=Wilson%2CM)
4. Clark, A. An embodied cognitive science. *Trends Cogn. Sci.* **3**, 345–351 (1999).

   [Article](https://doi.org/10.1016%2FS1364-6613%2899%2901361-3) 
   [Google Scholar](http://scholar.google.com/scholar_lookup?&title=An%20embodied%20cognitive%20science&journal=Trends%20Cogn.%20Sci.&doi=10.1016%2FS1364-6613%2899%2901361-3&volume=3&pages=345-351&publication_year=1999&author=Clark%2CA)
5. Stella, F., Della Santina, C. & Hughes, J. How can LLMs transform the robotic design process? *Nat. Mach. Intell.* **5**, 561–564 (2023).

   [Article](https://doi.org/10.1038%2Fs42256-023-00669-7) 
   [Google Scholar](http://scholar.google.com/scholar_lookup?&title=How%20can%20LLMs%20transform%20the%20robotic%20design%20process%3F&journal=Nat.%20Mach.%20Intell.&doi=10.1038%2Fs42256-023-00669-7&volume=5&pages=561-564&publication_year=2023&author=Stella%2CF&author=Santina%2CC&author=Hughes%2CJ)
6. Miriyev, A. & Kovac, M. Skills for physical artificial intelligence. *Nat. Mach. Intell.* **2**, 658–660 (2020).
7. Cui, J. & Trinkle, J. Toward next-generation learned robot manipulation. *Sci. Robot.* **6**, eabd9461 (2021).
8. Arents, J. & Greitans, M. Smart industrial robot control trends, challenges and opportunities within manufacturing. *Appl. Sci.* **12**, 937 (2022).
9. Billard, A. & Kragic, D. Trends and challenges in robot manipulation. *Science* **364**, eaat8414 (2019).
10. Yang, G.-Z. et al. The grand challenges of *Science Robotics*. *Sci. Robot.* **3**, eaar7650 (2018).
11. Buchanan, R., Rofer, A., Moura, J., Valada, A. & Vijayakumar, S. Online estimation of articulated objects with factor graphs using vision and proprioceptive sensing. In *2024 IEEE International Conference on Robotics and Automation (ICRA)* 16111–16117 (IEEE, 2024).
12. Nikolaidis, S., Ramakrishnan, R., Gu, K. & Shah, J. Efficient model learning from joint-action demonstrations for human-robot collaborative tasks. In *2015 10th ACM/IEEE International Conference on Human-Robot Interaction (HRI)* 189–196 (IEEE, 2015).
13. Saveriano, M., Abu-Dakka, F. J., Kramberger, A. & Peternel, L. Dynamic movement primitives in robotics: a tutorial survey. *Int. J. Robot. Res.* **42**, 1133–1184 (2023).
14. Kober, J. et al. Movement templates for learning of hitting and batting. In *2010 IEEE International Conference on Robotics and Automation* 853–858 (IEEE, 2010).
15. Huang, W. et al. VoxPoser: composable 3D value maps for robotic manipulation with language models. In *Proc. 7th Conference on Robot Learning* 540–562 (PMLR, 2023).
16. Zhang, D. et al. Explainable hierarchical imitation learning for robotic drink pouring. In *IEEE Transactions on Automation Science and Engineering* 3871–3887 (2022).
17. Hussein, A., Gaber, M. M., Elyan, E. & Jayne, C. Imitation learning: a survey of learning methods. *ACM Comput. Surv.* **50**, 21:1–21:35 (2017).

    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Imitation%20learning%3A%20a%20survey%20of%20learning%20methods&journal=ACM%20Comput.%20Surv.&volume=50&publication_year=2017&author=Hussein%2CA&author=Gaber%2CMM&author=Elyan%2CE&author=Jayne%2CC)
18. Di Palo, N. & Johns, E. DINOBot: robot manipulation via retrieval and alignment with vision foundation models. In *International Conference on Robotics and Automation (ICRA)* 2798–805 (IEEE, 2024).
19. Shridhar, M., Manuelli, L. & Fox, D. CLIPort: what and where pathways for robotic manipulation. In *Proc. 5th Conference on Robot Learning* 894–906 (PMLR, 2022).
20. Shridhar, M., Manuelli, L. & Fox, D. Perceiver-Actor: a multi-task transformer for robotic manipulation. In *Proc. 6th Conference on Robot Learning* 785–799 (PMLR, 2023).
21. Mees, O., Hermann, L. & Burgard, W. What matters in language conditioned robotic imitation learning over unstructured data. *IEEE Robot. Autom. Lett.* **7**, 11205–11212 (2022).
22. Mees, O., Borja-Diaz, J. & Burgard, W. Grounding language with visual affordances over unstructured data. In *2023 IEEE International Conference on Robotics and Automation (ICRA)* 11576–11582 (IEEE, 2023).
23. Shao, L., Migimatsu, T., Zhang, Q., Yang, K. & Bohg, J. Concept2Robot: learning manipulation concepts from instructions and human demonstrations. *Int. J. Robot. Res.* **40**, 1419–1434 (2021).
24. Ichter, B. et al. Do as I can, not as I say: grounding language in robotic affordances. In *Proc. 6th Conference on Robot Learning* 287–318 (PMLR, 2023).
25. Driess, D. et al. PaLM-E: an embodied multimodal language model. In *Proc. 40th International Conference on Machine Learning* 8469–8488 (PMLR, 2023).
26. Peng, A. et al. Preference-conditioned language-guided abstraction. In *Proc. 2024 ACM/IEEE International Conference on Human-Robot Interaction, HRI ’24* 572–581 (Association for Computing Machinery, 2024).
27. Huang, W., Abbeel, P., Pathak, D. & Mordatch, I. Language models as zero-shot planners: extracting actionable knowledge for embodied agents. In *Proc. 39th International Conference on Machine Learning* 9118–9147 (PMLR, 2022).
28. Huang, J. & Chang, K. C.-C. Towards reasoning in large language models: a survey. In *Findings of the Association for Computational Linguistics: ACL 2023* 1049–1065 (Association for Computational Linguistics, 2023).
29. Zitkovich, B. et al. RT-2: vision-language-action models transfer web knowledge to robotic control. In *Proc. 7th Conference on Robot Learning* 2165–2183 (PMLR, 2023).
30. Ma, X., Patidar, S., Haughton, I. & James, S. Hierarchical diffusion policy for kinematics-aware multi-task robotic manipulation. In *Proc. IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)* 18081–18090 (IEEE, 2024).
31. Zhang, C., Chen, J., Li, J., Peng, Y. & Mao, Z. Large language models for human-robot interaction: a review. *Biomimetic Intell. Robot.* **3**, 100131 (2023).
32. Lewis, P. et al. Retrieval-augmented generation for knowledge-intensive NLP tasks. In *Advances in Neural Information Processing Systems* 9459–9474 (Curran Associates, 2020).
33. Raiaan, M. et al. A review on large language models: architectures, applications, taxonomies, open issues and challenges. *IEEE Access* **12**, 26839–26874 (2024).
34. Rozo, L., Jimenez, P. & Torras, C. Force-based robot learning of pouring skills using parametric hidden Markov models. In *9th International Workshop on Robot Motion and Control* 227–232 (IEEE, 2013).
35. Huang, Y., Wilches, J. & Sun, Y. Robot gaining accurate pouring skills through self-supervised learning and generalization. *Robot. Auton. Syst.* **136**, 103692 (2021).

    [Article](https://doi.org/10.1016%2Fj.robot.2020.103692) 
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Robot%20gaining%20accurate%20pouring%20skills%20through%20self-supervised%20learning%20and%20generalization&journal=Robot.%20Auton.%20Syst.&doi=10.1016%2Fj.robot.2020.103692&volume=136&publication_year=2021&author=Huang%2CY&author=Wilches%2CJ&author=Sun%2CY)
36. Mon-Williams, R., Stouraitis, T. & Vijayakumar, S. A behavioural transformer for effective collaboration between a robot and a non-stationary human. In *2023 32nd IEEE International Conference on Robot and Human Interactive Communication (RO-MAN)* 1150–1157 (IEEE, 2023).
37. Belkhale, S., Cui, Y. & Sadigh, D. Data quality in imitation learning. In *Advances in Neural Information Processing Systems (NeurIPS)* 80375–80395 (Curran Associates, 2024).
38. Khazatsky, A. et al. DROID: a large-scale in-the-wild robot manipulation dataset. Robotics: Science and Systems; <https://www.roboticsproceedings.org/rss20/p120.pdf> (2024).
39. Acosta, B., Yang, W. & Posa, M. Validating robotics simulators on real-world impacts. *IEEE Robot. Autom. Lett.* **7**, 6471–6478 (2022).
40. Alomar, A. et al. CausalSim: a causal framework for unbiased trace-driven simulation. In *20th USENIX Symposium on Networked Systems Design and Implementation (NSDI 23)* 1115–1147 (USENIX Association, 2023).
41. Choi, H. et al. On the use of simulation in robotics: opportunities, challenges, and suggestions for moving forward. *Proc. Natl Acad. Sci. USA* **118**, e190785611 (2021).
42. Del Aguila Ferrandis, J., Moura, J. & Vijayakumar, S. Nonprehensile planar manipulation through reinforcement learning with multimodal categorical exploration. In *2023 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)* 5606–5613 (IEEE, 2023).
43. Kirk, R., Zhang, A., Grefenstette, E. & Rocktäschel, T. A survey of zero-shot generalisation in deep reinforcement learning. *J. Artific. Intell. Res.* **76**, 201–264 (2023).

    [Article](https://doi.org/10.1613%2Fjair.1.14174) 
    [MathSciNet](http://www.ams.org/mathscinet-getitem?mr=4546249) 
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20survey%20of%20zero-shot%20generalisation%20in%20deep%20reinforcement%20learning&journal=J.%20Artific.%20Intell.%20Res.&doi=10.1613%2Fjair.1.14174&volume=76&pages=201-264&publication_year=2023&author=Kirk%2CR&author=Zhang%2CA&author=Grefenstette%2CE&author=Rockt%C3%A4schel%2CT)
44. Dai, T. et al. Analysing deep reinforcement learning agents trained with domain randomisation. *Neurocomputing* **493**, 143–165 (2022).

    [Article](https://doi.org/10.1016%2Fj.neucom.2022.04.005) 
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Analysing%20deep%20reinforcement%20learning%20agents%20trained%20with%20domain%20randomisation&journal=Neurocomputing&doi=10.1016%2Fj.neucom.2022.04.005&volume=493&pages=143-165&publication_year=2022&author=Dai%2CT)
45. Chang, J., Uehara, M., Sreenivas, D., Kidambi, R. & Sun, W. Mitigating covariate shift in imitation learning via offline data with partial coverage. In *Advances in Neural Information Processing Systems* 965–979 (Curran Associates, 2021).
46. Huang, W. et al. Inner monologue: embodied reasoning through planning with language models. In *Proc. 6th Conference on Robot Learning* 1769–1782 (PMLR, 2023).
47. Nair, S., Rajeswaran, A., Kumar, V., Finn, C. & Gupta, A. R3M: a universal visual representation for robot manipulation. In *Proc. 6th Conference on Robot Learning* Vol. 205, 892–909 (PMLR, 2022).
48. Singh, I. et al. ProgPrompt: generating situated robot task plans using large language models. In *Proc. IEEE/CVF International Conference on Robotics and Automation (ICRA)* 11523–11530 (IEEE, 2023).
49. Song, C. H. et al. LLM-Planner: few-shot grounded planning for embodied agents with large language models. In *Proc. IEEE/CVF International Conference on Computer Vision (ICCV)* 2998–3009 (IEEE/CVF, 2023).
50. Vemprala, S. H., Bonatti, R., Bucker, A. & Kapoor, A. ChatGPT for robotics: design principles and model abilities. *IEEE Access* **12**, 55682–55696 (2024).

    [Article](https://doi.org/10.1109%2FACCESS.2024.3387941) 
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=ChatGPT%20for%20robotics%3A%20design%20principles%20and%20model%20abilities&journal=IEEE%20Access&doi=10.1109%2FACCESS.2024.3387941&volume=12&pages=55682-55696&publication_year=2024&author=Vemprala%2CSH&author=Bonatti%2CR&author=Bucker%2CA&author=Kapoor%2CA)
51. Ding, Y., Zhang, X., Paxton, C. & Zhang, S. Task and motion planning with large language models for object rearrangement. In *2023 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)* 2086–2092 (IEEE, 2023).
52. Kwon, M. et al. Toward grounded commonsense reasoning. In *Proc. International Conference on Robotics and Automation (ICRA)* 5463–5470 (IEEE, 2024).
53. Hong, J., Levine, S. & Dragan, A. Learning to influence human behavior with offline reinforcement learning. In *Advances in Neural Information Processing Systems (NeurIPS)* 36094–36105 (Curran Associates, 2024).
54. OpenAI. GPT-4 technical report. Preprint at <http://arxiv.org/abs/2303.08774> (2024).
55. OpenAI. Custom models program: fine-tuning GPT-4 for specific domains (2023); <https://platform.openai.com/docs/guides/fine-tuning/>
56. Pietsch, M. et al. Haystack: the end-to-end nlp framework for pragmatic builders. *GitHub* <https://github.com/deepset-ai/haystack> (2019).
57. Weaviate. Verba: the golden RAGtriever. *GitHub* <https://github.com/weaviate/Verba> (2023).
58. Kirillov, A. et al. Segment anything. In *Proc. IEEE/CVF International Conference on Computer Vision (ICCV)* 4015–4026 (IEEE, 2023).
59. Ramesh, A. et al. Zero-shot text-to-image generation. In *Proc. 38th International Conference on Machine Learning* 8821–8831 (PMLR, 2021).
60. Zeng, A. et al. Socratic models: composing zero-shot multimodal reasoning with language. In *Proc. International Conference on Learning Representations* (ICLR, 2023).
61. Cui, Y. et al. No, to the right: online language corrections for robotic manipulation via shared autonomy. In *Proc. 2023 ACM/IEEE International Conference on Human-Robot Interaction, HRI ’23* 93–101 (Association for Computing Machinery, 2023).
62. Bengio, Y. et al. Managing extreme AI risks amid rapid progress. *Science* **384**, 842–845 (2024).
63. Li, G., Jampani, V., Sun, D. & Sevilla-Lara, L. Locate: localize and transfer object parts for weakly supervised affordance grounding. In *Proc. IEEE/CVF Conference on Computer Vision and Pattern Recognition* 10922–10931 (IEEE, 2023).
64. Li, G., Sun, D., Sevilla-Lara, L. & Jampani, V. One-shot open affordance learning with foundation models. In *Proc. IEEE/CVF Conference on Computer Vision and Pattern Recognition* 3086–3096 (IEEE, 2024).
65. Liang, J. et al. Code as policies: language model programs for embodied control. In *2023 IEEE International Conference on Robotics and Automation (ICRA)* 9493–9500 (IEEE, 2023).
66. Hong, S. & Kim, H. An integrated GPU power and performance model. In *Proc. 37th Annual International Symposium on Computer Architecture* 280–289 (Association for Computing Machinery, 2010).
67. Kinova Robotics. Kinova Gen3 Ultra-Lightweight Robotic Arm User Guide (2023); <https://assets.iqr-robot.com/wp-content/uploads/2023/08/20230814163651088831.pdf>
68. US Environmental Protection Agency. GHG emission factors hub (2024); <https://www.epa.gov/climateleadership/ghg-emission-factors-hub>
69. Liu, S. et al. Grounding DINO: marrying DINO with grounded pre-training for open-set object detection. In *2024 European Conference on Computer Vision* (eds Leonardis, A. et al.) Vol. 15105 (Springer, 2023).
70. ruaridhmon. ruaridhmon/ELLMER: v1.0.0: Initial Release. *Zenodo* <https://doi.org/10.5281/zenodo.14483539> (2024).

[Download references](https://citation-needed.springer.com/v2/references/10.1038/s42256-025-01005-x?format=refman&flavour=references)

## Acknowledgements

This work was supported by the EPSRC CDT in RAS (EP/L016834/1). We thank S. Vijayakumar for his support and for providing access to resources; L. Martins and the Edinburgh Workshop for their assistance with hardware; and J. Wang, T. Stouraitis, J. Ferrandis and many others for their invaluable support and expertise.

## Author information

### Authors and Affiliations

1. University of Edinburgh, Edinburgh, UK

   Ruaridh Mon-Williams, Gen Li, Ran Long, Wenqian Du & Christopher G. Lucas
2. Massachusetts Institute of Technology, Boston, MA, USA

   Ruaridh Mon-Williams
3. Princeton University, Princeton, NJ, USA

   Ruaridh Mon-Williams
4. Alan Turing Institute, London, UK

   Wenqian Du

Authors

1. Ruaridh Mon-Williams

   [View author publications](/search?author=Ruaridh%20Mon-Williams)

   Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Ruaridh%20Mon-Williams) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Ruaridh%20Mon-Williams%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
2. Gen Li

   [View author publications](/search?author=Gen%20Li)

   Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Gen%20Li) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Gen%20Li%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
3. Ran Long

   [View author publications](/search?author=Ran%20Long)

   Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Ran%20Long) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Ran%20Long%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
4. Wenqian Du

   [View author publications](/search?author=Wenqian%20Du)

   Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Wenqian%20Du) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Wenqian%20Du%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)
5. Christopher G. Lucas

   [View author publications](/search?author=Christopher%20G.%20Lucas)

   Search author on:[PubMed](https://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=search&term=Christopher%20G.%20Lucas) [Google Scholar](https://scholar.google.co.uk/scholar?as_q=&num=10&btnG=Search+Scholar&as_epq=&as_oq=&as_eq=&as_occt=any&as_sauthors=%22Christopher%20G.%20Lucas%22&as_publication=&as_ylo=&as_yhi=&as_allsubj=all&hl=en)

### Contributions

Conceptualization: R.M.-W., G.L. and R.L. Methodology: R.M.-W., G.L., R.L., W.D. and C.G.L. Software: R.M.-W., G.L., R.L. and W.D. Formal analysis: R.M.-W. Investigation: R.M.-W. and W.D. Visualization: R.M.-W. Validation: R.M.-W. and W.D. Writing—original draft: R.M.-W. Writing—review and editing: R.M.-W., G.L., R.L. and C.G.L. Supervision: C.G.L.

### Corresponding authors

Correspondence to
[Ruaridh Mon-Williams](mailto:ruaridh.mw@ed.ac.uk) or [Gen Li](mailto:li.gen@ed.ac.uk).

## Ethics declarations

### Competing interests

The authors declare no competing interests.

## Peer review

### Peer review information

*Nature Machine Intelligence* thanks Matteo Saveriano and the other, anonymous, reviewer(s) for their contribution to the peer review of this work.

## Additional information

**Publisher’s note** Springer Nature remains neutral with regard to jurisdictional claims in published maps and institutional affiliations.

## Supplementary information

### [Supplementary Information](https://static-content.springer.com/esm/art%3A10.1038%2Fs42256-025-01005-x/MediaObjects/42256_2025_1005_MOESM1_ESM.pdf)

Supplementary Sections 1–3 and Table 1.

### [Supplementary Video 1](https://static-content.springer.com/esm/art%3A10.1038%2Fs42256-025-01005-x/MediaObjects/42256_2025_1005_MOESM2_ESM.mp4)

The video demonstrates a Kinova robot autonomously making coffee and decorating a plate using the ELLMER framework.

## Rights and permissions

**Open Access** This article is licensed under a Creative Commons Attribution 4.0 International License, which permits use, sharing, adaptation, distribution and reproduction in any medium or format, as long as you give appropriate credit to the original author(s) and the source, provide a link to the Creative Commons licence, and indicate if changes were made. The images or other third party material in this article are included in the article’s Creative Commons licence, unless indicated otherwise in a credit line to the material. If material is not included in the article’s Creative Commons licence and your intended use is not permitted by statutory regulation or exceeds the permitted use, you will need to obtain permission directly from the copyright holder. To view a copy of this licence, visit <http://creativecommons.org/licenses/by/4.0/>.

[Reprints and permissions](https://s100.copyright.com/AppDispatchServlet?title=Embodied%20large%20language%20models%20enable%20robots%20to%20complete%20complex%20tasks%20in%20unpredictable%20environments&author=Ruaridh%20Mon-Williams%20et%20al&contentID=10.1038%2Fs42256-025-01005-x&copyright=The%20Author%28s%29&publication=2522-5839&publicationDate=2025-03-19&publisherName=SpringerNature&orderBeanReset=true&oa=CC%20BY)

## About this article

[![Check for updates. Verify currency and authenticity via CrossMark](data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjgxIiB3aWR0aD0iNTciIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGcgZmlsbD0ibm9uZSIgZmlsbC1ydWxlPSJldmVub2RkIj48cGF0aCBkPSJtMTcuMzUgMzUuNDUgMjEuMy0xNC4ydi0xNy4wM2gtMjEuMyIgZmlsbD0iIzk4OTg5OCIvPjxwYXRoIGQ9Im0zOC42NSAzNS40NS0yMS4zLTE0LjJ2LTE3LjAzaDIxLjMiIGZpbGw9IiM3NDc0NzQiLz48cGF0aCBkPSJtMjggLjVjLTEyLjk4IDAtMjMuNSAxMC41Mi0yMy41IDIzLjVzMTAuNTIgMjMuNSAyMy41IDIzLjUgMjMuNS0xMC41MiAyMy41LTIzLjVjMC02LjIzLTIuNDgtMTIuMjEtNi44OC0xNi42Mi00LjQxLTQuNC0xMC4zOS02Ljg4LTE2LjYyLTYuODh6bTAgNDEuMjVjLTkuOCAwLTE3Ljc1LTcuOTUtMTcuNzUtMTcuNzVzNy45NS0xNy43NSAxNy43NS0xNy43NSAxNy43NSA3Ljk1IDE3Ljc1IDE3Ljc1YzAgNC43MS0xLjg3IDkuMjItNS4yIDEyLjU1cy03Ljg0IDUuMi0xMi41NSA1LjJ6IiBmaWxsPSIjNTM1MzUzIi8+PHBhdGggZD0ibTQxIDM2Yy01LjgxIDYuMjMtMTUuMjMgNy40NS0yMi40MyAyLjktNy4yMS00LjU1LTEwLjE2LTEzLjU3LTcuMDMtMjEuNWwtNC45Mi0zLjExYy00Ljk1IDEwLjctMS4xOSAyMy40MiA4Ljc4IDI5LjcxIDkuOTcgNi4zIDIzLjA3IDQuMjIgMzAuNi00Ljg2eiIgZmlsbD0iIzljOWM5YyIvPjxwYXRoIGQ9Im0uMiA1OC40NWMwLS43NS4xMS0xLjQyLjMzLTIuMDFzLjUyLTEuMDkuOTEtMS41Yy4zOC0uNDEuODMtLjczIDEuMzQtLjk0LjUxLS4yMiAxLjA2LS4zMiAxLjY1LS4zMi41NiAwIDEuMDYuMTEgMS41MS4zNS40NC4yMy44MS41IDEuMS44MWwtLjkxIDEuMDFjLS4yNC0uMjQtLjQ5LS40Mi0uNzUtLjU2LS4yNy0uMTMtLjU4LS4yLS45My0uMi0uMzkgMC0uNzMuMDgtMS4wNS4yMy0uMzEuMTYtLjU4LjM3LS44MS42Ni0uMjMuMjgtLjQxLjYzLS41MyAxLjA0LS4xMy40MS0uMTkuODgtLjE5IDEuMzkgMCAxLjA0LjIzIDEuODYuNjggMi40Ni40NS41OSAxLjA2Ljg4IDEuODQuODguNDEgMCAuNzctLjA3IDEuMDctLjIzcy41OS0uMzkuODUtLjY4bC45MSAxYy0uMzguNDMtLjguNzYtMS4yOC45OS0uNDcuMjItMSAuMzQtMS41OC4zNC0uNTkgMC0xLjEzLS4xLTEuNjQtLjMxLS41LS4yLS45NC0uNTEtMS4zMS0uOTEtLjM4LS40LS42Ny0uOS0uODgtMS40OC0uMjItLjU5LS4zMy0xLjI2LS4zMy0yLjAyem04LjQtNS4zM2gxLjYxdjIuNTRsLS4wNSAxLjMzYy4yOS0uMjcuNjEtLjUxLjk2LS43MnMuNzYtLjMxIDEuMjQtLjMxYy43MyAwIDEuMjcuMjMgMS42MS43MS4zMy40Ny41IDEuMTQuNSAyLjAydjQuMzFoLTEuNjF2LTQuMWMwLS41Ny0uMDgtLjk3LS4yNS0xLjIxLS4xNy0uMjMtLjQ1LS4zNS0uODMtLjM1LS4zIDAtLjU2LjA4LS43OS4yMi0uMjMuMTUtLjQ5LjM2LS43OC42NHY0LjhoLTEuNjF6bTcuMzcgNi40NWMwLS41Ni4wOS0xLjA2LjI2LTEuNTEuMTgtLjQ1LjQyLS44My43MS0xLjE0LjI5LS4zLjYzLS41NCAxLjAxLS43MS4zOS0uMTcuNzgtLjI1IDEuMTgtLjI1LjQ3IDAgLjg4LjA4IDEuMjMuMjQuMzYuMTYuNjUuMzguODkuNjdzLjQyLjYzLjU0IDEuMDNjLjEyLjQxLjE4Ljg0LjE4IDEuMzIgMCAuMzItLjAyLjU3LS4wNy43NmgtNC4zNmMuMDcuNjIuMjkgMS4xLjY1IDEuNDQuMzYuMzMuODIuNSAxLjM4LjUuMjkgMCAuNTctLjA0LjgzLS4xM3MuNTEtLjIxLjc2LS4zN2wuNTUgMS4wMWMtLjMzLjIxLS42OS4zOS0xLjA5LjUzLS40MS4xNC0uODMuMjEtMS4yNi4yMS0uNDggMC0uOTItLjA4LTEuMzQtLjI1LS40MS0uMTYtLjc2LS40LTEuMDctLjctLjMxLS4zMS0uNTUtLjY5LS43Mi0xLjEzLS4xOC0uNDQtLjI2LS45NS0uMjYtMS41MnptNC42LS42MmMwLS41NS0uMTEtLjk4LS4zNC0xLjI4LS4yMy0uMzEtLjU4LS40Ny0xLjA2LS40Ny0uNDEgMC0uNzcuMTUtMS4wNy40NS0uMzEuMjktLjUuNzMtLjU4IDEuM3ptMi41LjYyYzAtLjU3LjA5LTEuMDguMjgtMS41My4xOC0uNDQuNDMtLjgyLjc1LTEuMTNzLjY5LS41NCAxLjEtLjcxYy40Mi0uMTYuODUtLjI0IDEuMzEtLjI0LjQ1IDAgLjg0LjA4IDEuMTcuMjNzLjYxLjM0Ljg1LjU3bC0uNzcgMS4wMmMtLjE5LS4xNi0uMzgtLjI4LS41Ni0uMzctLjE5LS4wOS0uMzktLjE0LS42MS0uMTQtLjU2IDAtMS4wMS4yMS0xLjM1LjYzLS4zNS40MS0uNTIuOTctLjUyIDEuNjcgMCAuNjkuMTcgMS4yNC41MSAxLjY2LjM0LjQxLjc4LjYyIDEuMzIuNjIuMjggMCAuNTQtLjA2Ljc4LS4xNy4yNC0uMTIuNDUtLjI2LjY0LS40MmwuNjcgMS4wM2MtLjMzLjI5LS42OS41MS0xLjA4LjY1LS4zOS4xNS0uNzguMjMtMS4xOC4yMy0uNDYgMC0uOS0uMDgtMS4zMS0uMjQtLjQtLjE2LS43NS0uMzktMS4wNS0uN3MtLjUzLS42OS0uNy0xLjEzYy0uMTctLjQ1LS4yNS0uOTYtLjI1LTEuNTN6bTYuOTEtNi40NWgxLjU4djYuMTdoLjA1bDIuNTQtMy4xNmgxLjc3bC0yLjM1IDIuOCAyLjU5IDQuMDdoLTEuNzVsLTEuNzctMi45OC0xLjA4IDEuMjN2MS43NWgtMS41OHptMTMuNjkgMS4yN2MtLjI1LS4xMS0uNS0uMTctLjc1LS4xNy0uNTggMC0uODcuMzktLjg3IDEuMTZ2Ljc1aDEuMzR2MS4yN2gtMS4zNHY1LjZoLTEuNjF2LTUuNmgtLjkydi0xLjJsLjkyLS4wN3YtLjcyYzAtLjM1LjA0LS42OC4xMy0uOTguMDgtLjMxLjIxLS41Ny40LS43OXMuNDItLjM5LjcxLS41MWMuMjgtLjEyLjYzLS4xOCAxLjA0LS4xOC4yNCAwIC40OC4wMi42OS4wNy4yMi4wNS40MS4xLjU3LjE3em0uNDggNS4xOGMwLS41Ny4wOS0xLjA4LjI3LTEuNTMuMTctLjQ0LjQxLS44Mi43Mi0xLjEzLjMtLjMxLjY1LS41NCAxLjA0LS43MS4zOS0uMTYuOC0uMjQgMS4yMy0uMjRzLjg0LjA4IDEuMjQuMjRjLjQuMTcuNzQuNCAxLjA0Ljcxcy41NC42OS43MiAxLjEzYy4xOS40NS4yOC45Ni4yOCAxLjUzcy0uMDkgMS4wOC0uMjggMS41M2MtLjE4LjQ0LS40Mi44Mi0uNzIgMS4xM3MtLjY0LjU0LTEuMDQuNy0uODEuMjQtMS4yNC4yNC0uODQtLjA4LTEuMjMtLjI0LS43NC0uMzktMS4wNC0uN2MtLjMxLS4zMS0uNTUtLjY5LS43Mi0xLjEzLS4xOC0uNDUtLjI3LS45Ni0uMjctMS41M3ptMS42NSAwYzAgLjY5LjE0IDEuMjQuNDMgMS42Ni4yOC40MS42OC42MiAxLjE4LjYyLjUxIDAgLjktLjIxIDEuMTktLjYyLjI5LS40Mi40NC0uOTcuNDQtMS42NiAwLS43LS4xNS0xLjI2LS40NC0xLjY3LS4yOS0uNDItLjY4LS42My0xLjE5LS42My0uNSAwLS45LjIxLTEuMTguNjMtLjI5LjQxLS40My45Ny0uNDMgMS42N3ptNi40OC0zLjQ0aDEuMzNsLjEyIDEuMjFoLjA1Yy4yNC0uNDQuNTQtLjc5Ljg4LTEuMDIuMzUtLjI0LjctLjM2IDEuMDctLjM2LjMyIDAgLjU5LjA1Ljc4LjE0bC0uMjggMS40LS4zMy0uMDljLS4xMS0uMDEtLjIzLS4wMi0uMzgtLjAyLS4yNyAwLS41Ni4xLS44Ni4zMXMtLjU1LjU4LS43NyAxLjF2NC4yaC0xLjYxem0tNDcuODcgMTVoMS42MXY0LjFjMCAuNTcuMDguOTcuMjUgMS4yLjE3LjI0LjQ0LjM1LjgxLjM1LjMgMCAuNTctLjA3LjgtLjIyLjIyLS4xNS40Ny0uMzkuNzMtLjczdi00LjdoMS42MXY2Ljg3aC0xLjMybC0uMTItMS4wMWgtLjA0Yy0uMy4zNi0uNjMuNjQtLjk4Ljg2LS4zNS4yMS0uNzYuMzItMS4yNC4zMi0uNzMgMC0xLjI3LS4yNC0xLjYxLS43MS0uMzMtLjQ3LS41LTEuMTQtLjUtMi4wMnptOS40NiA3LjQzdjIuMTZoLTEuNjF2LTkuNTloMS4zM2wuMTIuNzJoLjA1Yy4yOS0uMjQuNjEtLjQ1Ljk3LS42My4zNS0uMTcuNzItLjI2IDEuMS0uMjYuNDMgMCAuODEuMDggMS4xNS4yNC4zMy4xNy42MS40Ljg0LjcxLjI0LjMxLjQxLjY4LjUzIDEuMTEuMTMuNDIuMTkuOTEuMTkgMS40NCAwIC41OS0uMDkgMS4xMS0uMjUgMS41Ny0uMTYuNDctLjM4Ljg1LS42NSAxLjE2LS4yNy4zMi0uNTguNTYtLjk0LjczLS4zNS4xNi0uNzIuMjUtMS4xLjI1LS4zIDAtLjYtLjA3LS45LS4ycy0uNTktLjMxLS44Ny0uNTZ6bTAtMi4zYy4yNi4yMi41LjM3LjczLjQ1LjI0LjA5LjQ2LjEzLjY2LjEzLjQ2IDAgLjg0LS4yIDEuMTUtLjYuMzEtLjM5LjQ2LS45OC40Ni0xLjc3IDAtLjY5LS4xMi0xLjIyLS4zNS0xLjYxLS4yMy0uMzgtLjYxLS41Ny0xLjEzLS41Ny0uNDkgMC0uOTkuMjYtMS41Mi43N3ptNS44Ny0xLjY5YzAtLjU2LjA4LTEuMDYuMjUtMS41MS4xNi0uNDUuMzctLjgzLjY1LTEuMTQuMjctLjMuNTgtLjU0LjkzLS43MXMuNzEtLjI1IDEuMDgtLjI1Yy4zOSAwIC43My4wNyAxIC4yLjI3LjE0LjU0LjMyLjgxLjU1bC0uMDYtMS4xdi0yLjQ5aDEuNjF2OS44OGgtMS4zM2wtLjExLS43NGgtLjA2Yy0uMjUuMjUtLjU0LjQ2LS44OC42NC0uMzMuMTgtLjY5LjI3LTEuMDYuMjctLjg3IDAtMS41Ni0uMzItMi4wNy0uOTVzLS43Ni0xLjUxLS43Ni0yLjY1em0xLjY3LS4wMWMwIC43NC4xMyAxLjMxLjQgMS43LjI2LjM4LjY1LjU4IDEuMTUuNTguNTEgMCAuOTktLjI2IDEuNDQtLjc3di0zLjIxYy0uMjQtLjIxLS40OC0uMzYtLjctLjQ1LS4yMy0uMDgtLjQ2LS4xMi0uNy0uMTItLjQ1IDAtLjgyLjE5LTEuMTMuNTktLjMxLjM5LS40Ni45NS0uNDYgMS42OHptNi4zNSAxLjU5YzAtLjczLjMyLTEuMy45Ny0xLjcxLjY0LS40IDEuNjctLjY4IDMuMDgtLjg0IDAtLjE3LS4wMi0uMzQtLjA3LS41MS0uMDUtLjE2LS4xMi0uMy0uMjItLjQzcy0uMjItLjIyLS4zOC0uM2MtLjE1LS4wNi0uMzQtLjEtLjU4LS4xLS4zNCAwLS42OC4wNy0xIC4ycy0uNjMuMjktLjkzLjQ3bC0uNTktMS4wOGMuMzktLjI0LjgxLS40NSAxLjI4LS42My40Ny0uMTcuOTktLjI2IDEuNTQtLjI2Ljg2IDAgMS41MS4yNSAxLjkzLjc2cy42MyAxLjI1LjYzIDIuMjF2NC4wN2gtMS4zMmwtLjEyLS43NmgtLjA1Yy0uMy4yNy0uNjMuNDgtLjk4LjY2cy0uNzMuMjctMS4xNC4yN2MtLjYxIDAtMS4xLS4xOS0xLjQ4LS41Ni0uMzgtLjM2LS41Ny0uODUtLjU3LTEuNDZ6bTEuNTctLjEyYzAgLjMuMDkuNTMuMjcuNjcuMTkuMTQuNDIuMjEuNzEuMjEuMjggMCAuNTQtLjA3Ljc3LS4ycy40OC0uMzEuNzMtLjU2di0xLjU0Yy0uNDcuMDYtLjg2LjEzLTEuMTguMjMtLjMxLjA5LS41Ny4xOS0uNzYuMzFzLS4zMy4yNS0uNDEuNGMtLjA5LjE1LS4xMy4zMS0uMTMuNDh6bTYuMjktMy42M2gtLjk4di0xLjJsMS4wNi0uMDcuMi0xLjg4aDEuMzR2MS44OGgxLjc1djEuMjdoLTEuNzV2My4yOGMwIC44LjMyIDEuMi45NyAxLjIuMTIgMCAuMjQtLjAxLjM3LS4wNC4xMi0uMDMuMjQtLjA3LjM0LS4xMWwuMjggMS4xOWMtLjE5LjA2LS40LjEyLS42NC4xNy0uMjMuMDUtLjQ5LjA4LS43Ni4wOC0uNCAwLS43NC0uMDYtMS4wMi0uMTgtLjI3LS4xMy0uNDktLjMtLjY3LS41Mi0uMTctLjIxLS4zLS40OC0uMzctLjc4LS4wOC0uMy0uMTItLjY0LS4xMi0xLjAxem00LjM2IDIuMTdjMC0uNTYuMDktMS4wNi4yNy0xLjUxcy40MS0uODMuNzEtMS4xNGMuMjktLjMuNjMtLjU0IDEuMDEtLjcxLjM5LS4xNy43OC0uMjUgMS4xOC0uMjUuNDcgMCAuODguMDggMS4yMy4yNC4zNi4xNi42NS4zOC44OS42N3MuNDIuNjMuNTQgMS4wM2MuMTIuNDEuMTguODQuMTggMS4zMiAwIC4zMi0uMDIuNTctLjA3Ljc2aC00LjM3Yy4wOC42Mi4yOSAxLjEuNjUgMS40NC4zNi4zMy44Mi41IDEuMzguNS4zIDAgLjU4LS4wNC44NC0uMTMuMjUtLjA5LjUxLS4yMS43Ni0uMzdsLjU0IDEuMDFjLS4zMi4yMS0uNjkuMzktMS4wOS41M3MtLjgyLjIxLTEuMjYuMjFjLS40NyAwLS45Mi0uMDgtMS4zMy0uMjUtLjQxLS4xNi0uNzctLjQtMS4wOC0uNy0uMy0uMzEtLjU0LS42OS0uNzItMS4xMy0uMTctLjQ0LS4yNi0uOTUtLjI2LTEuNTJ6bTQuNjEtLjYyYzAtLjU1LS4xMS0uOTgtLjM0LTEuMjgtLjIzLS4zMS0uNTgtLjQ3LTEuMDYtLjQ3LS40MSAwLS43Ny4xNS0xLjA4LjQ1LS4zMS4yOS0uNS43My0uNTcgMS4zem0zLjAxIDIuMjNjLjMxLjI0LjYxLjQzLjkyLjU3LjMuMTMuNjMuMi45OC4yLjM4IDAgLjY1LS4wOC44My0uMjNzLjI3LS4zNS4yNy0uNmMwLS4xNC0uMDUtLjI2LS4xMy0uMzctLjA4LS4xLS4yLS4yLS4zNC0uMjgtLjE0LS4wOS0uMjktLjE2LS40Ny0uMjNsLS41My0uMjJjLS4yMy0uMDktLjQ2LS4xOC0uNjktLjMtLjIzLS4xMS0uNDQtLjI0LS42Mi0uNHMtLjMzLS4zNS0uNDUtLjU1Yy0uMTItLjIxLS4xOC0uNDYtLjE4LS43NSAwLS42MS4yMy0xLjEuNjgtMS40OS40NC0uMzggMS4wNi0uNTcgMS44My0uNTcuNDggMCAuOTEuMDggMS4yOS4yNXMuNzEuMzYuOTkuNTdsLS43NC45OGMtLjI0LS4xNy0uNDktLjMyLS43My0uNDItLjI1LS4xMS0uNTEtLjE2LS43OC0uMTYtLjM1IDAtLjYuMDctLjc2LjIxLS4xNy4xNS0uMjUuMzMtLjI1LjU0IDAgLjE0LjA0LjI2LjEyLjM2cy4xOC4xOC4zMS4yNmMuMTQuMDcuMjkuMTQuNDYuMjFsLjU0LjE5Yy4yMy4wOS40Ny4xOC43LjI5cy40NC4yNC42NC40Yy4xOS4xNi4zNC4zNS40Ni41OC4xMS4yMy4xNy41LjE3LjgyIDAgLjMtLjA2LjU4LS4xNy44My0uMTIuMjYtLjI5LjQ4LS41MS42OC0uMjMuMTktLjUxLjM0LS44NC40NS0uMzQuMTEtLjcyLjE3LTEuMTUuMTctLjQ4IDAtLjk1LS4wOS0xLjQxLS4yNy0uNDYtLjE5LS44Ni0uNDEtMS4yLS42OHoiIGZpbGw9IiM1MzUzNTMiLz48L2c+PC9zdmc+)](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/a72dadc1f02c0012feb1e30b9ca10526.jpg)

### Cite this article

Mon-Williams, R., Li, G., Long, R. *et al.* Embodied large language models enable robots to complete complex tasks in unpredictable environments.
*Nat Mach Intell* **7**, 592–601 (2025). https://doi.org/10.1038/s42256-025-01005-x

[Download citation](https://citation-needed.springer.com/v2/references/10.1038/s42256-025-01005-x?format=refman&flavour=citation)

* Received: 22 June 2024
* Accepted: 31 January 2025
* Published: 19 March 2025
* Version of record: 19 March 2025
* Issue date: April 2025
* DOI: https://doi.org/10.1038/s42256-025-01005-x

### Share this article

Anyone you share the following link with will be able to read this content:

Get shareable link

Sorry, a shareable link is not currently available for this article.

Copy shareable link to clipboard

Provided by the Springer Nature SharedIt content-sharing initiative

## This article is cited by

* ### [MechRAG: a multimodal large language model for mechanical engineering](https://doi.org/10.1038/s44172-025-00517-z)

  + Shuang Li
  + Jonathan Corney

  *Communications Engineering* (2025)
* ### [Generative artificial intelligence in manufacturing: applications, case studies, and future directions for next-generation intelligent production systems](https://doi.org/10.1007/s00170-025-16667-5)

  + Mohammad Shahin
  + Ali Hosseinzadeh
  + F. Frank Chen

  *The International Journal of Advanced Manufacturing Technology* (2025)

---

*爬取时间: 2025-11-28 21:55:54*
