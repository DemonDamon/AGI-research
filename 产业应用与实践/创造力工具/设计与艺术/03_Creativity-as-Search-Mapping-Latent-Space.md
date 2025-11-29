# Creativity as Search: Mapping Latent Space

**来源**: [https://runwayml.com/research/creativity-as-search-mapping-latent-space](https://runwayml.com/research/creativity-as-search-mapping-latent-space)

---

# Runway Research | Creativity as Search: Mapping Latent Space

原文链接: https://runwayml.com/research/creativity-as-search-mapping-latent-space

Creativity as Search: Mapping Latent Space

December 2, 2024

by Bryan Loh

![Creativity as Search: Mapping Latent Space](ai-leaders-insights/产业应用与实践/创造力工具/设计与艺术/images/c335fe1639f35fc8787b59a623265486.png)

Creative exploration can be viewed as a search process in a space of possibilities. We create solutions, evaluate them, and refine them until we reach a result that we are happy with. The latent spaces of our generative models provide a direct software analog to this abstract space, where each point in latent space represents a possible creation conforming to patterns learned from data.

Traditionally, creative software has served primarily in the final stages of refinement and production. One reason for this is language: we had to translate our creative intent into tedious sequences of low-level, machine-readable parameters such as pixel coordinates and hex codes. Generative models have changed this. Instead of manipulating these low-level parameters, we can now express intent naturally, across various modalities—*"what would this picture look like at evening time?"* or *"make this video match the style of these images."* This shift enables software to move beyond production tools to become instruments of creative exploration.

However, navigating these vast latent spaces presents new challenges in interface design:

* How can we best visualize these high-dimensional spaces to help users discover interesting regions to explore?
* How can we enable precise user control while still leaving room for serendipitous moments of discovery?
* How can we support the nonlinear nature of creative exploration, enabling both divergent and convergent thinking?

[We recently shared](https://runwayml.com/research/pioneering-new-interfaces-age-generative-media) our philosophy around interface design for this new era of media, and today, we're excited to present a prototype that explores these questions through video keyframing.

##### Graph Structure: A Window into Latent Space

![A graph made up of image nodes and video edges. Continuous paths through the graph represent a continuous video sequence.](ai-leaders-insights/产业应用与实践/创造力工具/设计与艺术/images/824a3da6ca811d497d154736b305dcf9.png)

A graph made up of image nodes and video edges. Continuous paths through the graph represent a continuous video sequence.

The Graph structure is the foundation of the prototype. Images are represented as nodes, serving as waypoints in the model's latent space. These nodes can be connected to other nodes to create an edge; a video that transitions from the first frame to the last frame across latent space and time.

[](https://d3phaj0sisr2ct.cloudfront.net/site/content/videos/2_nodes_edge.mp4)

Creating a video by connecting two image nodes. The origin node will be the first frame of the video, and the target node will be the last frame.

##### Balancing Control and Serendipity

Precise controls help limit the vast space of possibilities, but at the same time, variation and unpredictability can result in "happy accidents"–possibilities that we would not have considered given precise control. To balance this tradeoff, we provide two affordances for users to manipulate images in a "relational" manner that allows unpredictability in consistent dimensions.

[](https://d3phaj0sisr2ct.cloudfront.net/site/content/videos/3_image_variations.mp4)

Generating alternate compositions of an image using “Image Variations”.

Users can transform selected images through *“Image to Image”*—preserving the original composition while altering the style via text prompts—and *“Image Variations”*—which maintains the original style while varying the composition.

[](https://d3phaj0sisr2ct.cloudfront.net/site/content/videos/4_image_to_image.mp4)

Restyling versions of an image using text prompts and “Image to Image”.

##### Supporting Non-Linear Exploration

[](https://d3phaj0sisr2ct.cloudfront.net/site/content/videos/5_branches.mp4)

Branching off the mid-point of a video to create a separate thread of experimentation.

Creative exploration rarely follows a straight line. The graph structure naturally affords exploration by allowing users to diverge at various points, creating new forks of possible alternatives. As more exploration occurs, the graph grows naturally, tracking various experimental paths.

[](https://d3phaj0sisr2ct.cloudfront.net/site/content/videos/6_sequencer.mp4)

Choosing a continuous path within the graph structure for previewing.

This allows users to construct non-linear timelines. We provide a sequencer to allow users to export their non-linear timelines into a video with a linear timeline, similar to a “choose your own adventure” experience.

##### An Open Workspace

Beyond the Graph structure, we do not impose any organizational constraints on the workspace. Users have complete freedom to organize their nodes and edges—clustering related explorations or separating distinct creative experiments as their process demands.

[](https://d3phaj0sisr2ct.cloudfront.net/site/content/videos/7_open_workspace.mp4)

Experiments clustered across the open workspace, showcasing different explorations.

##### Exploring Further

Our prototype demonstrates how creative interfaces can evolve in the age of generative media. The graph structure provides a way to navigate latent space, treating images as waypoints and transitions as paths through creative possibilities.

Through continued experimentation and curiosity to find new interface primitives, we can realize the full potential of generative models not just as production tools, but as active partners in the creative process—expanding our ability to discover and explore new possibilities.

Discover more

[![Runway Partners with Lionsgate](ai-leaders-insights/产业应用与实践/创造力工具/设计与艺术/images/e105dc0aa8eb6dfebbdac342d8c051ca.jpg)

Runway Partners with Lionsgate](/news/runway-partners-with-lionsgate)[![Exploring the Future of Filmmaking: Runway’s programming partnership with Tribeca Festival 2024](https://d3phaj0sisr2ct.cloudfront.net/site/images/news/1.webp)

Exploring the Future of Filmmaking: Runway’s programming partnership with Tribeca Festival 2024](/news/runway-partners-with-tribeca-festival)[![Partnering with Media.Monks to expand creative horizons](ai-leaders-insights/产业应用与实践/创造力工具/设计与艺术/images/e0c9fa5dae8a483c7208c3ae485198f2.jpg)

Partnering with Media.Monks to expand creative horizons](/news/partnering-with-media-monks)

---

*爬取时间: 2025-11-28 21:55:11*
