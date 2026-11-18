---
layout: default
title: "Horizon Summary: 2026-11-18 (ZH)"
date: 2026-11-18
lang: zh
---

> 从 43 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [Java4Shell：OpenJDK Base64 处理导致远程代码执行漏洞](#item-tech-news-1) ⭐️ 8.0/10
2. [ONNX Runtime 仓库从 GitHub 消失](#item-tech-news-2) ⭐️ 8.0/10
3. [Solid 2.0 为 SolidJS 引入服务器 RPC、实时与广播功能](#item-tech-news-3) ⭐️ 8.0/10
4. [Nvidia 停止披露新加坡销售额，收入达 1040 亿美元](#item-tech-news-4) ⭐️ 8.0/10
5. [外部沙箱用于编码代理的安全执行](#item-tech-news-5) ⭐️ 8.0/10
6. [美国超大规模数据中心耗电约占全国 2%](#item-tech-news-6) ⭐️ 8.0/10
7. [不同模型的最佳 Prompt Harness 评估](#item-tech-news-7) ⭐️ 7.0/10
8. [Anthropic 获准纳斯达克全球精选市场上市，代码 ANT](#item-tech-news-8) ⭐️ 7.0/10
9. [Telegram 限制 Bot 与小程序只能使用 Stars 支付](#item-tech-news-9) ⭐️ 7.0/10
10. [可灵 AI 推出支持原生 8K 的 Kling Image 4.0 图像模型](#item-tech-news-10) ⭐️ 7.0/10

**财经新闻**
1. [黄仁勋表态若董事会需要可重返英伟达 CEO](#item-finance-news-1) ⭐️ 8.0/10
2. [工信部委托评估 17 家车企 60 天账期](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Java4Shell：OpenJDK Base64 处理导致远程代码执行漏洞](https://calif.io/java4shell/) ⭐️ 8.0/10

2026 年 11 月披露的 CVE‑2026‑114938（CVSS 9.2）是一种无需认证的远程代码执行漏洞，利用 OpenJDK 在使用 AVX‑512 VBMI 指令集的 x86‑64 处理器上进行 Base64 解码时的缺陷。受影响的运行时包括 Java 17（自 17.0.6 起的全部 17 线）、Java 21、25、27，以及使用该指令集的 Oracle Java 8 Performance Pack；标准的 Java 8/11 在大多数平台上不受影响，ARM64 完全安全。

hackernews · werrett · 11月17日 21:11 · [社区讨论](https://news.ycombinator.com/item?id=50538240)

**「背景」** Java4Shell 利用的是 OpenJDK 在 Base64 解码时对 AVX‑512 VBMI 指令集的实现缺陷，该实现仅在搭载相应指令集的 x86‑64 处理器上启用。该缺陷导致内存损坏，可被未认证的远程攻击者触发，从而实现代码执行。CVE‑2026‑114938 已被标记为 9.2 分的严重漏洞，影响 Java 17（17.0.6 及以后所有 17 系列）以及后续的 Java 21、25、27 版本，而标准的 Java 8/11 通常不受影响。

**「影响」** 受影响的服务器必须尽快升级到已修补的 OpenJDK 版本或通过在启动参数中加入 ‑XX:UseAVX=2 以禁用 AVX‑512 加速，从而阻止该漏洞的利用。

**「社区讨论」** 社区成员 ievans 分享了 Semgrep 检测脚本，用于识别受影响的 HotSpot VM（包括 OpenJDK、Oracle JDK、GraalVM）并提供防御建议；AgentME 则指出可通过 ‑XX:UseAVX=2 标志规避该漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/java-17-rce-vulnerability-cve-2026-114938">Java4Shell Java 17 RCE ( CVE - 2026 - 114938 ): Fix &amp; Versions</a></li>
<li><a href="https://www.rapid7.com/blog/post/etr-cve-2026-114938-reported-critical-pre-authentication-remote-code-execution-java-17/">CVE - 2026 - 114938 : Reported Critical Pre-authentication Remote Code...</a></li>
<li><a href="https://orca.security/resources/research/java4shell-critical-openjdk-base64-decoder-flaw-could-allow-unauthenticated-remote-code-execution/">Java4Shell CVE - 2026 - 114938 : Affected Versions &amp; Mitigation</a></li>

</ul>
</details>

**标签**: `#Java`, `#Security`, `#OpenJDK`, `#RCE`, `#Vulnerability`

---

<a id="item-tech-news-2"></a>
### [ONNX Runtime 仓库从 GitHub 消失](https://github.com/microsoft/onnxruntime) ⭐️ 8.0/10

Microsoft 维护的 ONNX Runtime 开源仓库在 2026 年 11 月 17 日突然从 GitHub 上被删除，导致使用该库的机器学习流水线出现评估失败，并引发对代码安全性和供应链完整性的担忧。该仓库此前拥有约 22,000 星标，是执行 ONNX 模型的主要运行时。

hackernews · nvader · 11月17日 23:18 · [社区讨论](https://news.ycombinator.com/item?id=50539610)

**「ONNX Runtime 简介」** ONNX Runtime 是微软维护的跨平台机器学习模型加速库，能够高效推理符合 ONNX 开放标准的模型，并通过 GitHub 上的源码仓库和文档向社区提供。该项目同时包含可选的遥测功能，依据用户同意向微软发送使用数据以符合隐私法规。

**「影响」** 受影响的工程团队需要立即寻找替代方案，例如转向 Intel 维护的带有 OpenVINO 修改的 fork，或自行从源码构建并关闭遥测，以恢复模型评估和部署流程。

**「社区讨论」** 社区成员指出可以使用 Intel 的 onnxruntime fork 作为临时替代，并有人担心原仓库可能存在后门或遥测功能，建议在自行构建时禁用遥测或阻断相关 DNS 请求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/onnx/onnx">GitHub - onnx / onnx : Open standard for machine learning...</a></li>
<li><a href="https://onnxruntime.ai/docs/">ONNX Runtime is a cross-platform machine-learning model accelerator</a></li>
<li><a href="https://github.com/microsoft/onnxruntime/blob/main/docs/Privacy.md">onnxruntime/docs/Privacy.md at main · microsoft/onnxruntime</a></li>

</ul>
</details>

**标签**: `#ONNX`, `#MachineLearning`, `#Infrastructure`, `#Security`, `#GitHub`

---

<a id="item-tech-news-3"></a>
### [Solid 2.0 为 SolidJS 引入服务器 RPC、实时与广播功能](https://www.solidjs.com/blog/solid-2-0-the-long-hold/) ⭐️ 8.0/10

SolidJS 发布了 2.0 版本，正式加入服务器端 RPC、live（实时）以及 broadcast（广播）三大特性，面向需要在前端直接调用后端逻辑的 Web 开发者。该版本标记为一次重要的功能升级，而非全行业范式的转变。新特性在官方博客中归入 “Built to Be Written by Agents” 章节，旨在提升调试体验并简化前后端交互。

hackernews · pier25 · 11月17日 18:56 · [社区讨论](https://news.ycombinator.com/item?id=50536387)

**「背景」** SolidJS 是一个基于细粒度响应式系统的 JavaScript 前端框架，它通过编译 JSX 将声明式 UI 转换为高效的 DOM 更新，并在过去的版本中已经提供了客户端渲染和基本的服务器端渲染能力。此次 2.0 版本在此基础上加入了服务器端 RPC、Live 数据流和 Broadcast 广播等特性，使得前端代码可以更直接地调用后端函数并实现实时同步。

**「影响」** 前端团队现在可以使用 Solid 2.0 内置的 RPC 与实时广播，省去引入额外的状态同步或实时框架，从而加快开发速度并降低维护成本。

**「社区讨论」** 评论者 pwmglenn 称 Solid 的服务器 RPC、live 与 broadcast 使用感受比 LiveView 或 htmx 更自然；wk\_end 则指出 “Built to Be Written by Agents” 章节的调试改进对人工编写代码同样有益。

**标签**: `#frontend`, `#javascript`, `#web frameworks`, `#solidjs`

---

<a id="item-tech-news-4"></a>
### [Nvidia 停止披露新加坡销售额，收入达 1040 亿美元](https://www.ft.com/content/dbde7a30-548c-4f9d-a4be-7898a0c24dcf) ⭐️ 8.0/10

Nvidia 已停止在财报中单独披露其新加坡子公司 Megaspeed 的销售数据，尽管该子公司在 2025 财年报告了约 1040 亿美元的外部收入。媒体同时指出，美国当局正在调查该业务是否涉及向中国走私 GPU 芯片的行为。此举使得供应链透明度下降，并引发监管合规风险的担忧。该信息基于公司公开的财务公告和媒体报道的指控。

hackernews · louiereederson · 11月17日 17:12 · [社区讨论](https://news.ycombinator.com/item?id=50534631)

**「背景」** Nvidia 的亚洲业务通过子公司 Megaspeed 在新加坡汇总销售额，过去的财报会披露该子公司的收入。美国监管机构已对 Megaspeed 可能将高端芯片走私至中国并违反出口法进行调查，这导致 Nvidia 停止单独报告新加坡的销售数据。

**「影响」** 监管审查可能导致对 Nvidia 供应链的进一步限制，进而影响 AI 硬件在受限地区的可用性，企业在采购 GPU 时需关注合规风险并可能寻找替代供应商。

**「社区讨论」** 评论者 tamarind44 解释说，1040 亿美元是新加坡子公司的外部收入，包含通过该实体路由的所有 GPU 订单；终端客户通常通过 OEM、ODM 和经销商购买，而非直接向 Nvidia 采购，这意味着收入归属与实际芯片流向并不完全等同。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ft.com/content/dbde7a30-548c-4f9d-a4be-7898a0c24dcf?syn-25a6b1a6=1">Nvidia stopped disclosing Singapore sales as revenues hit $104bn</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Semiconductors`, `#AI hardware`, `#Sanctions`

---

<a id="item-tech-news-5"></a>
### [外部沙箱用于编码代理的安全执行](https://simonwillison.net/2026/Nov/17/external-sandboxes-for-coding-agents/) ⭐️ 8.0/10

Prime Radiant 与作者合作推出了“外部沙箱”模式，允许 AI 编码代理的代码在独立的沙箱环境中运行，而代理本身保持在外部。为演示该模式，发布了三套开源服务器实现：使用 v86 在 WebAssembly 中运行 Alpine Linux 的 external‑sandbox‑v86、在 Apple Containers 中运行 Alpine Linux 的 external‑sandbox‑container，以及基于 Microsoft Quicksand 的 external‑sandbox‑quicksand。所有实现提供统一的本地主机 API，并支持可选的 HTTP/HTTPS 允许列表代理和凭证替换功能，以细粒度控制网络访问和安全凭证。

rss · Simon Willison · 11月17日 22:52

**「背景」** 编码代理（如 Claude Code、Codex、Pi）会根据提示生成并执行代码。为了防止这些由 AI 生成的代码进行恶意操作或因提示注入导致破坏，通常需要在隔离环境中运行它们。外部沙箱模式将代理本身置于主机外部，而执行代码的环境通过独立的沙箱服务器提供，实现网络访问控制和凭证替换等安全措施。

**「影响」** 开发者现在可以将 Claude Code、Pi、Codex 等生成的代码通过这些沙箱安全执行，显著降低因代码错误或提示注入导致的系统破坏风险，并可在不泄露敏感凭证的前提下让代码访问外部服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/prime-radiant-inc/external-sandbox-container">GitHub - prime - radiant -inc/ external - sandbox -container: Python...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#sandboxing`, `#coding agents`, `#devtools`

---

<a id="item-tech-news-6"></a>
### [美国超大规模数据中心耗电约占全国 2%](https://arstechnica.com/science/2026/11/hyperscale-data-centers-use-2-of-us-electricity/) ⭐️ 8.0/10

一项研究统计了 2024 年 5 月至 2025 年 4 月期间美国 403 座超大规模数据中心的电力使用，估计总耗电量在 68 至 99 太瓦时之间，占全美用电量的 1.5%至 2.2%。这些设施从商业数据库的 675 座候选中筛选，平均电力容量约为 40 兆瓦。研究未能区分 AI 计算与传统数据服务的耗电，但提供了后续追踪的基准数据。

telegram · zaihuapd · 11月17日 12:54

**「超大规模数据中心概述」** 超大规模数据中心（hyperscale data centers）指容量通常在数十兆瓦以上、由云服务商和大型互联网公司运营的设施，提供云计算、存储和大模型训练等服务。此前的研究已指出，这类数据中心在美国整体电力消耗中占比约 1%‑2%，但缺乏统一的容量数据和时间范围的基准。

**「影响」** 该数据表明，超大规模数据中心对美国整体电网负荷贡献显著，能源规划者和企业在设计新设施或扩容时需将其电力需求纳入可持续性和成本评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arstechnica.com/science/2026/11/hyperscale-data-centers-use-2-of-us-electricity/">Hyperscale data centers use 2% of US electricity - Ars Technica</a></li>

</ul>
</details>

**标签**: `#data centers`, `#energy consumption`, `#computer systems`

---

<a id="item-tech-news-7"></a>
### [不同模型的最佳 Prompt Harness 评估](https://runta.com/blog/introducing-frontierharness-eval-v1-1/) ⭐️ 7.0/10

在 Hacker News 讨论中，作者对多种 Prompt Harness（包括系统提示、工具命名、上下文压缩等）在终端基准任务上的表现进行了对比测试。结果显示，不同模型对同一 Harness 的响应差异显著，约 64% 的算力花费用于未通过基准验证的任务。该讨论未伴随官方发布，仅提供了实验数据和对各模型适配最佳 Harness 的初步结论。

hackernews · Edward40 · 11月17日 14:53 · [社区讨论](https://news.ycombinator.com/item?id=50532191)

**「背景」** 在大语言模型（LLM）驱动的编码代理中，“harness”（提示套件）指的是围绕系统提示、工具名称、上下文压缩方式等的组合，用以引导模型完成任务。Runta 之前发布的 FrontierHarness Eval 1.0 只在单一模型上评估了多种 harness，以衡量其质量和成本；而在 2026 年 11 月推出的 v1.1 版对 5 种模型和 22 种 harness 进行交叉评测，共计 27,280 次运行，揭示了不同模型与 harness 之间的兼容性差异，并提供了成本、代币使用和延迟等指标的比较。

**「影响」** 开发者在部署 LLM 驱动的工具时，需要针对所使用的模型单独评估并选择最合适的 Harness，以避免大量算力浪费在无法通过基准验证的任务上。

**「社区讨论」** 评论者 krawczstef 认为，Harness 的差异主要来源于上下文工程细节，如果统一系统提示和工具名称，模型间的性能差异可能会大幅缩小。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://runta.com/blog/introducing-frontierharness-eval-v1-1/">Introducing FrontierHarness Eval v1.1 — RUNTA</a></li>
<li><a href="https://runta.com/blog/introducing-frontierharness-eval/">Introducing FrontierHarness Eval — RUNTA</a></li>

</ul>
</details>

**标签**: `#prompt engineering`, `#AI agents`, `#benchmarking`, `#software engineering`

---

<a id="item-tech-news-8"></a>
### [Anthropic 获准纳斯达克全球精选市场上市，代码 ANT](https://mp.weixin.qq.com/s/IkZCf2pJaAAXPJEpXnEBHQ) ⭐️ 7.0/10

Anthropic 已获准在纳斯达克全球精选市场以 A 类普通股上市，股票代码为 ANT。此批准仅表示公司满足纳斯达克上市条件，实际交易启动仍需完成招股说明书备案和首次公开发行（IPO）程序。该消息面向潜在投资者和行业观察者，标志着 Anthropic 从私有公司向公开交易公司转型的关键一步。

telegram · zaihuapd · 11月17日 13:00

**「背景」** Anthropic 为在纳斯达克全球精选市场上市，需要向美国证券交易委员会提交 Form S‑1 注册声明。该公司于 2026 年 10 月 26 日公开提交了 S‑1，披露了约 170 亿美元的第三季度收入、约 233 亿美元的净亏损以及 8950 亿美元的算力承诺，并首次公布了股票代码 ANT。完成此类注册是纳斯达克批准上市的前置条件。

**「影响」** 获批后，投资者可在 Nasdaq Global Select Market 通过代码 ANT 关注并在未来买卖 Anthropic 股票，需留意公司后续披露的 IPO 定价、发行规模及监管文件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ctrlmag.com/blog/anthropic-files-s-1-nasdaq-ticker-ant">Anthropic Files S-1 for Nasdaq Listing Under Ticker ANT</a></li>
<li><a href="https://cleus.ai/blog/anthropic-ipo-filing-s1-explained">Anthropic IPO Filing: $17B Revenue, $23B Loss... | Cleus Blog</a></li>

</ul>
</details>

**标签**: `#AI`, `#Business`, `#StockMarket`, `#Anthropic`

---

<a id="item-tech-news-9"></a>
### [Telegram 限制 Bot 与小程序只能使用 Stars 支付](https://telegram.me/zaihuapd/45189) ⭐️ 7.0/10

Telegram 官方通知称，依据苹果和谷歌的应用内购买规则，所有 Bot 和小程序内的数字商品只能通过 Telegram Stars 进行销售，包括 Bot 订阅、付费工具、第三方 AI 模型访问权限以及积分或代币。涉及加密货币交易的商品仅可使用 GRAM。自本周起平台将主动排查违规行为，违规者将被立即封禁且不再另行警告。此为已发布的政策要求，开发者需在上线前完成相应支付集成。

telegram · zaihuapd · 11月17日 14:46

**「Telegram Stars 支付要求背景」** Telegram Stars 是 Telegram 推出的内部虚拟货币，用于在 Telegram 应用内的 Bot 和小程序中购买数字商品和服务。根据 Telegram 官方文档，所有此类支付必须使用 Stars，以符合 Apple App Store 与 Google Play Store 的应用内购买政策。此前 Bot 可通过多种支付方式收款，但新规要求统一使用 Stars，违者将被封禁。

**「影响」** 开发者必须改用 Telegram Stars（或 GRAM）收款，否则其 Bot 或小程序将面临封禁，迫使其重新设计货币化流程并可能承担迁移成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://core.telegram.org/bots/payments-stars">Bot Payments API for Digital Goods and Services - Telegram APIs</a></li>

</ul>
</details>

**标签**: `#Telegram`, `#Payments`, `#Bots`, `#AI`

---

<a id="item-tech-news-10"></a>
### [可灵 AI 推出支持原生 8K 的 Kling Image 4.0 图像模型](https://mp.weixin.qq.com/s/p3_DIBRUUgmxShjD5Wp27w) ⭐️ 7.0/10

2026 年 11 月 17 日，可灵 AI 正式发布面向企业客户和开发者的 Kling Image 4.0 图像模型，并已全量上线。该模型首次原生支持 8K 分辨率图像生成，最高可接受 15000 个文本 token 输入，单张图像支持 2000 字排版并内置 70 余种商用字体。一次调用可生成最多 10 张风格统一的组图或超长画幅图像，且提供开放 API 接入。

telegram · zaihuapd · 11月18日 01:05

**「背景」** 文本到图像生成模型（如 Stable Diffusion 等）通过将自然语言描述转化为像素，实现自动图像创作；近年来这些模型已支持高分辨率输出，但多数仍受限于 4K 以下的分辨率或需要分块拼接。Kling Image 4.0 在此基础上采用统一的理解‑生成架构，提升了文本 token 上限至 15000，并首次实现原生 8K（7680×4320）图像生成，面向企业和开发者提供 API 接入。

**「影响」** 开发者可通过可灵 AI 的 API 直接生成 8K 超高清图像，省去后期放大步骤，适用于高质量广告、媒体和设计等场景，但需考虑更高的计算和带宽成本。

**标签**: `#image generation`, `#AI model`, `#API`, `#8K resolution`, `#software engineering`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [黄仁勋表态若董事会需要可重返英伟达 CEO](https://x.com/JensenHuang/status/2122726005219737649) ⭐️ 8.0/10

黄仁勋在离职后首次公开回应称，如董事会认为有利，他愿意重新担任英伟达 CEO，但董事会目前并未考虑重新聘用他。

telegram · zaihuapd · 11月17日 16:14

**「背景」** 黄仁勋因个人丑闻于上周突然辞去英伟达 CEO 职务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://edition.cnn.com/2026/11/17/business/jensen-huang-nvidia-ceo-statement">Jensen Huang says he would be ‘honored’ to be reinstated as Nvidia ...</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Leadership`, `#Corporate Governance`, `#Stock Market`

---

<a id="item-finance-news-2"></a>
### [工信部委托评估 17 家车企 60 天账期](http://www.caam.org.cn/chn/5/cate_68/con_5237404.html) ⭐️ 7.0/10

工信部委托中国汽车工业协会对 17 家重点车企进行供应商账款支付情况评估，核查其是否落实不超过 60 天的付款期限。

telegram · zaihuapd · 11月18日 01:15

**「背景」** 工信部此前已推动汽车行业实行不超过 60 天的供应商付款期限，以规范供应链资金流并防止拖欠。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://insidechinaauto.com/2025/06/14/chinese-automakers-make-60-day-supplier-payment-pledge-to-strengthen-supply-chain/">Chinese Automakers Make 60 - Day Supplier Payment Pledge To...</a></li>

</ul>
</details>

**标签**: `#automotive industry`, `#supplier payments`, `#regulatory policy`, `#China`

---