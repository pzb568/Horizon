---
layout: default
title: "Horizon Summary: 2026-10-23 (ZH)"
date: 2026-10-23
lang: zh
---

> 从 44 条内容中筛选出 17 条重要资讯。

---

**科技新闻**
1. [OpenShell – A safe, private runtime for fleets of autonomous AI agents](#item-tech-news-1) ⭐️ 8.0/10
2. [pwn.watch 实时漏洞仪表盘上线](#item-tech-news-2) ⭐️ 8.0/10
3. [Anthropic 将 Agent Skills 标准捐赠给 Agentic AI 基金会](#item-tech-news-3) ⭐️ 8.0/10
4. [We shrank our steerable small TTS to 11.84 MB. WER is unchanged, UTMOS drops ~0.1 \[p\]](#item-tech-news-4) ⭐️ 8.0/10
5. [澳洲法院裁定苹果须向 iPhone 开放第三方应用商店](#item-tech-news-5) ⭐️ 8.0/10
6. [米哈游联合清华大学等开源 GameScaling 游戏操作模型](#item-tech-news-6) ⭐️ 8.0/10
7. [甲骨文发布 Java SE 高危漏洞安全警报](#item-tech-news-7) ⭐️ 8.0/10
8. [Nvidia 禁运 B300 芯片现身中国国有网络](#item-tech-news-8) ⭐️ 8.0/10
9. [Quad9 将退出法国市场](#item-tech-news-9) ⭐️ 7.0/10
10. [Faster than earcut: triangulating 3.7M map polygons in 489 ms](#item-tech-news-10) ⭐️ 7.0/10
11. [Carbon-X：开源 14.8B DNA 与文本多模态模型](#item-tech-news-11) ⭐️ 7.0/10
12. [I built Open-XTTS-Trainer: Now you can add new language scripts and train all 3 XTTS v2 components in 1 click \[P\]](#item-tech-news-12) ⭐️ 7.0/10
13. [部分智能电视关闭 ACR 后仍上报内容数据](#item-tech-news-13) ⭐️ 7.0/10
14. [小鹏 IRON 机器人升级：0.2 秒推理实现亚秒级交互](#item-tech-news-14) ⭐️ 7.0/10
15. [古尔曼：iPhone Duo 2 原型测试屏下 Face ID](#item-tech-news-15) ⭐️ 7.0/10
16. [333 个被植入后门的 Tor 出口节点下线](#item-tech-news-16) ⭐️ 7.0/10

**财经新闻**
1. [沪深 300 指数回落 20% 接近熊市](#item-finance-news-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenShell – A safe, private runtime for fleets of autonomous AI agents](https://github.com/NVIDIA/OpenShell) ⭐️ 8.0/10

OpenShell provides a secure, container‑based runtime for autonomous AI agents, offering timely tooling for safe deployment.

hackernews · niemandhier · 10月22日 17:44 · [社区讨论](https://news.ycombinator.com/item?id=50198675)

**标签**: `#AI agents`, `#runtime security`, `#containerization`, `#NVIDIA`, `#open source`

---

<a id="item-tech-news-2"></a>
### [pwn.watch 实时漏洞仪表盘上线](https://pwn.watch/) ⭐️ 8.0/10

pwn.watch（https://pwn.watch/）上线了一个实时漏洞仪表盘，聚合当前公开的高危安全漏洞信息，供开发者和 AI 系统设计者随时查看。该站点持续更新 CVE、漏洞利用代码和受影响的项目列表，帮助用户快速获取最新的安全风险情报。

hackernews · mrkd · 10月22日 14:08 · [社区讨论](https://news.ycombinator.com/item?id=50195543)

**「实时漏洞仪表盘概述」** 实时漏洞仪表盘是一类持续抓取并展示当前公开漏洞（CVE）及其利用情况的服务，帮助开发者和安全团队快速了解哪些漏洞正在被攻击以及补丁状态。pwn.watch 正在提供全球范围内的实时安全事件列表，列出每个 CVE 的严重程度、补丁可用性、已修复版本等信息，并支持按严重性和补丁状态过滤以及 RSS/JSON 推送。

**「影响」** 开发者和安全团队可以直接在仪表盘上监控最新漏洞，及时评估并修补受影响的依赖或模型组件，从而降低因新出现的攻击而导致的系统泄露风险。

**「社区讨论」** 评论者 xbar 认为，“LLM 将引发有史以来最大规模的安全事件”，暗示 AI 生成代码和模型的普及会显著提升漏洞曝光率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pwn.watch/">pwn.watch · live security incidents</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerabilities`, `#AI`, `#software‑engineering`

---

<a id="item-tech-news-3"></a>
### [Anthropic 将 Agent Skills 标准捐赠给 Agentic AI 基金会](https://simonwillison.net/2026/Oct/22/donating-agent-skills/) ⭐️ 8.0/10

Anthropic 今日宣布将其 Agent Skills 标准捐赠给由 Linux 基金会托管的 Agentic AI Foundation（AAIF），该基金会去年由 Anthropic、Block 和 OpenAI 共同创立。此举旨在保持 Agent Skills 的开放、社区驱动和供应商中立，并将其与此前已捐赠的模型上下文协议（MCP）一起交由 AAIF 管理。该标准目前仅为规范性文档，尚未伴随新的实现或功能发布。

rss · Simon Willison · 10月22日 18:09

**「背景」** Agent Skills 是用于描述和共享 AI 代理可执行功能的开放标准，旨在让不同模型和平台能够以统一方式调用这些能力。2025 年 12 月，Linux 基金会成立了 Agentic AI Foundation（AAIF），并接受了包括 Anthropic 的 Model Context Protocol（MCP）在内的首批开源项目，以提供一个中立、社区驱动的治理结构来托管此类规范。AAIF 的成立为 Anthropic 将 Agent Skills 标准捐赠给该基金会提供了合适的组织平台。

**「影响」** 开发者现在可以在 AAIF 的治理下使用统一的 Agent Skills 规范来描述和共享 AI 代理的功能，从而提升不同平台之间的互操作性，并可直接参与标准的进一步演进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linuxfoundation.org/press/linux-foundation-announces-the-formation-of-the-agentic-ai-foundation">Linux Foundation Announces the Formation of the Agentic AI ...</a></li>

</ul>
</details>

**标签**: `#AI standards`, `#Agentic AI`, `#Open source`, `#Anthropic`

---

<a id="item-tech-news-4"></a>
### [We shrank our steerable small TTS to 11.84 MB. WER is unchanged, UTMOS drops ~0.1 \[p\]](https://www.reddit.com/r/MachineLearning/comments/1xcum4s/we_shrank_our_steerable_small_tts_to_1184_mb_wer/) ⭐️ 8.0/10

A compact, quantized steerable TTS model is released, maintaining performance while shrinking to under 12 MB for edge use.

reddit · r/MachineLearning · /u/Working\_Hat5120 · 10月22日 20:57

**标签**: `#text-to-speech`, `#model-compression`, `#quantization`, `#edge-AI`

---

<a id="item-tech-news-5"></a>
### [澳洲法院裁定苹果须向 iPhone 开放第三方应用商店](https://9to5mac.com/2026/10/21/apple-must-open-iphone-to-alternative-app-stores-in-australia-after-epic-games-ruling/) ⭐️ 8.0/10

澳大利亚联邦法院判决，苹果必须自 2027 年 3 月 1 日起在澳洲允许 iPhone 用户通过第三方应用商店或网站安装应用，并开放替代支付方式及外部支付链接。此裁定源于 Epic 对苹果的反垄断诉讼，法官认定苹果在 iOS 应用分发和支付领域拥有实质性市场力量，限制竞争违反澳大利亚竞争法。苹果表示将上诉并已申请暂缓执行。

telegram · zaihuapd · 10月22日 06:54

**「监管背景与 Epic 诉讼」** 苹果的 iOS 应用分发和内置支付体系长期受到反垄断审查。2021 年，Epic Games 在美国提起诉讼，指控苹果利用 App Store 强制使用其支付系统并限制竞争；随后该案在澳大利亚也被提起，指称苹果在 iOS 应用分发和支付市场拥有实质性市场力量，违反《竞争与消费者法》。类似的监管压力已在多个国家出现，监管机构要求苹果开放第三方应用商店和替代支付渠道，以消除对开发者的不公平限制。

**「影响」** 开发者需准备在澳洲通过替代应用商店分发 iOS 应用，可能规避苹果 30%的抽成，并需适配外部支付链接，以符合新规定的合规要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.businessinsider.com/apple-app-store-antitrust-investigations-regulations-around-the-world-payments-2022-1">All the Countries Forcing Apple to Open Its App Store to Competition</a></li>
<li><a href="https://www.theverge.com/2021/3/10/22323100/epic-google-australia-legal-claim-fortnite-play-store-antitrust-lawsuit">Epic expands app store fight even further with new legal... | The Verge</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Antitrust`, `#App Stores`, `#Mobile Development`

---

<a id="item-tech-news-6"></a>
### [米哈游联合清华大学等开源 GameScaling 游戏操作模型](https://arxiv.org/abs/2610.28698v1) ⭐️ 8.0/10

miHoYo and Tsinghua release the open‑source GameScaling model for predictive keyboard/mouse actions, based on Qwen3.5, offering sizable checkpoints and an Apache‑2.0 inference client.

telegram · zaihuapd · 10月22日 11:32

**标签**: `#game AI`, `#vision-language models`, `#open source`, `#machine learning`, `#software engineering`

---

<a id="item-tech-news-7"></a>
### [甲骨文发布 Java SE 高危漏洞安全警报](https://www.oracle.com/security-alerts/alert-cve-2026-91403.html) ⭐️ 8.0/10

Oracle warns of a severe remote code execution flaw in Java SE, urging prompt patching.

telegram · zaihuapd · 10月22日 12:30

**标签**: `#Java`, `#Security`, `#Vulnerability`

---

<a id="item-tech-news-8"></a>
### [Nvidia 禁运 B300 芯片现身中国国有网络](https://theinference.org/article/china-s-state-money-bought-banned-nvidia-b300-servers-then-redacted-the-receipts) ⭐️ 8.0/10

Nvidia B300 chips, under strict US export bans, were reportedly acquired by a Chinese state‑owned leasing firm for AI servers, raising concerns about enforcement and AI hardware availability in China.

telegram · zaihuapd · 10月22日 15:22

**标签**: `#Nvidia`, `#ExportControls`, `#AIHardware`, `#China`, `#SemiconductorSupplyChain`

---

<a id="item-tech-news-9"></a>
### [Quad9 将退出法国市场](https://quad9.net/news/blog/au-revoir-france/) ⭐️ 7.0/10

Quad9 宣布因法国法院要求对特定内容进行阻断的裁决而退出法国市场，计划在 2026 年 11 月 24 日之后通过 GeoIP 过滤阻止法国用户使用其 DNS 解析服务。此举标志着该隐私导向的 DNS 解析器在法国的运营将停止。

hackernews · farrokhi · 10月22日 14:32 · [社区讨论](https://news.ycombinator.com/item?id=50195959)

**「法国法院对 DNS 解析的监管背景」** 法国法院近年来通过判决要求 DNS 解析服务对特定内容（如体育盗版网站）实施地理位置过滤，迫使运营商在法国境内阻止相关域名的解析。这类强制性内容屏蔽已导致 Google、Cloudflare 和 Cisco 等大型 DNS 提供商在法国实施类似的过滤措施，且在法律争议中被迫遵守或面临罚款。Quad9 的退出正是对该司法环境的直接回应。

**「影响」** 法国用户将失去 Quad9 的 DNS 解析服务，需要改用其他公共解析器；在法国依赖 Quad9 的开发者和组织也必须迁移或重新配置其 DNS 解析设置。

**「社区讨论」** Quad9 首席技术官在评论中表示，除退出外公司可能在 11 月 24 日后使用 GeoIP 过滤彻底阻止法国用户；其他评论提到类似的市场退出案例，如 Cisco 之前因法国网络封锁令而退出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.heise.de/en/news/Censorship-ruling-prompts-DNS-service-Quad9-to-leave-France-11497631.html">Censorship ruling prompts DNS service Quad9 to leave France</a></li>

</ul>
</details>

**标签**: `#DNS`, `#Internet Governance`, `#Privacy`, `#Legal`

---

<a id="item-tech-news-10"></a>
### [Faster than earcut: triangulating 3.7M map polygons in 489 ms](https://globus.software/blog/2026/10/16/cutting-map-polygons/) ⭐️ 7.0/10

A new triangulation library outperforms Earcut, processing 3.7 M map polygons in under half a second, which is valuable for high‑performance mapping and graphics applications.

hackernews · molind · 10月22日 09:31 · [社区讨论](https://news.ycombinator.com/item?id=50193170)

**标签**: `#triangulation`, `#computational-geometry`, `#performance`, `#mapping`, `#WebAssembly`

---

<a id="item-tech-news-11"></a>
### [Carbon-X：开源 14.8B DNA 与文本多模态模型](https://www.reddit.com/r/MachineLearning/comments/1xchayq/carbonx_is_an_open_148b_model_trained_jointly_on/) ⭐️ 7.0/10

Carbon‑X 是一个 14.8 B 参数的解码器‑仅模型，能够在同一对话中接受原始 DNA 序列（使用 6‑mer 令牌）并以英文回答。模型在约 302 B 令牌上进行中期训练，权重以 bfloat16 格式可装入单块 80 GB GPU，采用 Apache 2.0 许可证开源。官方基准显示，在五项 DNA 任务上平均得分 66.7%，与闭源的 GPT‑6.1 Sol（67.5%）相近，但尚未进行临床验证，序列的精确操作仍需代码实现。

reddit · r/MachineLearning · /u/jatingargiitk · 10月22日 12:32

**「背景」** 在过去几年中，基因组语言模型（gLM）已被开发用于在 DNA 序列上进行自监督预训练，常使用 k‑mer（如 6‑mer）作为词汇单元，以便将 DNA 表示映射到与文本相同的嵌入空间。这类模型的开源实现（例如 Frontiers 报告的开源 DNA 预测模型）已经证明能够在多个基准上接近专有系统的表现，并为研究者提供无需重新实现的基础设施。

**「影响」** 该模型使研究机构和企业能够在本地 GPU 上对敏感基因组数据进行分析，避免将原始序列上传至云端，从而提升数据隐私和合规性；同时，开源许可鼓励社区进一步优化和验证其在私有变体数据集上的表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.frontiersin.org/journals/medicine/articles/10.3389/fmed.2025.1503229/full">Frontiers | DNA sequence analysis landscape: a comprehensive review...</a></li>
<li><a href="https://arxiv.org/pdf/2407.11435">Genomic Language Models : Opportunities and Challenges</a></li>

</ul>
</details>

**标签**: `#bioinformatics`, `#multimodal‑models`, `#open‑source‑LLM`, `#genomics‑AI`, `#large‑language‑models`

---

<a id="item-tech-news-12"></a>
### [I built Open-XTTS-Trainer: Now you can add new language scripts and train all 3 XTTS v2 components in 1 click \[P\]](https://www.reddit.com/r/MachineLearning/comments/1xcurgj/i_built_openxttstrainer_now_you_can_add_new/) ⭐️ 7.0/10

Open‑XTT‑Trainer provides the first complete, easy‑to‑use training pipeline for XTTS v2, enabling new language scripts and simplifying model fine‑tuning.

reddit · r/MachineLearning · /u/yashubhakt · 10月22日 21:03

**标签**: `#text-to-speech`, `#open-source`, `#machine-learning`, `#speech-synthesis`

---

<a id="item-tech-news-13"></a>
### [部分智能电视关闭 ACR 后仍上报内容数据](https://watchingthewatchers.github.io/watchingthewatchers/index.html) ⭐️ 7.0/10

研究对美国市场 10 家厂商的 12 台智能电视进行 5943 次受控实验，发现部分机型在设置中关闭自动内容识别（ACR）后仍向外发送内容相关流量。VIDAA OS 的电视通过明文 MQTT 上报包含不可重置设备 ID 与音频指纹的数据；Vizio 的 WatchFree+ 则在未加密的 DNS 查询中泄露节目名称，且用户无法关闭该功能。

telegram · zaihuapd · 10月22日 09:50

**「背景」** 自动内容识别（ACR）是智能电视内置的技术，用于实时捕获正在播放的节目音频或视频指纹，并通过网络向厂商或第三方平台上报，以实现内容推荐、观看统计或广告投放等功能。此前已有研究和媒体报道指出，ACR 数据往往包含唯一设备标识或观看记录，若未加密传输会带来隐私泄露风险。

**「影响」** 用户的观看记录可能被未加密地外泄，导致隐私风险；安全团队应审计电视固件并在网络层面阻断或监控 MQTT 与 DNS 流量，以防止未经授权的数据上报。

**标签**: `#privacy`, `#smart-tv`, `#ACR`, `#security`

---

<a id="item-tech-news-14"></a>
### [小鹏 IRON 机器人升级：0.2 秒推理实现亚秒级交互](https://www.ithome.com/1/016/667.htm) ⭐️ 7.0/10

小鹏汽车宣布第二代 VLA 大模型已在端侧落地人形机器人 IRON，机器人能够每 0.2 秒基于当前视觉画面重新推理一次，并预测未来 6 秒内的动作变化。该能力使 IRON 在握手、击掌等交互中能够即时应对对方的临时变招，如手掌突变为拳头或改变击掌位置。小鹏计划在 2026 年底实现 IRON 的量产，并于 2027 年上半年开始在门店、商场等场景交付使用。

telegram · zaihuapd · 10月22日 13:37

**「背景」** 小鹏 IRON 机器人基于公司第二代 VLA（Vision‑Language‑Action）大模型，该模型是面向物理世界的多模态基础模型，已在车载端实现落地并用于机器人推理。VLA 的升级使得模型能够在边缘设备上每 0.2 秒完成一次感知‑决策循环，从而支持实时交互动作。此前 XPeng 已在 2026 年启动 IRON 机器人的小批量试产，为即将的量产奠定了硬件和软件基础。

**「影响」** 零售和商场运营方若在 2027 年上半年部署 IRON，需要提前完成场景适配和接口集成，以利用其亚秒级实时推理提升客户互动体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://researchinchina.com/Htmls/Report/2026/81189.html">Research Report on Application of VLA Large Model in Automobiles...</a></li>
<li><a href="https://chinaevhome.com/2026/07/24/xpeng-iron-humanoid-robot-starts-pilot-production-enters-stores-in-2027/">XPeng IRON Humanoid Robot Starts Pilot Production... | ChinaEVHome</a></li>

</ul>
</details>

**标签**: `#robotics`, `#real-time inference`, `#humanoid AI`, `#hardware`

---

<a id="item-tech-news-15"></a>
### [古尔曼：iPhone Duo 2 原型测试屏下 Face ID](https://9to5mac.com/2026/10/22/gurman-iphone-duo-2-face-id/) ⭐️ 7.0/10

Rumored under‑screen Face ID in the iPhone Duo 2 prototype signals a significant hardware advance for Apple’s biometric system.

telegram · zaihuapd · 10月22日 14:12

**标签**: `#Apple`, `#iPhone`, `#Face ID`, `#under‑screen sensors`, `#hardware`

---

<a id="item-tech-news-16"></a>
### [333 个被植入后门的 Tor 出口节点下线](https://kaba.cx/posts/20261020_Tor/) ⭐️ 7.0/10

A script identified 333 Tor exit relays infected with the Ebury backdoor, leading to their BadExit marking and removal.

telegram · zaihuapd · 10月22日 14:52

**标签**: `#security`, `#privacy`, `#networking`, `#Tor`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [沪深 300 指数回落 20% 接近熊市](https://www.bloomberg.com/news/articles/2026-10-22/china-stocks-set-for-bear-market-as-ai-trade-policy-hopes-fade) ⭐️ 7.0/10

沪深 300 指数较 6 月高点累计回落 20%，标志着 A 股逼近熊市。

telegram · zaihuapd · 10月22日 05:05

**「沪深 300 指数概述」** 沪深 300（CSI 300）指数是衡量上海和深圳证券交易所市值最大、流动性最好的 300 只 A 股的加权基准指数。

**「影响」** 持有 A 股的投资者可能面临进一步的资产缩水。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CSI_300_Index">CSI 300 Index - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Chinese equities`, `#CSI 300`, `#market decline`

---