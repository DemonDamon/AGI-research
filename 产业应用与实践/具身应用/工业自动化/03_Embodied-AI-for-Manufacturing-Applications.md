# Embodied AI for Manufacturing Applications

**来源**: [https://graymatter-robotics.com/embodied-ai-for-manufacturing-applications/](https://graymatter-robotics.com/embodied-ai-for-manufacturing-applications/)

---

# Embodied AI for Manufacturing Applications - GrayMatter Robotics

原文链接: https://graymatter-robotics.com/embodied-ai-for-manufacturing-applications/

![](data:image/svg+xml;base64,PHN2ZyB4bWxucz0naHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmcnIHZpZXdCb3g9JzAgMCAyNTYwIDE0NDAnPjwvc3ZnPg==)

**Embodied AI vs Digital AI**

Most of the AI that we experience in our daily lives is digital AI. It produces digital artifacts, decision recommendations, or predictions that will either be used by a human or some other digital agent. Examples include generating a cover letter for a job application using ChatGPT, recommendations for watching a movie on NetFlix, creating a painting using Dall.E, getting a fraud notification in a credit card transaction, and detecting a tumor in a medical image.

A different kind of AI is being developed to manage the behavior of physical systems. For example, a driverless car, an underwater exploration vehicle, or a robot performing welding need AI to operate autonomously. This AI is called embodied AI. It is tasked with one or more goals and it uses the sensor data to produce a sequence of actions that the physical system executes to achieve the goal. For example, a robotic cell can be tasked with sanding the top surface of a part placed in the cell with the desired surface finish. The embodied AI monitors the cell state using sensors and generates instructions for the robot to perform the task. Digital AI and embodied AI share some similarities and utilize many underlying techniques. However, understanding the differences between these two types of AI is critical to successfully adapting digital AI approaches for use in the context of embodied AI applications.

**Considering Risk in the Context of Embodied AI**

We will focus on manufacturing automation applications in this article. Robotics applications in the context of manufacturing are different from many other types of robotics applications. In manufacturing applications, the work environment can be controlled to some extent and reasonably good models are available to inform the decision making process. On the other hand, the process quality expectations are very high and operation execution needs to be time optimal in manufacturing. Errors are very expensive and therefore the manufacturing community tends to be risk averse.

The risk profile of embodied AI in manufacturing applications is fundamentally different from that of digital AI applications. If the accuracy of a digital AI tool is 99%, then it can tremendously boost human productivity in many applications. For example, if you are using AI to generate a 1000-word cover letter that only requires you to manually edit 10 of those words, then you will be saving a lot of time compared to writing that letter from scratch. And for the case of a recommendation engine, you wouldn’t mind if it gave you a poor suggestion for a movie once every couple of months.

Comparatively, accuracy requirements for the embodied AI system in manufacturing are often very different due to risk considerations. For example, if a robot has a success rate of 99% on processing steps and it works on a part that requires 200 steps, then every part made by the robot will contain two errors. As a result, the part would get scrapped or would require repairs. In most manufacturing applications, a technology that does not exhibit extremely high process quality will not be considered viable.

Risk consists of two aspects: (1) probability of making an error and (2) the consequence of making errors. When the consequence of making an error is not significant, then a much higher probability of error can be tolerated. That is why an error probability of 1% will be acceptable in many digital AI applications. Conversely, many embodied AI applications demand errors probabilities better than one in a million. Reducing error probability using a purely data-driven approach requires using enormous amounts of data. In most cases, the need for data grows exponentially. Unfortunately, acquiring data from physical systems is expensive. Therefore, a different approach needs to be followed when dealing with embodied AI applications.

**Architecting Embodied AI System**

In digital AI, we see great success by deploying large end-to-end learning models (e.g., LLMs). These models thrive on the vast amount of data. However, they are unable to meet many characteristics mentioned above regarding embodied AI.

Embodied AI and the physical system controlled by it need to be co-designed to ensure that the embodied AI is aware of the physical system capabilities and limitations to deliver the best possible performance at the system level. For example, if a robotic cell has an infrared thermal camera and force sensor, then AI managing the cell should include perception modules that can make use of this sensor data. When a new failure mode associated with embodied AI is discovered, users expect that this failure mode can be prevented in the future by rapidly updating the system. Moreover, the system should include safeguards to ensure that risks created by failures can be mitigated to the maximum extent possible and the system can recover quickly.

Embodied AI should be viewed as a complex system that involves interactions among multiple AI components. The following principles should be used to design the architecture of the embodied AI system for manufacturing applications:

* *Select the right functional decomposition to achieve the best trade off between modularity and performance*: The system should use the right functional decomposition to ensure that it is able to achieve the desired trade off in performance and modularity. This ensures the ease of upgrades and enables rapid generation of a new AI system to match a new hardware configuration.
* *Select the right AI approach for each functional block*: Many different AI approaches exist (e.g., deep learning, reinforcement learning, transformers, diffusion, graph neural networks, active learning). Each approach has its pros and cons. It is unlikely that a single approach will suffice to deliver the desired performance. Therefore, each functional block should use the right AI approach by carefully considering pros and cons.
* *Exploit known models*: We should use AI approaches that can exploit the known models and use a data-driven approach to augment the known models and existing knowledge based on experimental data to fill the missing model gaps.
* *Develop clear and easy to understand specifications for interfaces between functional components*: Ensuring ease of the failure diagnosis and enabling explainability requires us to use clear and easy to understand specifications for interfaces.
* *Select the right V&V methodology for each functional block*: Each functional block needs to be verified and validated after initial training and every system update or adaptation. We need the right V&V technology to accomplish updates with minimal disruption to the system.
* *Compose from Pre-trained Modular Components*: Physical systems can have a wide variety of configurations to support their intended requirements. For example, manufacturing robotic cells can come in many different configurations based on the size of the part being processed and the process being performed (e.g., sanding or blasting). Different cells may include robots with different capabilities (mobile platform mounted robot vs. gantry mounted robot), different types of sensors (depth camera vs thermal camera), and different tools (orbital sanders vs blasting nozzle) . Therefore developing universal embodied AI that works for all manufacturing applications out of the box is not likely to perform well. The AI for the system needs to be quickly synthesized from the modular components to match the sensing and actuation capabilities of the system and the work environment.
* *Integrate an AI-Powered Digital Twin Component*: The overall system needs a digital twin to evaluate alternative sequences of actions and select the right action sequence. The digital twin cannot use traditional simulations, as these tend to be slow. The digital twin needs to be powered by AI to ensure that it can support evaluations of a large number of options.
* *Incorporate a Built-in AI-powered PHM Component*: Every physical system is likely to exhibit failures due to physical component malfunction or changes in the working conditions. It becomes necessary to monitor the action execution in the physical world and issue alerts using a prognostics and health management (PHM) component. Therefore, embodied AI needs to include a built-in AI-powered PHM component.
* *Distributed Architecture to Enable Partitioning of Computation between Edge and Cloud*: It is not possible to perform all AI computation in the cloud in the context of embodied AI. The system should be designed to ensure that computation that is sensitive to network latency can be performed on the edge. The use of edge computing may also be needed to support applications where sensor data cannot be transmitted to clouds due to privacy/security reasons.

**Conclusions**

Embodied AI for manufacturing applications cannot be realized as a monolithic system running on the cloud. The right level of modularity is necessary to meet the requirements related to ease-of-upgrade, customizability, explainability, and performance. Heterogeneity in component level technologies becomes necessary to exploit the recent advances in AI and meet the demanding requirements of manufacturing applications. The focus should be on the system level performance optimization and not on optimizing individual component performance. Humans are important parts of manufacturing operations and therefore human-system integration issues need to be proactively addressed during the system design. Therefore, having the right system architecture in the embodied AI system is the key to success in manufacturing applications. This requires paying close attention to the requirements of applications and developing AI components that can be easily configured and validated.

[Why Embodied AI For Manufacturing Applications Is Different From Digital AI](https://www.forbes.com/councils/forbestechcouncil/2024/08/26/why-embodied-ai-for-manufacturing-applications-is-different-from-digital-ai/)

Search

#### Table of Contents

##### Categories

* [Automation](https://graymatter-robotics.com/category/automation/) (20)
* [GMR-AI](https://graymatter-robotics.com/category/gmr-ai/) (7)
* [High-Mix Manufacturing](https://graymatter-robotics.com/category/high-mix-manufacturing/) (6)
* [Labor Shortage](https://graymatter-robotics.com/category/labor-shortage/) (7)
* [Manufacturing](https://graymatter-robotics.com/category/manufacturing/) (21)
* [Physics-Informed AI](https://graymatter-robotics.com/category/physics-informed-ai/) (6)
* [Prognostics And Health Management (PHM)](https://graymatter-robotics.com/category/prognostics-and-health-management-phm/) (2)
* [RaaS](https://graymatter-robotics.com/category/raas/) (3)
* [Robotics](https://graymatter-robotics.com/category/robotics/) (5)
* [Smart Robotic Cells](https://graymatter-robotics.com/category/smart-robotic-cells/) (6)

##### Recent Posts

* [GrayMatter Robotics Named Winner in U.S. Navy’s Advanced Manufacturing Innovation for Maritime Readiness Challenge](https://graymatter-robotics.com/graymatter-robotics-named-winner-in-us-navys-advanced-manufacturing-innovation-for-maritime-readiness-challenge/)
* [Navigating the Future: AI Robotics in Specialty Vehicle Manufacturing](https://graymatter-robotics.com/navigating-the-future-ai-robotics-in-specialty-vehicle-manufacturing/)
* [AI Robotics in Aviation MRO: Transforming Aircraft Maintenance While Meeting Compliance Standards](https://graymatter-robotics.com/ai-robotics-in-aviation-mro-transforming-aircraft-maintenance-while-meeting-compliance-standards/)
* [The Future of Manufacturing: Trends in Industrial Robotics](https://graymatter-robotics.com/the-future-of-manufacturing-trends-in-industrial-robotics/)
* [Driving Innovation in Manufacturing: GrayMatter Robotics Earns Spot on Fast Company’s Most Innovative Companies List](https://graymatter-robotics.com/graymatter-robotics-fast-company-innovative-companies-2025/)

##### Tags

[Aerospace](https://graymatter-robotics.com/tag/aerospace/) [AI](https://graymatter-robotics.com/tag/ai/) [Aircraft](https://graymatter-robotics.com/tag/aircraft/) [Airplane](https://graymatter-robotics.com/tag/airplane/) [Automaton](https://graymatter-robotics.com/tag/automaton/) [Aviation](https://graymatter-robotics.com/tag/aviation/) [Aviation MRO](https://graymatter-robotics.com/tag/aviation-mro/) [Fast Company](https://graymatter-robotics.com/tag/fast-company/) [MRO](https://graymatter-robotics.com/tag/mro/) [Planes](https://graymatter-robotics.com/tag/planes/)

---

*爬取时间: 2025-11-28 21:55:59*
