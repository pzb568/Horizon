---
layout: default
title: "Horizon Summary: 2026-10-17 (ZH)"
date: 2026-10-17
lang: zh
---

> 从 40 条内容中筛选出 16 条重要资讯。

---

**科技新闻**
1. [Apple 发布 MLX 库，支持在 Mac Studio 上推理近万亿参数模型](#item-tech-news-1) ⭐️ 8.0/10
2. [Claude Code 团队的 AI 代码审查流程](#item-tech-news-2) ⭐️ 8.0/10
3. [报告称 90%美国工作时间不在 AI 基准覆盖范围](#item-tech-news-3) ⭐️ 8.0/10
4. [OpenBSD 37 年老内核漏洞被利用](#item-tech-news-4) ⭐️ 8.0/10
5. [\[Research\] 2,788 tokens/s on a single RTX 5090 with a diffusion LLM — Introducing ORL \(fully open source\) \[R\]](#item-tech-news-5) ⭐️ 8.0/10
6. [RTX 5090 停售传闻与 80 系显卡涨价至 90 价](#item-tech-news-6) ⭐️ 8.0/10
7. [Claude reveals ECDSA curve origins](#item-tech-news-7) ⭐️ 7.0/10
8. [在越狱 PS5 上运行 Llama.cpp：本地支持任意 GGUF 模型](#item-tech-news-8) ⭐️ 7.0/10
9. [Waymo 将在多伦多推出自动驾驶出行服务](#item-tech-news-9) ⭐️ 7.0/10
10. [JPEG XL 与 AVIF 在网页图像中的对比](#item-tech-news-10) ⭐️ 7.0/10
11. [I never authorized an integration that scans my secrets](#item-tech-news-11) ⭐️ 7.0/10
12. [Show HN: Gemini 4 Argon plays StarCraft](#item-tech-news-12) ⭐️ 7.0/10
13. [OpenAI 发布 GPT‑Live‑1.1，新增六种语言语音支持](#item-tech-news-13) ⭐️ 7.0/10
14. [阶跃星辰发布 600B 多模态模型 Step 5 Preview](#item-tech-news-14) ⭐️ 7.0/10
15. [苹果首款折叠屏 iPhone Duo 一分钟售罄，盘前股价涨超 2%](#item-tech-news-15) ⭐️ 7.0/10

**财经新闻**
1. [Anthropic IPO 估值预期下调至 1.5 万亿美元](#item-finance-news-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Apple 发布 MLX 库，支持在 Mac Studio 上推理近万亿参数模型](https://machinelearning.apple.com/research/mlx-distributed-inference) ⭐️ 8.0/10

Apple 在今日发布的 MLX 库支持分布式推理，允许在配备最高 512 GB 统一内存的 Mac Studio 上运行近万亿参数的 Muse Spark Open 模型。该实现可在单机或四机集群上实现约 36 tokens/秒的生成速度，提供了 Apple 硬件上本地大模型推理的可行路径。

hackernews · antipaul · 10月16日 13:43 · [社区讨论](https://news.ycombinator.com/item?id=50118320)

**「背景」** MLX 是 Apple 为 macOS 开发的高性能机器学习推理库，支持在配备统一内存的 Mac Studio（如搭载 M5 Ultra/Max 的机型）上进行分布式推理。Muse Spark Open 是 Meta 最近发布的约 800 B 参数的开源大模型，定位为目前最强的美国开放权重模型，旨在让开发者在本地硬件上运行。Apple 将该模型与最新的 MLX 结合，展示了在单台或多台 Mac Studio 上的推理性能。

**「影响」** AI 开发者现在可以在本地 Mac Studio 上进行大模型推理，减少对云 GPU 集群的依赖并可能降低推理成本，但需配备高内存配置并在多机部署时考虑网络同步开销。

**「社区讨论」** 部分评论者指出，Apple 的基准使用 4‑bit 量化对比 Meta 模型的 BF16，可能夸大性能优势；也有人提醒，15‑36 tokens/秒的测评基于 8 k 上下文长度，实际使用更长上下文时效果会受限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.meta.ai/models/muse-spark-open">Muse Spark Open | Meta</a></li>
<li><a href="https://research.meta.ai/blog/muse-spark-open">Introducing Muse Spark Open, The Most Capable US Open‑Weight ...</a></li>

</ul>
</details>

**标签**: `#MLX`, `#distributed inference`, `#Apple hardware`, `#large language models`

---

<a id="item-tech-news-2"></a>
### [Claude Code 团队的 AI 代码审查流程](https://claude.dev/blog/solving-code-review-at-anthropic/) ⭐️ 8.0/10

Anthropic 在其 Claude Code 博客中描述了一套 AI 增强的代码审查系统，该系统自动化了大部分审查工作，仅在最高风险的情况下保留最多一名人工审查员（通常是代码作者本人）。博客称该系统能够每日处理约 30,000 条 Pull Request，显著降低了对人工审查的依赖。此信息来源于 Anthropic 的官方说明，尚未有独立的性能验证。

hackernews · pretext · 10月16日 19:04 · [社区讨论](https://news.ycombinator.com/item?id=50122951)

**「背景」** Claude Code 是 Anthropic 开发的基于终端的 AI 编码助手，能够在命令行环境中生成、调试和运行代码（来源 tool-1-3）。2026 年 10 月 15 日，Anthropic 将其多代理拉取请求审查系统 “Code Review” 正式向 Claude Team 与 Enterprise 客户开放，标志着该功能从内部实验转为可商用的代码审查服务（来源 tool-1-2）。

**「影响」** 使用 Claude Code 的开发团队可以期待审查工作负荷大幅下降，从而加快合并速度，但同时需要评估其对合规性（如 SOC2）和内部安全审计的影响，并可能需要在关键代码上保留额外的人为检查。

**「社区讨论」** 有评论者指出，Claude Code 声称“最多只需一名人类审查员”，这可能与 SOC2 等合规要求冲突，因为这些标准通常要求代码在进入生产前至少由另一位人员审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unite.ai/anthropic-makes-code-review-for-claude-code-generally-available/">Anthropic Makes Code Review for Claude Code Generally ...</a></li>
<li><a href="https://convly.ai/claude-code-review-2026/">Claude Code Review (2026): The Terminal Agent That Actually</a></li>

</ul>
</details>

**标签**: `#code review`, `#AI‑assisted development`, `#software engineering`, `#dev tools`, `#Anthropic`

---

<a id="item-tech-news-3"></a>
### [报告称 90%美国工作时间不在 AI 基准覆盖范围](https://www.mercor.com/research/labor-index/benchmark-map/) ⭐️ 8.0/10

最新报告显示，美国约 90%的工作时间涉及的任务在现有 AI 基准中几乎没有或根本没有得到良好覆盖，且这些基准倾向于过度代表高工资职业的任务。报告指出，尽管 AI 在某些高价值工作上已有较多评测，但大多数日常工作任务仍未被有效衡量。

hackernews · speckx · 10月16日 17:08 · [社区讨论](https://news.ycombinator.com/item?id=50121179)

**「AI 基准概述及其在工作任务评估中的局限」** AI 基准是一组用于评估模型在特定任务上的表现的测试集合，通常只覆盖少数高频或技术性任务。此前 Mercor 将 29 个主流 AI 基准映射到 18,797 个美国职业任务（基于 O\*NET），发现仅有 208 个职业（约 923 个中的 22%）在这些基准中得到代表，说明现有基准对大多数工作任务的覆盖极为有限。

**「影响」** 该发现提醒 AI 研究者和产品团队，当前的评测套件可能无法反映真实工作场景的需求，促使他们开发更广泛且多样化的基准，以评估模型在实际业务中的实用性。

**「社区讨论」** 评论者指出，“覆盖良好”往往等同于“有覆盖”，仅用少量提示（如 13 条）来代表复杂职业（如社工）并不足以评估真实任务；另有评论称现有基准主要聚焦于高收入岗位，导致 AI 实际能提升的工作比例仅在 2%至 5%之间。

<details><summary>参考链接</summary>
<ul>
<li>Mercor Research mapped AI benchmarks to actual US jobs ... - X</li>
<li>AI Benchmark Coverage: 90% of US Work Is Unmeasured - explainx.ai</li>

</ul>
</details>

**标签**: `#AI benchmarks`, `#labor market`, `#AI evaluation`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [OpenBSD 37 年老内核漏洞被利用](https://calif.io/research/big-fish) ⭐️ 8.0/10

研究人员公开了一个在 OpenBSD 内核中存在了 37 年的漏洞利用示例，表明即使是长期且高度审计的代码库仍可能隐藏深层缺陷。该漏洞的出现并被成功利用，凸显了在系统安全防护中发现此类老旧缺陷的难度。

hackernews · rs\_rs\_rs\_rs\_rs · 10月16日 14:44 · [社区讨论](https://news.ycombinator.com/item?id=50118977)

**「背景」** OpenBSD 的内核代码最初来源于 1970 年代的 BSD，仍保持严格的代码审计。该漏洞是一处约 37 年前引入的整数溢出/共享内存计数器溢出，随后在 OpenBSD 7.9 中被链式利用，绕过了 KARL 地址随机化以及 SMAP/SMEP 等硬件防护。该缺陷已在公开的 errata 中得到修补，之前在 NetBSD 的一次代码重写（1999 年）已意外修复。

**「影响」** 该漏洞的公开可能促使 OpenBSD 项目发布安全通告并提供补丁，用户应关注后续更新并及时升级受影响的系统版本。

**「社区讨论」** 有评论指出该代码在 1999 年的 NetBSD 重写中已意外修复，另一位评论者讨论了仅靠审计难以发现此类缺陷，询问模糊测试或静态分析是否能有效检测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/37-year-old-kernel-openbsd-flaw/">37-Year-Old Kernel Flaw Exploited to Gain Root Access on ...</a></li>
<li><a href="https://thehackernews.com/2026/10/researchers-demonstrate-openbsd-root.html">Researchers Demonstrate OpenBSD Root Exploit Chaining 37-Year ...</a></li>
<li><a href="https://aicrier.com/post/got9bqqjbi3quvvti9pq">Big Fish Exploits 37-Year OpenBSD Bug — AICrier</a></li>

</ul>
</details>

**标签**: `#security`, `#openbsd`, `#kernel`, `#vulnerability`

---

<a id="item-tech-news-5"></a>
### [\[Research\] 2,788 tokens/s on a single RTX 5090 with a diffusion LLM — Introducing ORL \(fully open source\) \[R\]](https://www.reddit.com/r/MachineLearning/comments/1x7qgr0/research_2788_tokenss_on_a_single_rtx_5090_with_a/) ⭐️ 8.0/10

ORL introduces a fast, open‑source approach to diffusion LLM inference, delivering multi‑fold token‑throughput gains on modern GPUs.

reddit · r/MachineLearning · /u/arty\_photography · 10月16日 20:03

**标签**: `#diffusion-LLM`, `#inference-optimization`, `#open-source`, `#hardware-acceleration`

---

<a id="item-tech-news-6"></a>
### [RTX 5090 停售传闻与 80 系显卡涨价至 90 价](https://www.techpowerup.com/353578/nvidia-reportedly-ending-the-rtx-5090-reserves-gb202-silicon-for-workstation-gpus) ⭐️ 8.0/10

据报道，英伟达已停止向 GeForce 系列供应 RTX 5090/V2 使用的 GB202 晶圆，并将产能全部转向利润更高的 RTX PRO 系列，导致 RTX 5090 官方出货价从 1,999 美元飙升至 4,500‑6,000 多美元。英伟达个人运算业务副总裁 Jeff Fisher 在台北公开否认停产，但美国官方商城已下架该卡页面，Micro Center 标记为“不再销售”，多家门店已售罄。国内 32 GB 版现货价格也从 9 月初约 3.5 万元涨至 10 月中旬约 5.4 万元。与此同时，基于 GB203 核心、显存仅 24 GB、芯片规模不足 RTX 5090 一半的 RTX 5080 成为新的消费级旗舰，仍保持旗舰价位。

telegram · zaihuapd · 10月17日 00:02

**「GeForce 与 RTX PRO 产品线的区别」** RTX 5090 属于 Nvidia 的 GeForce 消费级显卡系列，使用 GB202 制程的芯片，定位高端游戏与桌面 AI 工作负载。与之对应，Nvidia 还有面向工作站的 RTX PRO 系列，专为专业 AI 与可视化计算设计，采用不同的产品定位和更高的利润率。了解这两条产品线的分工有助于理解传闻中将 GB202 产能转向 RTX PRO、导致消费级 RTX 5090 供应收紧并推高售价的背景。

**「影响」** 高端 GPU 开发者和 AI/ML 研究者将面临 RTX 5090 的供应紧张和价格大幅上升，可能被迫转向性能较低但仍属旗舰价位的 RTX 5080，或延迟采购计划。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/products/workstations/professional-desktop-gpus/">RTX PRO in Desktops | Built For Professionals | NVIDIA</a></li>

</ul>
</details>

**标签**: `#GPU`, `#Nvidia`, `#AI/ML`, `#Hardware`, `#TechIndustry`

---

<a id="item-tech-news-7"></a>
### [Claude reveals ECDSA curve origins](https://www.anthropic.com/research/ecdsa-curve-origins) ⭐️ 7.0/10

Anthropic&\#x27;s Claude uncovered that NIST elliptic curve seeds were generated using a simple timestamp‑seeded RNG, raising security concerns for many systems.

hackernews · ahlCVA · 10月16日 18:55 · [社区讨论](https://news.ycombinator.com/item?id=50122800)

**标签**: `#cryptography`, `#security`, `#software engineering`, `#industry`

---

<a id="item-tech-news-8"></a>
### [在越狱 PS5 上运行 Llama.cpp：本地支持任意 GGUF 模型](https://github.com/cobanov/PS5LM) ⭐️ 7.0/10

开源项目 PS5LM 让越狱的 PlayStation 5 能直接运行 llama.cpp 并加载任意 GGUF 格式的大语言模型。示例使用 2 位量化的 Qwen 3.8‑27B，功耗约 0.07 美元/天，可产出约 200 万 token。该方案仅适用于已越狱的主机，属于爱好者级别的边缘计算实验，未对主流部署或商业使用构成改变。

hackernews · Anon84 · 10月16日 18:32 · [社区讨论](https://news.ycombinator.com/item?id=50122431)

**「背景」** llama.cpp 是用 C/C++ 编写的高性能推理引擎，专门用于在本地 CPU/GPU 上运行 Llama 系列及兼容模型，并采用 GGUF（Quantized GGUF）二进制格式存储模型权重。GGUF 格式使得模型可以在不同硬件上以低内存占用进行推理，llama.cpp 只需提供模型文件路径即可加载并执行。对 PlayStation 5 进行越狱后，能够移除官方固件的限制并在主机上运行自定义 Linux 环境或原生二进制，这为在该主机上编译并运行 llama.cpp 提供了技术前提。

**「在越狱 PS5 上本地运行大型模型的实际效果」** 越狱后的 PlayStation 5 可通过 PS5LM 项目本地运行 GGUF 格式的 LLM，27 B 参数的 Qwen 模型约能达到 20 token/秒，小模型最高可达约 124 token/秒，功耗约 0.7 美元/天，约可生成 200 万 token。此方案为爱好者提供了低成本的边缘推理平台，但仅限于已越狱的主机，存在被 Sony 关闭或法律风险，且性能远低于专业服务器。

**「社区讨论」** 评论者 jjcm 认为即使只运行 2‑bit 量化的 Qwen 3.8‑27B，也足以支撑持续的低成本任务，如服务器错误率监控、安防录像审查或植物生长控制等，日耗电约 70 美分，可输出约 200 万 token，展示了该 hack 的实用潜力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://slowlow999.github.io/The_Jailbreak_Index/">The jailbreak index</a></li>
<li><a href="https://huggingface.co/docs/inference-endpoints/engines/llama_cpp">llama.cpp · Hugging Face</a></li>
<li><a href="https://huggingface.co/docs/hub/gguf-llamacpp">GGUF usage with llama.cpp · Hugging Face</a></li>
<li><a href="https://www.analyticsinsight.net/news/jailbroken-ps5-turns-into-a-local-ai-machine-with-speeds-above-100-tokens-per-second">Jailbroken PS5 Turns into a Local AI Machine with Speeds ...</a></li>
<li><a href="https://wccftech.com/jailbroken-ps5-local-ai-server-27b-llm/">A Jailbroken PS5 Got Turned Into a Local AI Server That Can ...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Edge Computing`, `#Hardware Hacking`, `#Open Source`

---

<a id="item-tech-news-9"></a>
### [Waymo 将在多伦多推出自动驾驶出行服务](https://waymo.com/blog/2026/10/waymo-in-toronto/) ⭐️ 7.0/10

Waymo 宣布将在加拿大多伦多扩展其自动驾驶出行服务，计划在当地部署 Waymo One 车队并创造就业机会。此举属于运营层面的区域扩张，而非技术突破或新硬件发布。

hackernews · ChrisArchitect · 10月16日 14:44 · [社区讨论](https://news.ycombinator.com/item?id=50118981)

**「背景」** Waymo 的无人驾驶出租车服务目前已在美国的洛杉矶、旧金山湾区、菲尼克斯以及通过 Uber 在奥斯汀和亚特兰大运营。2025 年的报道已指出，Toronto 正在被列入 Waymo 考虑的扩张目标之一。

**「影响」** 多伦多居民将在未来可通过 Waymo One 预约无人驾驶车辆，需关注当地监管批准进度并在服务正式上线后注册使用。

**「社区讨论」** 评论中有人分享在东京和奥斯汀的 Waymo 乘车经历，既有对技术的惊喜，也有行程延误的负面反馈；还有用户指出多伦多公告强调了就业机会，并提及其他城市面临的立法阻力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mobilesyrup.com/2025/12/02/toronto-waymo-self-driving-taxis/">Toronto looking into allowing Waymo self-driving taxis</a></li>

</ul>
</details>

**标签**: `#autonomous-vehicles`, `#Waymo`, `#self-driving`, `#AI`, `#transportation`

---

<a id="item-tech-news-10"></a>
### [JPEG XL 与 AVIF 在网页图像中的对比](https://jakearchibald.com/2026/jpeg-xl-vs-avif/) ⭐️ 7.0/10

文章对 JPEG XL 与 AVIF 两种网页图像格式进行技术对比，指出在相同视觉质量下，AVIF 通常能实现更小的文件体积，而 JPEG XL 在最高压缩力度（effort &gt; 7）下可比默认设置再小 2–7%（照片）或约 25%（截图、插画），但编码时间会延长至 9–46 秒，约为默认速度的 50–180 倍。两者的实际表现取决于所选的编码参数和使用场景。

hackernews · farlight · 10月16日 16:12 · [社区讨论](https://news.ycombinator.com/item?id=50120224)

**「背景」** JPEG XL 和 AVIF 是旨在取代 JPEG 与 PNG 的下一代网页图像编解码器，提供更高的压缩率、HDR 支持以及可选的无损模式。它们的实际采用受浏览器兼容性（AVIF 已在多数浏览器可用，而 JPEG XL 支持仍有限）以及编码速度影响——JPEG XL 在高压缩力度下的编码时间远高于默认设置。2026 年的多篇基准报告（如 lpic.cc、cleanor.app、fileza.io）已经对两者在相同质量下的文件大小、质量和编码时长进行了对比，为本次深度分析提供了参考数据。

**「影响」** 对于需要在页面加载速度和带宽成本之间取得平衡的 Web 开发者，若对编码时间不敏感且追求极致体积，可在 JPEG XL 上使用高 effort 设置；若更看重快速生成和兼容性，则应优先采用 AVIF 并调优其压缩参数以获得最佳体积。

**「社区讨论」** 评论者 yhjc2692 说明 libjxl 在高 effort 模式下虽能把文件再压缩 2–7%（照片）或约 25%（插画），但耗时显著增加；而 PaulHoule 则指出 AVIF 在高对比度细节（如赛车灯光）上会出现明显的伪影，提醒使用者注意画质损失。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lpic.cc/en/blog/webp-avif-jpegxl-format-comparison">WebP vs AVIF vs JPEG XL 2026: Complete Format Comparison ...</a></li>
<li><a href="https://cleanor.app/blog/next-gen-image-formats-2026-avif-webp-jpeg-xl-benchmark">AVIF vs WebP vs JPEG XL: Best Web Image Format 2026</a></li>
<li><a href="https://fileza.io/articles/avif-vs-jpeg-xl-2026-comparison">AVIF vs JPEG XL in 2026: The Definitive Format Comparison for ...</a></li>

</ul>
</details>

**标签**: `#image formats`, `#web performance`, `#compression`

---

<a id="item-tech-news-11"></a>
### [I never authorized an integration that scans my secrets](https://github.com/home-assistant/home-assistant.io/issues/49314) ⭐️ 7.0/10

A Home Assistant security feature that checks passwords against breach databases can be turned off, raising privacy concerns for users and developers.

hackernews · trvrprkr · 10月16日 20:33 · [社区讨论](https://news.ycombinator.com/item?id=50124251)

**标签**: `#security`, `#privacy`, `#home-assistant`, `#open-source`, `#software-engineering`

---

<a id="item-tech-news-12"></a>
### [Show HN: Gemini 4 Argon plays StarCraft](https://starskirmish.com/bench/v0-2/) ⭐️ 7.0/10

A new benchmark shows how top LLMs perform when writing code to play StarCraft, highlighting comparative strengths and research directions.

hackernews · \_\_cayenne\_\_ · 10月16日 14:18 · [社区讨论](https://news.ycombinator.com/item?id=50118688)

**标签**: `#LLM benchmarking`, `#Game AI`, `#Code generation`, `#AI research`

---

<a id="item-tech-news-13"></a>
### [OpenAI 发布 GPT‑Live‑1.1，新增六种语言语音支持](https://x.com/OpenAI/status/2110797830361436604) ⭐️ 7.0/10

OpenAI 今日向所有用户发布了语音模型 GPT‑Live‑1.1，正式加入法语、德语、印地语、墨西哥西班牙语、韩语和日语六种语言的语音输出。新版本改进了口音表现并显著缩短了“checking...”的等待时间，提升了实时交互的响应速度。API 对外的语音调用功能尚在即将上线的阶段，现有的 ChatGPT、Codex 与点点语音功能已可直接使用这些新增语言。

telegram · zaihuapd · 10月16日 04:50

**「背景说明」** GPT‑Live 是 OpenAI 的实时语音合成模型，最初在 2024 年以 GPT‑Live‑1.0 版本发布，仅支持英文语音输出，并通过流式 API 为 ChatGPT、Codex 等产品提供即时语音交互功能。此次 1.1 版在此基础上扩展了多语言支持。

**「影响」** 开发者现在可以在上述六种语言上部署实时语音交互应用，但需等待 API 正式开放后才能通过编程方式调用该功能。

**标签**: `#OpenAI`, `#speech AI`, `#multilingual support`, `#API update`

---

<a id="item-tech-news-14"></a>
### [阶跃星辰发布 600B 多模态模型 Step 5 Preview](https://huggingface.co/stepfun-ai/Step-5-Preview) ⭐️ 7.0/10

阶跃星辰在 Hugging Face 上发布了 Step 5 Preview，采用稀疏 MoE 架构，拥有 6000 亿（约 600 B）总参数和 270 亿激活参数，并支持最高 100 万 token 的上下文长度。该模型可接受文本、图像和视频输入，面向智能体工作、软件工程及金融等专业任务。发布方提供 OpenAI 兼容的 API，建议使用 vLLM 或 SGLang 部署，并采用 StepFun Model License 1.0 授权。性能宣称尚未独立验证。

telegram · zaihuapd · 10月16日 06:36

**「稀疏 MoE 与长上下文的技术背景」** 稀疏混合专家（Mixture‑of‑Experts，MoE）架构通过在推理时只激活模型的一小部分参数，使得模型总参数规模可以达到数千亿甚至上万亿，而实际计算量保持在数十亿级别。近年来，多个厂商已推出 600 B 级别的 MoE 大模型，并配备 1 M token 的上下文窗口，以满足需要处理长文档或多轮交互的智能体任务。StepFun 在 2026 年 9 月发布的 Step 5 Preview 继续沿用这一路线，提供 6000 亿总参数、270 亿激活参数的稀疏 MoE，并支持最高 100 万 token 的文本、图像和视频输入【tool-2-1】【tool-2-2】。

**「影响」** 开发者可利用现有的 OpenAI‑兼容堆栈快速部署超大规模多模态智能体，享受长上下文和跨媒体输入的能力，但需准备足够的算力并遵守 StepFun Model License 1.0 的使用限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://build.nvidia.com/stepfun-ai/step-5-preview">Step 5 Preview Model by Stepfun-ai | NVIDIA NIM</a></li>
<li><a href="https://www.i-scoop.eu/stepfun-step-5-preview/">StepFun Step 5 Preview uit Shanghai | i-SCOOP</a></li>

</ul>
</details>

**标签**: `#large-language-model`, `#multimodal`, `#AI-agents`, `#software-engineering`, `#long-context`

---

<a id="item-tech-news-15"></a>
### [苹果首款折叠屏 iPhone Duo 一分钟售罄，盘前股价涨超 2%](https://api3.cls.cn/share/article/2507193?os=android&amp;amp;sv=8.8.4&amp;amp;app=cailianpress) ⭐️ 7.0/10

苹果在 2026 年 10 月 16 日正式开售首款折叠屏手机 iPhone Duo，所有型号在开售后约一分钟即全部售罄。该销售情况导致苹果美股盘前涨幅超过 2%，创下开盘新高。

telegram · zaihuapd · 10月16日 12:45

**「iPhone Duo 折叠屏的前期发布概况」** iPhone Duo 是苹果首款折叠屏手机，苹果在 2026 年 9 月的发布会上首次公开该产品，并在 10 月 16 日凌晨 5 点（太平洋时间）开启预订，提供 7.6 英寸可折叠内屏和全新纳米纹理表面。此前苹果的 iPhone 系列均为固定形态的单屏设备，这次的折叠设计标志着其在硬件形态上的首次突破。

**「影响」** 短时间内的抢购推动了苹果股价在盘前快速上涨，投资者需关注后续供货情况和可能的市场情绪波动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/10/open-up-to-new-possibilities-with-iphone-duo/">Open up to new possibilities with iPhone Duo - Apple</a></li>
<li><a href="https://www.apple.com/newsroom/2026/09/apple-unveils-iphone-duo/">Apple unveils iPhone Duo</a></li>

</ul>
</details>

**标签**: `#hardware`, `#mobile`, `#market`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Anthropic IPO 估值预期下调至 1.5 万亿美元](https://www.reuters.com/business/finance/investors-temper-anthropic-ipo-valuation-expectations-over-revenue-growth-2026-10-15/) ⭐️ 7.0/10

投资者将 Anthropic 的 IPO 估值预期从 2 万亿美元下调至约 1.5 万亿美元，原因包括增速放缓、模型价格竞争加剧及算力投入压力。

telegram · zaihuapd · 10月16日 15:46

**「背景」** Anthropic 是一家专注大模型的人工智能公司，计划在 2026 年首次公开募股（IPO），此前市场普遍预期其估值约为 2 万亿美元。

**「影响」** 此估值下调可能对智谱、MiniMax、Kimi 和 DeepSeek 等其他 AI 公司的估值形成压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tipranks.com/news/anthropic-ipo-why-investors-are-rethinking-its-2-trillion-valuation">Anthropic IPO: Why Investors Are Rethinking Its $2 Trillion ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#IPO`, `#Valuation`, `#Anthropic`, `#TechSector`

---