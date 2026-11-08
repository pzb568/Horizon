---
layout: default
title: "Horizon Summary: 2026-11-08 (ZH)"
date: 2026-11-08
lang: zh
---

> 从 39 条内容中筛选出 15 条重要资讯。

---

**科技新闻**
1. [Claude Code&\#x27;s &quot;Don&\#x27;t Ask Again&quot; exposes passwords in 1,122 public GitHub files](#item-tech-news-1) ⭐️ 8.0/10
2. [MaxxBench – &quot;Nice DeepSWE score. But is it true?&quot;](#item-tech-news-2) ⭐️ 8.0/10
3. [GitHub 新 Rubicon 架构实现每秒 7200 次推送](#item-tech-news-3) ⭐️ 8.0/10
4. [The end of Microsoft Research&\#x27;s AI Frontiers group](#item-tech-news-4) ⭐️ 7.0/10
5. [Windows 11 应用应放弃 Electron，Discord 示例揭示高内存问题](#item-tech-news-5) ⭐️ 7.0/10
6. [Asahi Linux 7.3 进展报告：Fedora Asahi Remix 同日发布，USB‑C 显示支持仍待完善](#item-tech-news-6) ⭐️ 7.0/10
7. [We Visited China’s Stargate in Inner Mongolia](#item-tech-news-7) ⭐️ 7.0/10
8. [微软逐步终止租用甲骨文 AI 算力协议](#item-tech-news-8) ⭐️ 7.0/10
9. [🍏 苹果称 iPhone Duo 适配应用已超 10 万个](#item-tech-news-9) ⭐️ 7.0/10
10. [特斯拉 Optimus 机器人或仅提供租赁](#item-tech-news-10) ⭐️ 7.0/10
11. [Claude Code 网页搜索可能泄露登录邮箱](#item-tech-news-11) ⭐️ 7.0/10
12. [🤖 Claude Max 用量宣传被诉，Anthropic 被判决须应诉](#item-tech-news-12) ⭐️ 7.0/10
13. [苹果发布 HALO 人形机器人系统，使用两款千问模型](#item-tech-news-13) ⭐️ 7.0/10
14. [美民主党议员呼吁立法禁 AI 递归自我改进](#item-tech-news-14) ⭐️ 7.0/10

**财经新闻**
1. [软银与 ABB 计划拆分中国机器人业务以挽救被叫停的收购](#item-finance-news-1) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Claude Code&\#x27;s &quot;Don&\#x27;t Ask Again&quot; exposes passwords in 1,122 public GitHub files](https://apiiro.com/blog/coding-agents-leaking-secrets-github-dont-ask-again) ⭐️ 8.0/10

Claude Code’s “Don’t Ask Again” feature can expose secrets if local settings are committed, underscoring AI‑assistant security concerns.

hackernews · shmulc · 11月7日 20:45 · [社区讨论](https://news.ycombinator.com/item?id=50407882)

**标签**: `#AI coding assistants`, `#secret leakage`, `#software security`, `#GitHub`, `#developer tooling`

---

<a id="item-tech-news-2"></a>
### [MaxxBench – &quot;Nice DeepSWE score. But is it true?&quot;](https://maxxbench.unlap.ai/research/why-maxxbench/) ⭐️ 8.0/10

A Hacker News debate examines the validity of MaxxBench&\#x27;s DeepSWE scores, raising broader questions about LLM benchmark trustworthiness.

hackernews · antiuniverse · 11月7日 17:19 · [社区讨论](https://news.ycombinator.com/item?id=50406222)

**标签**: `#benchmarks`, `#LLM evaluation`, `#AI research`

---

<a id="item-tech-news-3"></a>
### [GitHub 新 Rubicon 架构实现每秒 7200 次推送](https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/) ⭐️ 8.0/10

GitHub 在限量私有预览中推出代号 Rubicon 的新 Git 存储架构，将 Git 对象存入 Azure Blob Storage，并使用 Ref‑CAS 与虚拟副本管理读写。内部测试显示，该架构可支持约 5000 个 AI 智能体并发协作，最高每秒处理 7200 次推送，且读取延迟保持在较低水平。

telegram · zaihuapd · 11月7日 14:12

**「背景」** Git 传统上将仓库对象以 pack 文件形式存放在本地磁盘上，引用信息与对象数据耦合，导致在高并发写入场景下协调成本较高。Rubicon 将 Git 对象迁移至 Azure Blob Storage，并使用独立的 Ref‑CAS（Reference Compare‑and‑Swap）日志服务来管理引用和 pack 清单，从而实现存储与计算分离、降低组件间协调，为大规模 AI 智能体并发推送提供基础。

**「影响」** 对需要高并发推送的 AI‑驱动工作流或大规模仓库的组织而言，加入 Rubicon 预览可显著降低推送瓶颈；但目前仅限私有预览，需向 GitHub 申请访问并在后续公开推广后再行部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/">Inside GitHub’s new Git storage architecture - The GitHub Blog</a></li>

</ul>
</details>

**标签**: `#GitHub`, `#Infrastructure`, `#AI tooling`

---

<a id="item-tech-news-4"></a>
### [The end of Microsoft Research&\#x27;s AI Frontiers group](https://hunch.net/?p=13764006) ⭐️ 7.0/10

Microsoft Research is ending its AI Frontiers group, signaling a strategic move toward transformer‑centric scaling over exploratory AI research.

hackernews · srean · 11月7日 18:02 · [社区讨论](https://news.ycombinator.com/item?id=50406563)

**标签**: `#Microsoft Research`, `#AI research strategy`, `#industry trends`

---

<a id="item-tech-news-5"></a>
### [Windows 11 应用应放弃 Electron，Discord 示例揭示高内存问题](https://www.windowslatest.com/2026/11/06/every-windows-11-app-should-kill-electron-and-discord-just-showed-why-no-starting-screen-and-70-less-ram-even-with-two-accounts-signed-in/) ⭐️ 7.0/10

Discord 在 Windows 11 上启动时出现无启动画面，并在两个账户同时登录的情况下仍比预期多占用约 70% 的内存，暴露了 Electron 框架在该系统上的高 RAM 消耗。文章指出，这种资源浪费对普通用户和开发者都是显著的性能瓶颈。

hackernews · thunderbong · 11月7日 11:11 · [社区讨论](https://news.ycombinator.com/item?id=50403507)

**「背景」** Electron 是一个将 Chromium 浏览器内核和 Node.js 运行时打包在一起的跨平台桌面应用框架，因其一次开发即可在 Windows、macOS、Linux 上运行而被广泛采用，但也因同时加载完整的浏览器进程而导致显著的内存占用。Discord 过去的桌面客户端正是基于 Electron，启动时会出现长时间的“Starting”界面并消耗数 GB 的 RAM。近期 Discord 的联合创始人兼 CTO 展示了全新用 Rust 重写的客户端（内部代号 Discord Phoenix），该客户端在 Windows 11 上冷启动即完成加载，并在同时登录两个账号时仅使用约 290 MB RAM，约比 Electron 版省去 70% 以上的内存，这一对比成为本文批评 Electron 在 Windows 11 上性能表现的核心依据。

**「影响」** 开发者在为 Windows 11 构建桌面应用时，可能需要重新评估使用 Electron 的成本，转而考虑更轻量的本地 GUI 框架或 Rust 等低内存占用的替代方案，以避免类似的内存膨胀。

**「社区讨论」** 评论者 cheschire 提到，Electron 的高内存问题自早期就已被广泛认知，甚至在 VS Code 首发时就受到批评，文章并未提供新的解决思路。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.windowslatest.com/2026/11/06/every-windows-11-app-should-kill-electron-and-discord-just-showed-why-no-starting-screen-and-70-less-ram-even-with-two-accounts-signed-in/">Every Windows 11 app should kill Electron, and Discord just ...</a></li>
<li><a href="https://todayforai.com/en/items/art-5eb62195-e80">Discord Rewrites Client in Rust, Beating Electron on Cold ...</a></li>
<li><a href="https://undercodenews.com/discords-new-rust-based-client-is-shockingly-fast-uses-70-less-ram-and-could-make-whatsapp-and-teams-look-outdated/">Discord&#x27;s New Rust-Based Client Is Shockingly Fast, Uses 70% ...</a></li>

</ul>
</details>

**标签**: `#electron`, `#windows-11`, `#desktop-app-development`, `#performance`

---

<a id="item-tech-news-6"></a>
### [Asahi Linux 7.3 进展报告：Fedora Asahi Remix 同日发布，USB‑C 显示支持仍待完善](https://asahilinux.org/2026/11/progress-report-7-3/) ⭐️ 7.0/10

Asahi Linux 7.3 的进展报告指出，Fedora 45 于 11 月 3 日发布的同一天，Fedora Asahi Remix 也同步发布，实现了首次与上游 Fedora 同步发布。报告同时说明，Apple Silicon 设备的硬件支持仍在推进，尤其是对 USB‑C 外接显示器的支持仍未完成。

hackernews · ackyshake · 11月7日 05:20 · [社区讨论](https://news.ycombinator.com/item?id=50401867)

**「背景」** Asahi Linux 是一个将上游 Linux 内核移植到 Apple Silicon（M1、M2、M3 系列）上的开源项目，依赖社区向主线内核提交驱动和平台代码。自 Linux 7.3 内核于 2026 年发布后，项目已上游了 macaudio 与 avd 等关键驱动，并在其下游发行版 Fedora Asahi Remix 中同步发布，首次实现与 Fedora 45 同日上线。

**「影响」** 开发者和用户现在可以在同一天获取基于 Fedora 45 的 Asahi Remix，简化了安装和测试流程，但缺乏 USB‑C 显示支持仍限制了在 MacBook Air 等设备上使用外部显示器的场景。

**「社区讨论」** 社区评论中，用户 alentred 表示 USB‑C 显示器支持是其使用 Asahi Linux 的关键阻碍，认为该功能的优先级应提升，以满足需要外接显示的用户需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://asahilinux.org/2026/11/progress-report-7-3/">Progress Report: Linux 7.3 - Asahi Linux</a></li>
<li><a href="https://asahilinux.org/2026/11/progress-report-7-3/">Progress Report: Linux 7.3 - Asahi Linux</a></li>

</ul>
</details>

**标签**: `#Linux`, `#Apple Silicon`, `#Open Source`, `#Operating Systems`

---

<a id="item-tech-news-7"></a>
### [We Visited China’s Stargate in Inner Mongolia](https://newsletter.semianalysis.com/p/we-visited-chinas-stargate-in-inner) ⭐️ 7.0/10

The piece reports on a massive Chinese AI datacenter, highlighting its scale, cost efficiency, and strategic significance.

rss · Semianalysis · 11月7日 19:01

**标签**: `#AI infrastructure`, `#datacenters`, `#China`, `#compute scaling`

---

<a id="item-tech-news-8"></a>
### [微软逐步终止租用甲骨文 AI 算力协议](https://www.bloomberg.com/news/articles/2026-11-06/microsoft-is-winding-down-oracle-deal-to-rent-ai-cloud-capacity) ⭐️ 7.0/10

微软正逐步终止自 2023 年起与甲骨文的 AI 算力租用协议，近几个月未续签合同，导致甲骨文股价一度下跌约 3%。甲骨文提供的硬件基于老一代英伟达芯片，已不符合微软的需求。

telegram · zaihuapd · 11月7日 02:00

**「微软与甲骨文的 AI 计算租赁协议概述」** 2023 年，微软宣布与竞争对手甲骨文签署租用 GPU 算力的协议，利用甲骨文数据中心的英伟达芯片为新版 Bing 的生成式 AI 提供计算支持。当时业界将此视为因全球 AI 计算资源紧缺而出现的罕见跨云合作。

**「影响」** 随着协议结束，甲骨文将失去来自微软的 AI 计算租金收入，可能进一步削弱其在高端 AI 基础设施市场的竞争力；微软则需转向自建或其他云供应商以满足其 AI 计算需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.zerohedge.com/markets/microsoft-pulls-plug-oracle-ai-rental-post-election-data-center-fallout-spreads">Microsoft Pulls The Plug On Oracle AI Rental As... | ZeroHedge</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#Oracle`, `#AI compute`, `#Cloud infrastructure`, `#Hardware`

---

<a id="item-tech-news-9"></a>
### [🍏 苹果称 iPhone Duo 适配应用已超 10 万个](https://9to5mac.com/2026/11/06/apple-says-there-are-already-over-100000-apps-built-for-iphone-duo/) ⭐️ 7.0/10

Apple reports over 100,000 apps adapted for the iPhone Duo, indicating rapid developer adoption.

telegram · zaihuapd · 11月7日 02:30

**标签**: `#iPhone Duo`, `#App Store`, `#Mobile Development`

---

<a id="item-tech-news-10"></a>
### [特斯拉 Optimus 机器人或仅提供租赁](https://www.ithome.com/1/023/675.htm) ⭐️ 7.0/10

埃隆·马斯克在巴伦投资大会上透露，特斯拉的 Optimus 人形机器人可能只以租赁方式提供，具体租金和可完成的工作尚未公布。单台机器的初期制造成本约为 3 万美元，目标降至 2 万美元，且生产效率据称是普通人类的 5 倍。该机器人已于今年 10 月在弗里蒙特工厂启动早期生产，计划年产能达 100 万台，但要实现全面生产速度仍需至少一年，预计将在 2027 年底左右开始对外交付。

telegram · zaihuapd · 11月7日 06:33

**「Optimus 机器人的前期研发与生产概况」** Optimus 是特斯拉研发的类人形机器人，首次在 2021 年的 AI 日上公开概念，并在随后几年展示了原型机和功能演示。2023 年特斯拉宣布将进入小批量试产，随后在 2024 年展示了第二代（Gen 2）机型的改进，包括更轻的结构和更快的步态。2025 年 10 月，特斯拉在弗里蒙特工厂启动了早期生产，目标年产能约 100 万台，计划在 2027 年底前实现大规模交付。

**「影响」** 如果 Optimus 仅以租赁形式提供，企业和机构在采用该机器人时将面临运营支出而非一次性资本支出，需要评估租赁费用与工作产出之间的成本效益，并可能促使特斯拉建立专门的维护和服务网络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://interestingengineering.com/ai-robotics/tesla-optimus-robot-enters-production">Tesla Optimus production starts as Musk targets 20,000 robots weekly</a></li>

</ul>
</details>

**标签**: `#robotics`, `#AI`, `#hardware`, `#industry-news`

---

<a id="item-tech-news-11"></a>
### [Claude Code 网页搜索可能泄露登录邮箱](https://github.com/anthropics/claude-code/issues/107757) ⭐️ 7.0/10

Anthropic 的 Claude Code 在执行联网搜索时，会把用户登录邮箱写入请求体，导致邮箱被发送至外部站点，如 Wikipedia 和美国证券交易委员会。该问题自 2024 年 7 月被报告，2.1.317 版本已加入拦截措施，但可被自定义 Python 脚本绕过。Anthropic 表示将在下一版本中彻底移除上下文中的登录邮箱。

telegram · zaihuapd · 11月7日 08:09

**「背景」** Claude Code 是 Anthropic 推出的具备联网搜索功能的代码助手。为了解决模型在生成代码时错误填入作者姓名的问题，开发团队在 2025 年将登录邮箱加入模型上下文，结果导致在访问需要联系信息的站点时，Claude Code 会在 HTTP 请求的 User‑Agent 或其他头部中自动携带用户的实际邮箱，从而被发送至 Wikipedia、美国证券交易委员会等外部网站。该问题最早于 2024 年 7 月被报告，随后在 2026 年 2.1.317 版加入拦截，但仍可被自定义 Python 脚本绕过。

**「影响」** 受影响的开发者可能会因邮箱泄露而收到大量诈骗邮件，建议尽快升级到已加入拦截的 2.1.317 版或等待下个版本的修复。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gate.com/news/detail/claude-code-automatically-leaks-user-email-to-wikipedia-sec-anthropic-25467614">Claude Code Automatically Leaks User Email to Wikipedia, SEC ...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#privacy`, `#Claude Code`, `#software engineering`

---

<a id="item-tech-news-12"></a>
### [🤖 Claude Max 用量宣传被诉，Anthropic 被判决须应诉](https://thenextweb.com/news/anthropic-claude-max-lawsuit-ruling-usage-claims) ⭐️ 7.0/10

Anthropic must respond to claims that its Claude Max pricing was misleading, a notable legal development for the AI industry.

telegram · zaihuapd · 11月7日 12:44

**标签**: `#AI`, `#Legal`, `#Anthropic`, `#Pricing`

---

<a id="item-tech-news-13"></a>
### [苹果发布 HALO 人形机器人系统，使用两款千问模型](https://weibo.com/1642634100/RqjjGllvw) ⭐️ 7.0/10

苹果研究团队于 2026 年 11 月 4 日在 arXiv 上发布论文，披露了名为 HALO 的三层人形机器人自主控制系统，并在宇树 G1 机器人上实现了从仿真到真实房间的动作迁移。系统上层使用千问 Qwen3.6-35B-A3B 进行任务编排，中层采用千问 Qwen3.5-2B 生成具体动作，底层则是经强化学习训练的动作跟踪器。研究团队已公开数据生成、模型训练与部署代码，属于研究预印本阶段，尚未商业化。

telegram · zaihuapd · 11月7日 13:35

**「背景」** HALO 系统在仿真环境中生成 egocentric 视觉‑语言‑动作数据，并通过强化学习训练的动作跟踪器将这些动作迁移到真实的 Unitree G1 人形机器人上，实现了从未见过的房间中执行任务的能力。该工作基于近期在仿真到实物（sim‑to‑real）迁移和大语言模型用于任务编排与动作生成的研究趋势。

**「影响」** 开放的代码和模型使得机器人研究者能够直接复现并扩展 HALO 的仿真‑实境迁移流程，加速基于大语言模型的机器人任务规划与运动生成的实验与应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2611.06908">Perceptive Humanoid Motion from Simulation - arXiv.org</a></li>
<li><a href="https://www.c114pro.com/ainews/210857.html">Apple Reveals Progress on HALO Robot: Validated on Unitree G1 ...</a></li>

</ul>
</details>

**标签**: `#robotics`, `#large-language-models`, `#reinforcement-learning`, `#Apple`

---

<a id="item-tech-news-14"></a>
### [美民主党议员呼吁立法禁 AI 递归自我改进](https://x.com/AlexBores/status/2118494668769878037) ⭐️ 7.0/10

美国民主党议员 Alex Bores 于本月在社交媒体上呼吁国会在今年通过立法，禁止 AI 的递归自我改进（RSI），即让 AI 自动设计并部署下一代 AI 系统。他引用 OpenAI 计划在 2028 年 3 月实现“自动化 AI 研究员”目标，以及 Anthropic 员工预测 2027 年底 AI 将承担约 80% 的前沿模型开发工作，认为这些趋势放大了错误和对齐偏差的风险。Bores 还提到 METR 报告显示 AI 研发速度在加速，主张禁令“刻不容缓”。该提议目前仅为立法呼吁，尚未形成法律。

telegram · zaihuapd · 11月8日 01:30

**「背景」** 递归自我改进（RSI）指 AI 系统能够自行设计、训练并部署下一代更强的 AI，进而形成潜在的指数式能力提升。2026 年 OpenAI 已公开承诺将在 2028 年 3 月实现“自动化 AI 研究员”，即让 AI 与人类研究者并行完成研究任务；Anthropic 亦预测到 2027 年底，其 Claude 系统将承担约 80% 的前沿模型开发工作。这些计划显示业界已在向能够自行迭代的 AI 迈进，为立法者提出的 RSI 禁令提供了具体的技术背景。

**「影响」** 如果相关立法通过，AI 研发机构将被迫停止或限制任何涉及自动化模型生成的项目，可能导致研发进度放缓并增加合规成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/built-to-benefit-everyone-our-plan/">Built to benefit everyone: our plan - OpenAI</a></li>
<li><a href="https://cryptobriefing.com/anthropic-claude-lead-frontier-model-training-2027/">Anthropic projects Claude will lead 80-90% of frontier model ...</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#AI safety`, `#Legislation`, `#Recursive self‑improvement`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [软银与 ABB 计划拆分中国机器人业务以挽救被叫停的收购](https://www.bloomberg.com/news/articles/2026-11-07/softbank-abb-weigh-china-carve-out-to-salvage-robotics-deal) ⭐️ 8.0/10

软银与 ABB 正考虑将 ABB 在华机器人业务拆分为独立实体，以挽救被中国监管叫停的 54 亿美元收购。

telegram · zaihuapd · 11月7日 11:24

**「交易被中国监管阻止」** 此前，中国外商投资安全审查工作机制办公室已叫停软银收购 ABB 机器人业务的 54 亿美元跨境并购。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reuters.com/business/media-telecom/softbank-abb-explore-china-carve-out-salvage-robotics-deal-bloomberg-news-2026-11-07/">SoftBank, ABB explore China carve-out to salvage robotics ...</a></li>

</ul>
</details>

**标签**: `#Mergers &amp; Acquisitions`, `#Robotics`, `#China Policy`, `#SoftBank`, `#ABB`

---