# Gemini 2.5 for robotics and embodied intelligence

**来源**: [https://developers.googleblog.com/en/gemini-25-for-robotics-and-embodied-intelligence/](https://developers.googleblog.com/en/gemini-25-for-robotics-and-embodied-intelligence/)

---

# 
            
            Gemini 2.5 for robotics and embodied intelligence
            
            
            - Google Developers Blog
            
        

原文链接: https://developers.googleblog.com/en/gemini-25-for-robotics-and-embodied-intelligence/

[![Google for Developers](https://storage.googleapis.com/gweb-developer-goog-blog-cms-assets/site/20251118-195321/images/g-dev.svg)](https://developers.google.com/)

Search

[Gemini](/en/search/?product_categories=Gemini) / [Google AI Studio](/en/search/?product_categories=Google+AI+Studio)

# Gemini 2.5 for robotics and embodied intelligence

JUNE 24, 2025

[Laura Graesser](/en/search/?author=Laura+Graesser)
Staff Research Scientist

[Fei Xia](/en/search/?author=Fei+Xia)
Staff Research Scientist

Share

* [Facebook](https://www.facebook.com/sharer/sharer.php?u={url} "Share on Facebook")
* [Twitter](https://twitter.com/intent/tweet?text={url} "Share on Twitter")
* [LinkedIn](https://www.linkedin.com/shareArticle?url={url}&mini=true "Share on LinkedIn")
* [Mail](mailto:name@example.com?subject=Check%20out%20this%20site&body=Check%20out%20{url} "Send via Email")

The latest generation of Gemini models, [2.5 Pro and Flash](https://blog.google/products/gemini/gemini-2-5-model-family-expands/), are unlocking new frontiers in robotics. Their advanced coding, reasoning, and multimodal capabilities, now combined with spatial understanding, provide the foundation for the next generation of interactive and intelligent robots.

This post explores how developers can leverage [Gemini 2.5](https://developers.googleblog.com/en/search/?query=Gemini+2.5) to build sophisticated robotics applications. We'll provide practical examples with prompts to show using Gemini 2.5 and the Live API for:

* Semantic scene understanding for complex queries: Identify and label objects from robot camera feeds. Understand complex queries through multimodal reasoning.

* Combine spatial reasoning with code generation to control robots: Use the robot's API to call functions and bring task plans to life.

* Build interactive robotics applications with the [Live API](https://ai.google.dev/gemini-api/docs/live): Convert voice commands into executable robot plans.

In March, we launched our [Gemini Robotics](https://deepmind.google/models/gemini-robotics/) models, including [Gemini Robotics-ER](https://deepmind.google/models/gemini-robotics/gemini-robotics-er/), our advanced embodied reasoning model optimized for the unique demands of robotics applications. We’re also excited to share how our [Gemini Robotics](https://deepmind.google/models/gemini-robotics/) trusted testers are already demonstrating the power of Gemini in robotics applications. We are including examples from Agile Robots, Agility Robotics, Boston Dynamics, and Enchanted Tools. [Join the Gemini Robotics-ER trusted tester program waitlist](https://docs.google.com/forms/d/1sM5GqcVMWv-KmKY3TOMpVtQ-lDFeAftQ-d9xQn92jCE/edit?ts=67cef986).

## Semantic scene understanding for complex queries

Reasoning about the physical world is at the core of general and robust control. Gemini 2.5 represents a step in this direction with its improved ability to reason multimodally. Below we share two examples, utilizing Gemini’s pointing and object detection capabilities.

**Pointing** allows a model to refer to entities or parts of entities precisely, and locate them in space. Gemini 2.5 Pro is able to reason about the entities it is pointing to, opening new opportunities for interacting with images. For example, Gemini 2.5 Pro is able to reason about empty space in the context of a supermarket display, knowing that this indicates restocking may be needed. In the example below, Gemini identifies the baby eggplant needs restocking. Gemini 2.5 Pro also shows a nascent ability to locate and read information from that location, as illustrated in the gauge example.

**Example 1:** Gemini 2.5 can locate objects in the scene based on fine-grained language descriptions, for example, find a shelf that needs restocking.

**Prompt:** *Point to one bin on the shelf that needs restocking. The answer should follow the json format: [{"point": <point>, "label": <label1>}, ...]. The points are in [y, x] format normalized to 0-1000.*

**Input image with response overlay:**

![Gemini 2.5 can locate objects in the scene based on fine-grained language descriptions, for example, find a shelf that needs restocking.](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/fe7c913329249aaba6c6336c78ae1bc5.png)

**Example 2:** Gemini 2.5 can locate small objects in the scene and estimate states of those objects. For example, it can read gauges.

**Prompt:** *Point to all the round gauges. The answer should follow the json format: [{"point": <point>, "label": <label1>}, ...]. The points are in [y, x] format normalized to 0-1000.*

**Input image with response overlay:**

![Gemini 2.5 can locate small objects in the scene and estimate states of those objects. For example, it can read gauges.](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/571cd80f6ffdd449e4a5506a12750192.png)

**Prompt:** *What is the reading on the middle gauge?*

**Response:** Based on the close-up view, the round gauge in the center-left of the image appears to be reading 0. The needle is pointing directly at the "0" mark on the dial.

### **Going beyond object-centric perception**

Gemini 2.5 is able to accurately track multiple objects across time and detect open ended concepts like ‘a spill’. Gemini 2.5 can be prompted into trajectory prediction in the form of a sequence of points.

**Example 1:** Gemini 2.5 can generate bounding boxes for each frame in a video and be visualized like below.

**Prompt:** *Detect green bowl, crab, wallet, pink bowl, phone, return a json array with keys box\_2d and label. (executed per frame).*

**Input image with response overlay:**

[![


Sorry, your browser doesn't support playback for this video

](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/wagtailvideo-hdmsnor7_thumb.jpg)](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/per_frame_det_final.mp4)

**Example 2:** Gemini 2.5 can detect open-ended concepts relevant to robotics, requiring commonsense knowledge and context specific reasoning. For example, a helpful robot needs to understand the concept of a “spill”.

**Prompt:**

*1) Show me the bounding box of spill. Return in a json array with keys box\_2d and label.*

*2) Give the segmentation masks for the spill. Output a JSON list of segmentation masks where each entry contains the 2D bounding box in the key "box\_2d", the segmentation mask in key "mask", and the text label in the key "label".*

**Input image with response overlay:**

![Gemini 2.5 can detect open-ended concepts relevant to robotics, requiring commonsense knowledge and context specific reasoning. For example, a helpful robot needs to understand the concept of a “spill”.](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/fe19e827de113bd2597a6bd4c868e556.png)

**Example 3:** Gemini 2.5 can be prompted into trajectory prediction in the form of a sequence of points.

**Prompt:** *Generate a robot arm trajectory of 10 points to move the cloth to the spill. The answer should follow the json format: [{"point": <point>, "label": <label1>}, ...]. The points are in [y, x] format normalized to 0-1000.*

**Input image with response overlay:**

![Gemini 2.5 can be prompted into trajectory prediction in the form of a sequence of points.](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/56bed699014fb59397746579ad72bdd4.png)

## Using spatial understanding and code generation to control robots

Gemini 2.5 can utilize its underlying spatial understanding to control robots through code generation. By providing Gemini 2.5 with a robot control API, it can apply advanced capabilities in scene understanding, object manipulation, and code writing together to perform tasks zero-shot, with no additional training.

Example 1 below showcases code-generation for “Put the banana in the bowl”. It gives Gemini access to a robot control API and shows how the model leverages its spatial understanding, thinking, and code generation capabilities to select the appropriate API calls and arguments given the task. Gemini 2.5 generates 2 different feasible plans for putting the banana in the bowl. The first solution is to simply pick up the banana, move it above the bowl, and drop it. The second solution lifts the banana, moves the bowl below the banana, and then drops the banana.

**Example 1:** Gemini 2.5 Generate high-level planning code for pick-and-place tasks with different strategies.

**Prompt:**

*You are given a robot control API and example code below:*

```
# Provided API
class RobotAPI:
  def detect_object(self, obj: str) -> Detection
    """Detects the given object's XYZ location"""

  def get_grasp_position_and_euler_orientation(self, gripper: str, object_name: str) -> tuple[numpy.ndarray, numpy.ndarray]:
    """Returns the grasp position and orientation for the given object and gripper from the Gemini Robotics ER model or other grasping primitives.

  def move_gripper_to(self, gripper: str, position: numpy.ndarray, orientation: numpy.ndarray):
    """Moves the gripper to the given position and orientation."""
   
  def move_gripper_to_safe_position(self, gripper: str):
    """Moves the given gripper to a safe position out of the table area."""

  def open_gripper(self, gripper: str):
    """Opens the given gripper."""
    
  def close_gripper(self, gripper: str):
    """Closes the given gripper."""

robot=RobotAPI()

# Example code
robot.open_gripper(gripper='RIGHT')
banana_detection = robot.detect_object(obj='banana')
banana_position = banana_detection.position
print(f"Detected banana position: {banana_position}")    # Gemini uses this to determine which gripper to use.

grasp_position, grasp_orientation = robot.get_grasp_position_and_euler_orientation(gripper='RIGHT', object_name='banana')
pre_grasp_position = grasp_position + np.array([0, 0, 0.1]) # Add 10cm to the Z-coordinate for pre-grasp
robot.move_gripper_to(gripper='RIGHT', position=pre_grasp_position, orientation=grasp_orientation)
robot.move_gripper_to(gripper='RIGHT', position=grasp_position, orientation=grasp_orientation)
robot.close_gripper(gripper='RIGHT')
```

Python

Copied

*Now generate code for the task “put the banana in the bowl”.*

**Response 1 with results of code executed:**

Reasoning (abbreviated)

1: The current position of the right gripper is `[-0.04, -0.028, 0.176]`.

2: The bowl's detected position is `[-0.03839983, -0.02811164, 0.0073104]`.

3: To place the banana inside the bowl, the gripper's Z-coordinate needs to be lowered. I will use the bowl's detected X and Y coordinates for the target position. For the Z-coordinate, I will use the bowl's detected Z-coordinate (`0.0073104`) and add a small offset (e.g., 0.03m) to ensure the banana is placed inside the bowl and not through the table. This would result in a target Z of approximately `0.007 + 0.03 = 0.037m`. This Z-coordinate is higher than the bowl's base but lower than the typical height of a banana when standing on the table, ensuring it's placed \*into\* the bowl.

**Code Snippet:**

```
# Detect the bowl's position (re-detect to ensure fresh data, though it's unlikely to have moved)
bowl_detection = robot.detect_object('bowl')
if bowl_detection.position is None:
    raise ValueError("Bowl not detected.")

# Define the target Z-coordinate for dropping the banana into the bowl
# Use the bowl's Z-position and add an offset to place the banana inside.
# The banana's original Z was ~0.032, bowl's Z is ~0.007.
# A target Z of 0.037 (0.007 + 0.03) should place it inside the bowl.
drop_z = bowl_detection.position[2] + 0.03
```

Python

Copied

[![


Sorry, your browser doesn't support playback for this video

](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/wagtailvideo-66cw7vmd_thumb.jpg)](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/lift_and_drop_final_v2.mp4)

**Response 2 with results of code executed:**

Reasoning (abbreviated)

# Re-planning due to reachability constraints: The RIGHT arm cannot reach the bowl's current position.

# The plan will now involve the LEFT arm moving the bowl to the RIGHT arm's reachable area.

# The RIGHT arm can reach x-coordinates from 0.04m to 0.40m. I will move the bowl to an x-coordinate of 0.10m, which is well within the RIGHT arm's reach and also allows for some clearance from the center.

**Code Snippet:**

```
target_bowl_position = [-0.07274145, -0.08317622, 0.00720479] # Original bowl position
# Move the bowl to an x-coordinate reachable by the RIGHT arm, keeping the same y and z (lifted)
# Let's choose x = 0.10m for the bowl, which is within the right arm's reach (0.04 to 0.40)
# Keep the lifted height at 0.20m
move_bowl_position = [0.10, bowl_detection.position[1], 0.20]
robot.move_gripper_to('LEFT', move_bowl_position, current_left_gripper_orientation)
```

Python

Copied

[![


Sorry, your browser doesn't support playback for this video

](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/wagtailvideo-6ipq9el9_thumb.jpg)](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/bowl_to_banana_final.mp4)

Gemini 2.5 can also effectively utilize a small number of in-context examples to perform more dexterous robot control tasks. In the two examples shown below of an ALOHA robot packing boxes and folding a dress, 10 demonstrations consisting of interleaved reasoning and robot actions for each task were added to Gemini’s context. We’ve created open-source code showing how to do this using Gemini, including examples of the input demonstrations. This enables robots to be taught and deployed on the spot. See the [Colab](https://colab.research.google.com/drive/19D83Yv2LILLR5pFRqFnBHsUw9MXAI2lP).

**Example 2:** Gemini 2.5 (Flash) utilizes a small number of in-context examples to perform more dexterous robot control tasks.

**Prompt:** *see* [*colab*](https://colab.research.google.com/drive/19D83Yv2LILLR5pFRqFnBHsUw9MXAI2lP)*.*

**Response with results of code executed:**

[![


Sorry, your browser doesn't support playback for this video

](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/wagtailvideo-9lzps7qf_thumb.jpg)](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/pack_box_icl.mp4)

[![


Sorry, your browser doesn't support playback for this video

](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/wagtailvideo-9ysg7lq3_thumb.jpg)](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/fold_dress_icl.mp4)

## Building interactive robotics applications with the Live API

The [Live API](https://ai.google.dev/gemini-api/docs/live) for realtime streaming was recently introduced and can be used to build interactive applications that let people control robots using their voice. Intuitive human-robot-interaction is an important aspect of making robots that are easy and safe to use. We recently showcased an interactive [Gemini Robotics demo](https://www.youtube.com/watch?v=1oSSex9b6fc) at I/O 2025, which was built around Live API for voice interaction and function calling.

Live API supports both audio and video as input modalities, and audio / text as output modalities. This allows you to send both voice input and the robot camera feed to the Live API. This is even more powerful when combined with tool use.

Tool use allows Live API to go beyond just conversation by enabling it to perform actions in the real-world while maintaining a real time connection. For example, the robot APIs defined above can be defined as function calls including `robot.open_gripper()`, `robot.close_gripper()` and `robot.move_gripper_to()`. After they are defined as tool calls, they can be integrated into the workflow where people can interact with the robot using voice in real time. Developers can [get started on GitHub](https://github.com/google-gemini/live-api-web-console), and refer to [API documentation](https://ai.google.dev/gemini-api/docs/live-tools) for function calling features.

[![


Sorry, your browser doesn't support playback for this video

](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/wagtailvideo-hfu3sy_o_thumb.jpg)](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/mm_live_short.mp4)

🔊 Demonstration of a realtime web console for robotics built with Live API, right click to open in a new tab for audio.

### **Safety**

The 2.5 Pro and 2.5 Flash models demonstrate robust performance on the [ASIMOV Multimodal and Physical Injury benchmarks](https://asimov-benchmark.github.io/) released along with the [Gemini Robotics tech report](https://deepmind.google/models/gemini-robotics/), exhibiting accuracy comparable to that of 2.0 models. Beyond the ASIMOV benchmarks, the 2.5 Pro and 2.5 Flash models also exhibit excellent performance in rejecting prompts that attempt to leverage embodied reasoning capabilities while violating safety policies such as promoting harmful stereotypes, discrimination, or endangerment of minors. Following rigorous evaluation against such synthetically generated adversarial prompts, 2.5 Pro and Flash demonstrated near-zero violation rates.

## How Gemini is being used today for Robotics

In March we released the [Gemini Robotics-ER model](https://deepmind.google/models/gemini-robotics/gemini-robotics-er/) and we’re already inspired by how the community is using it for robotics applications. Check out these examples of interactivity, perception, planning, and function calling from our trusted testers: [Agile Robots](https://www.agile-robots.com/en/), [Agility Robotics](https://www.agilityrobotics.com/), [Boston Dynamics](https://bostondynamics.com/), and [Enchanted Tools](https://enchanted.tools/).

[![


Sorry, your browser doesn't support playback for this video

](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/wagtailvideo-vhiy9_rf_thumb.jpg)](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/agile-robots-demo_7yG7BAf.mp4)

[![


Sorry, your browser doesn't support playback for this video

](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/wagtailvideo-3_nyjmsr_thumb.jpg)](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/agility-robotics-demo.mp4)

[![


Sorry, your browser doesn't support playback for this video

](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/wagtailvideo-6hssh621_thumb.jpg)](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/boston-dynamics-demo_2.mp4)

[![


Sorry, your browser doesn't support playback for this video

](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/wagtailvideo-gdgwydio_thumb.jpg)](https://storage.googleapis.com/gweb-developer-goog-blog-assets/original_videos/enchanted_tools_1_1.mp4)

We can’t wait to see what you create.

### **References**

Embodied reasoning in Gemini 2.5 Flash and Pro are available in Google AI Studio, the Gemini API, and Vertex AI. To start building with these models in the Gemini API, visit [our developer guide](https://ai.google.dev/gemini-api/docs/vision?lang=python) to get started. If you are interested in building with Gemini Robotics-ER, please sign up for the [trusted tester program](https://deepmind.google/models/gemini-robotics/).

---

### **Acknowledgements**

We thank researchers in the Embodied Reasoning team: Alex Hofer, Annie Xie, Arunkumar Byravan, Ashwin Balakrishna, Assaf Hurwitz Michaely, Carolina Parada, David D'Ambrosio, Deepali Jain, Jacky Liang, Jie Tan, Junkyung Kim, Kanishka Rao, Keerthana Gopalakrishnan, Ksenia Konyushkova, Lewis Chiang, Marissa Giustina, Mohit Sharma, Montserrat Gonzalez Arenas, Nicolas Heess, Norman Di Palo, Peng Xu, Pierre Sermanet, Sean Kirmani, Stefani Karp, Stefano Saliceti, Steven Hansen, Sudeep Dasari, Ted Xiao, Thomas Lampe, Tianli Ding, Wenhao Yu, and Wentao Yuan; Gemini team: Xi Chen, Weicheng Kuo, and Paul Voigtlaender; Robotics Safety team: Vikas Sindhwani and Abhishek Jindal; Product and Program support: Kendra Byrne and Sally Jesmonth; and members of developer relationship team: Paul Ruiz and Paige Bailey, for helping with this article.

posted in:

* [Gemini](/en/search/?product_categories=Gemini)
* [Google AI Studio](/en/search/?product_categories=Google+AI+Studio)
* [AI](/en/search/?technology_categories=AI)
* [How-To Guides](/en/search/?content_type_categories=How-To+Guides)
* [Gemini API](/en/search/?tag=Gemini API)
* [Gemini 2.5 Pro](/en/search/?tag=Gemini 2.5 Pro)
* [multimodal AI](/en/search/?tag=multimodal AI)
* [Learn](/en/search/?tag=Learn)
* [Developer Tools](/en/search/?tag=Developer Tools)
* [code generation](/en/search/?tag=code generation)
* [Gemini 2.5 Flash](/en/search/?tag=Gemini 2.5 Flash)
* [DeepMind](/en/search/?tag=DeepMind)
* [robotics](/en/search/?tag=robotics)

Previous

Next

Related Posts

[![Introducing Gemini 2.5 Flash Image, our state-of-the-art image model](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/9250041494c20cef94e6d1335a819861.jpg)

Gemini
Google AI Studio
AI
Announcements

Introducing Gemini 2.5 Flash Image, our state-of-the-art image model

AUG. 26, 2025](/en/introducing-gemini-2-5-flash-image/)
[![New Gemini API updates for Gemini 3](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/e52cb82d4a66b52f46cf7a12d626c2ee.png)

AI
Best Practices

New Gemini API updates for Gemini 3

NOV. 25, 2025](/en/new-gemini-api-updates-for-gemini-3/)
[![Unlocking Peak Performance on Qualcomm NPU with LiteRT](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/2a05e190e3ebac3a37c7e5d4c45512ba.png)

Mobile
AI
Announcements
Industry Trends

Unlocking Peak Performance on Qualcomm NPU with LiteRT

NOV. 24, 2025](/en/unlocking-peak-performance-on-qualcomm-npu-with-litert/)
[![Beyond the terminal: Gemini CLI comes to Zed](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/56ecbe45bf57c4591fa5ef661a4e85a5.jpg)

Gemini
AI
Announcements

Beyond the terminal: Gemini CLI comes to Zed

AUG. 27, 2025](/en/gemini-cli-is-now-integrated-into-zed/)
[![Announcing the Agent Development Kit for Go: Build Powerful AI Agents with Your Favorite Languages](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/6aa4fc0ded8d3e75c5ca8480c0295db2.png)

AI
Cloud
How-To Guides
Announcements

Announcing the Agent Development Kit for Go: Build Powerful AI Agents with Your Favorite Languages

NOV. 7, 2025](/en/announcing-the-agent-development-kit-for-go-build-powerful-ai-agents-with-your-favorite-languages/)
[![Announcing User Simulation in ADK Evaluation](ai-leaders-insights/产业应用与实践/具身应用/机器人/images/182f32465b09fbcd595c4de40ea12516.png)

AI
Cloud
How-To Guides
Announcements

Announcing User Simulation in ADK Evaluation

NOV. 7, 2025](/en/announcing-user-simulation-in-adk-evaluation/)

---

*爬取时间: 2025-11-28 21:55:56*
