# CES 2026：黄仁勋与英伟达的物理AI宣言

**报告日期**: 2026年1月7日
**作者**: Damon Li

---

## 摘要

在2026年国际消费电子展（CES）上，英伟达（NVIDIA）创始人兼首席执行官黄仁勋（Jensen Huang）发表了一场具有里程碑意义的主题演讲，系统性地阐述了公司从芯片到物理世界的全栈AI战略。本次演讲的核心并非发布单一的消费级产品，而是宣告了一个新时代的到来：**物理AI（Physical AI）**。黄仁勋明确指出，AI正从云端的虚拟世界大规模迁移至汽车、机器人、工业制造等物理实体中，而英伟达正通过“极端协同设计”的算力革命、从“生成式”到“推理式”的模型范式转移，以及全面的开源生态，为这场变革提供核心动力 [1][2]。

> “计算已经因加速计算、因人工智能而被根本性地重塑。这意味着过去十年约10万亿美元的计算基础设施，现在正在被现代化为这种新的计算方式。”
> — 黄仁勋，CES 2026

本次演讲的三大主线清晰地勾勒出英伟达的未来蓝图：

1.  **基础设施重构**：通过新一代 **Vera Rubin 平台**，以超出摩尔定律的性能飞跃，将AI推理成本降低一个数量级，为代理智能体（Agentic AI）的规模化应用扫清障碍。
2.  **模型范式转移**：正式确立从“生成式AI”向“**推理型AI**”（Test-time Scaling）的演进，强调AI需要具备多步思考、规划和长时记忆的能力。
3.  **物理世界落地**：宣布“物理AI”进入商业变现期，通过与**梅赛德斯-奔驰**和**西门子**等行业巨头的深度合作，将AI能力注入实体经济的核心环节。

---

## 核心发布：Vera Rubin 平台——新一代AI引擎

本次演讲最重磅的发布是新一代AI计算平台——**Vera Rubin**，该平台已全面投产，并计划于2026年下半年交付首批客户。黄仁勋强调，面对AI推理成本每年需下降10倍、而AI“思考”产生的Token数量每年增长5倍的巨大挑战，传统的芯片迭代已无法满足需求。Rubin平台的设计哲学是“**极端协同设计**”（Extreme Codesign），即不再是简单地提升单个组件的性能，而是将GPU、CPU、网络、存储和软件作为一个整体进行系统级优化 [3]。

### Rubin 平台关键组件与性能对比

Rubin平台由六大核心组件构成，其性能相较于上一代Blackwell平台实现了指数级飞跃。

| 组件 | 型号/规格 | 关键特性与性能提升 |
| :--- | :--- | :--- |
| **GPU** | Rubin GPU | **50 PFLOPS** 的NVFP4推理性能（Blackwell的**5倍**），3360亿晶体管（1.6倍），8组HBM4内存 |
| **CPU** | Vera CPU | 88个定制Arm核心，采用“空间多线程”设计，专为Agentic处理和数据移动优化 |
| **互联** | NVLink 6 | 机架内通信带宽达 **240 TB/s**（全球互联网总带宽的2倍以上） |
| **网络** | Spectrum-X Ethernet Photonics | 用于数据中心横向扩展（Scale-out）的光子网络技术 |
| **网卡** | ConnectX-9 SuperNICs | 超级网络接口卡，为大规模AI集群提供超低延迟网络 |
| **DPU** | BlueField-4 DPU | 驱动AI原生存储平台，负责数据处理和安全隔离 |

*表 1: Vera Rubin 平台核心组件及性能亮点 [1][4]*

### 成本革命：AI原生存储平台

为了解决大模型应用中的“显存墙”问题，Rubin平台引入了**AI原生推理上下文内存存储平台**（NVIDIA Inference Context Memory Storage Platform）。这是一个专为AI设计的KV-cache层，能够将长上下文推理的每秒Token处理量提升5倍，同时将每TCO美元的性能和能效均提升5倍。这一创新使得运行具有长时记忆的复杂AI Agent在经济上成为可能，最终将Token生成成本降低至Blackwell平台的**十分之一** [3]。

---

## 性能、价格与购买渠道

### 四代旗舰GPU性能对比

下表详细对比了NVIDIA最近四代数据中心GPU的关键性能指标，展示了其惊人的迭代速度。

| 指标 | Rubin (R100) | Blackwell (B200) | Hopper (H100) | Ampere (A100) |
| :--- | :--- | :--- | :--- | :--- |
| **发布年份** | 2026 | 2024 | 2022 | 2020 |
| **推理性能 (FP4)** | **50 PFLOPS** | 10 PFLOPS | ~5 PFLOPS | ~2.5 PFLOPS |
| **训练性能 (FP8)** | **35 PFLOPS** | 10 PFLOPS | ~5 PFLOPS | - |
| **晶体管数量** | **3360亿** | 2100亿 | 800亿 | 540亿 |
| **内存类型** | HBM4 | HBM3e | HBM3 | HBM2e |
| **内存带宽** | **22 TB/s** | 8 TB/s | 3.35 TB/s | 2 TB/s |
| **NVLink 带宽** | **3.6 TB/s** | 1.8 TB/s | 900 GB/s | 600 GB/s |

*表 2: NVIDIA 四代旗舰数据中心 GPU 性能对比 [4][6]*

### 价格对比与预测

| 型号/平台 | 价格 (估算) | 备注 |
| :--- | :--- | :--- |
| **Vera Rubin NVL72** | **$8.4M - $16.8M** | 预测价格，取决于市场策略 [7] |
| **Blackwell GB200 NVL72** | **~$3.35M** | 估算价格 |
| **H200 单卡** | **$27,000** | 中国市场报价 (2026年1月) [8] |
| **H100 单卡** | **$25,000 - $40,000** | 市场浮动价格 |
| **A100 单卡** | **$10,000 - $15,000** | 二手市场价格 |

*表 3: NVIDIA GPU 价格对比与预测 [7][8]*

### 购买渠道

1.  **企业级采购 (推荐)**:
    *   **NVIDIA 官方**: 直接联系NVIDIA企业销售部门。
    *   **授权经销商**: Dell, HPE, Supermicro, Lenovo, 浪潮等。

2.  **云服务商租赁 (灵活)**:
    *   **国际**: AWS, Azure, Google Cloud, Oracle Cloud。
    *   **专业**: Lambda Labs, Paperspace, CoreWeave。
    *   **中国**: 阿里云, 腾讯云, 华为云等。

3.  **二手市场 (预算有限)**:
    *   **平台**: eBay, Reddit (r/hardwareswap), 淘宝/闲鱼。
    *   **风险**: 无质保，可能存在矿卡风险，不适合生产环境。

---

## 模型与生态：从开源到物理世界

黄仁勋宣布英伟达将转型为“前沿AI模型构建者”，并将其在超级计算机上训练的六大领域基础模型完全开源，旨在赋能全球各行各业。

### 六大开源模型家族

- **Clara**: 医疗健康
- **Earth-2**: 气候科学
- **Nemotron**: 通用推理与多模态AI
- **Cosmos**: 机器人与物理世界仿真
- **GR00T**: 具身智能
- **Alpamayo**: 自动驾驶

### 物理AI的商业化元年

演讲中最激动人心的部分莫过于物理AI的商业化落地。英伟达通过两大合作，正式宣告AI走出屏幕，进入实体经济。

1.  **自动驾驶：Alpamayo模型上车**
    *   **Alpamayo R1**是业界首个开源的推理视觉-语言-动作（VLA）模型，它不仅能“看”和“开”，更能“思考”和“推理”其驾驶行为。
    *   首款搭载该模型的**梅赛德斯-奔驰CLA**将于2026年在美国上路，标志着Level 4级自动驾驶能力进入消费级市场 [5]。

2.  **工业制造：与西门子共创工业元宇宙**
    *   通过将英伟达的 **Omniverse** 仿真平台、合成数据生成能力与西门子的工业软件（如Teamcenter X）深度集成，两家公司正在构建工厂的“数字孪生”。
    *   这使得企业可以在虚拟世界中完成机器人的训练、产线的调试和优化，然后再部署到物理世界，极大地缩短了开发周期并降低了成本。黄仁勋预言：“这些制造工厂将本质上成为巨型机器人。” [1]

---

## 游戏与创作：技术普惠

除了数据中心和物理AI，英伟达也发布了面向游戏玩家和创作者的一系列更新，核心是将前沿AI技术下放至PC端。

- **DLSS 4.5**：引入“动态多帧生成”技术，并为RTX 50系列GPU提供6X多帧生成模式，进一步提升游戏性能和画质。
- **NVIDIA ACE**：为游戏NPC赋予长期记忆和更强的交互智能，在《PUBG: BATTLEGROUNDS》等游戏中落地。
- **4K AI视频生成**：通过RTX GPU加速，在PC上实现高质量的AI视频生成。

## 结论

黄仁勋在CES 2026的演讲，不仅是一次技术发布，更是一次战略宣言。英伟达通过对算力、模型和应用的全栈布局，清晰地展示了其引领下一波AI浪潮的决心。从将推理成本降低一个数量级的Rubin平台，到赋能各行各业的开源模型，再到让AI在物理世界中创造价值的商业化落地，英伟达正在系统性地构建一个“AI无处不在”的未来。对于整个科技行业而言，2026年将是“物理AI”从概念走向现实的关键一年。

---

## 参考文献

[1] NVIDIA. (2026, January 5). *NVIDIA Rubin Platform, Open Models, Autonomous Driving: NVIDIA Presents Blueprint for the Future at CES*. NVIDIA Blog. [https://blogs.nvidia.com/blog/2026-ces-special-presentation/](https://blogs.nvidia.com/blog/2026-ces-special-presentation/)

[2] The Verge. (2026, January 6). *The biggest Nvidia announcements at CES 2026*. [https://www.theverge.com/tech/856439/nvidia-ces-2026-announcements-roundup](https://www.theverge.com/tech/856439/nvidia-ces-2026-announcements-roundup)

[3] 华尔街见闻. (2026, January 6). *黄仁勋CES演讲全文来了！Rubin全面投产，算力暴涨5倍，砸掉智驾门槛All in物理世界*. [https://wallstreetcn.com/articles/3762621](https://wallstreetcn.com/articles/3762621)

[4] 新浪财经. (2026, January 6). *比Blackwell算力提升5倍！黄仁勋展示Vera Rubin计算平台*. [https://finance.sina.com.cn/tech/shenji/2026-01-06/doc-inhfiqwt1450987.shtml](https://finance.sina.com.cn/tech/shenji/2026-01-06/doc-inhfiqwt1450987.shtml)

[5] Engadget. (2026, January 6). *Everything NVIDIA announced at CES 2026*. [https://www.engadget.com/ai/everything-nvidia-announced-at-ces-2026-225653684.html](https://www.engadget.com/ai/everything-nvidia-announced-at-ces-2026-225653684.html)

[6] NVIDIA Developer. (2026, January 5). *Inside the NVIDIA Rubin Platform: Six New Chips, One AI Supercomputer*. NVIDIA Technical Blog. [https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/](https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/)

[7] The Next Platform. (2026, January 5). *Nvidia’s Vera-Rubin Platform Obsoletes Current AI Iron Six Months Ahead Of Launch*. [https://www.nextplatform.com/2026/01/05/nvidias-vera-rubin-platform-obsoletes-current-ai-iron-six-months-ahead-of-launch/](https://www.nextplatform.com/2026/01/05/nvidias-vera-rubin-platform-obsoletes-current-ai-iron-six-months-ahead-of-launch/)

[8] PC Online. (2026, January 4). *H200显卡只要19万元NVIDIA对国区定价良心了：6倍H20性能*. [https://news.pconline.com.cn/2057/20571212.html](https://news.pconline.com.cn/2057/20571212.html)
