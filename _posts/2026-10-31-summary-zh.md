---
layout: default
title: "Horizon Summary: 2026-10-31 (ZH)"
date: 2026-10-31
lang: zh
---

> 从 35 条内容中筛选出 15 条重要资讯。

---

**科技新闻**
1. [Backdoor in Claude Code for VS Code extension on the Cursor Marketplace](#item-tech-news-1) ⭐️ 8.0/10
2. [Azure 五项跨租户漏洞导致完整租户泄露](#item-tech-news-2) ⭐️ 8.0/10
3. [Binance 63 亿美元被盗案仅用 20 分钟完成](#item-tech-news-3) ⭐️ 8.0/10
4. [Multi-Token Prediction Done Right \[R\]](#item-tech-news-4) ⭐️ 8.0/10
5. [Apple 智能功能 11 月 4 日在中国开启测试](#item-tech-news-5) ⭐️ 8.0/10
6. [Tangled 推出联邦代码托管平台](#item-tech-news-6) ⭐️ 7.0/10
7. [Show HN: A working Nintendo in ~1GB of Qwen weights](#item-tech-news-7) ⭐️ 7.0/10
8. [Bunny CDN Security Incident](#item-tech-news-8) ⭐️ 7.0/10
9. [AI 导致 SRE 技能退化而非取代](#item-tech-news-9) ⭐️ 7.0/10
10. [🤖 Claude 语音模式接入 🍏 苹果 CarPlay](#item-tech-news-10) ⭐️ 7.0/10
11. [百度网盘 iOS 摇一摇广告改用磁力计绕过运动权限](#item-tech-news-11) ⭐️ 7.0/10
12. [小米开源 0.8B 参数文档理解模型](#item-tech-news-12) ⭐️ 7.0/10

**财经新闻**
1. [Anthropic 成为 SpaceX 最大单一客户，每月贡献约 31 亿美元](#item-finance-news-1) ⭐️ 8.0/10
2. [证监会强调稳市场、深化投融资改革](#item-finance-news-2) ⭐️ 7.0/10
3. [日系车企在华产量跌至 2020 峰值的 40%以下](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Backdoor in Claude Code for VS Code extension on the Cursor Marketplace](https://phorion.io/blog/offical-claude-code-vsx-compromise/) ⭐️ 8.0/10

A tampered Claude Code VS Code extension on Cursor’s marketplace added a malicious SSH key to users’ authorized\_keys, prompting urgent security action.

hackernews · \_chall · 10月30日 07:09 · [社区讨论](https://news.ycombinator.com/item?id=50300683)

**标签**: `#security`, `#developer-tools`, `#AI-extensions`, `#VSCode`

---

<a id="item-tech-news-2"></a>
### [Azure 五项跨租户漏洞导致完整租户泄露](https://www.binarysecurity.no/posts/2026/10/one-root-case) ⭐️ 8.0/10

Azure 发现五个跨租户漏洞，攻击者可在不同租户之间实现完整的权限提升和数据泄露，影响使用 Azure AD 登录和资源管理的所有客户。

hackernews · swq115 · 10月30日 10:06 · [社区讨论](https://news.ycombinator.com/item?id=50301854)

**「背景」** Azure Logic Apps 中的 API Connections 采用了一个全局共享的内部架构，未在文档中公开，允许跨租户调用并可能泄露密钥、存储等资源。此前的博客（2025 年 3 月、2025 年 8 月以及 2026 年 2 月）已揭示了这些未记录的 API、其提升权限的机制以及一次完整的跨租户攻击示例。

**「影响」** 受影响的租户可能被其他租户完全接管，企业应立即审查 Azure AD 配置、监控异常登录并等待 Microsoft 发布修补或临时缓解措施。

**「社区讨论」** 一位评论者指出 login.microsoftonline.com/.../adminconsent 流程的回调地址可被伪造，只要攻击者知道目标租户 ID，即使文档警告不应使用该参数进行身份验证，仍可能被利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.binarysecurity.no/posts/2026/10/one-root-case">Azure&#x27;s Weakest Link - Five Full Cross-Tenant Compromises</a></li>
<li><a href="https://binarysecurity.no/posts/2025/08/azures-weakest-link-part2">Azure&#x27;s Weakest Link - Full Cross-Tenant Compromise</a></li>
<li><a href="https://www.binarysecurity.no/posts/2025/03/api-connections">Azure’s Weakest Link? How API Connections Spill Secrets</a></li>

</ul>
</details>

**标签**: `#azure`, `#cloud-security`, `#cross-tenant`, `#vulnerability`, `#software-engineering`

---

<a id="item-tech-news-3"></a>
### [Binance 63 亿美元被盗案仅用 20 分钟完成](https://www.wired.com/story/the-dollar63-billion-binance-hack-was-pulled-off-in-just-20-minutes/) ⭐️ 8.0/10

2026 年 10 月 30 日，报道指出全球最大加密货币交易所之一 Binance 在一次攻击中损失约 63 亿美元，黑客在约 20 分钟内完成了资金转移。该事件突显了加密平台热钱包管理和实时监控的薄弱环节，提醒业界即使是成熟交易所也可能在极短时间内遭受大规模资产窃取。

hackernews · domhudson · 10月30日 12:50 · [社区讨论](https://news.ycombinator.com/item?id=50303172)

**「背景概述」** Binance 是全球最大的加密货币交易所之一，过去已多次遭受大规模攻击。2026 年 10 月的 63 亿美元被盗事件利用了以太坊改进提案 EIP‑7702 中的合约部署权限漏洞，使攻击者能够在未经充分审计的智能合约中执行授权转账，并在约 20 分钟内跨链抽取多个区块链上的资产。

**「约 30 亿美元资产被冻结，币安承诺赔偿」** 币安在本次约 63 亿美元的被盗事件中已冻结约 30 亿美元的加密资产，并表示将对受影响用户的损失进行赔付，这将导致用户短期内无法提取这些资金并对市场流动性产生冲击。

**「社区讨论」** 评论者指出，虽然实际窃取只用了 20 分钟，但背后的策划与准备可能历时多年，说明此类攻击的成功更多依赖于长期的情报收集和漏洞积累，而非瞬时的技术突破。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cryptotimes.io/insights/binance-hack-explained/">Binance Hack Explained: How $ 6 . 3 Billion Was Drained in 20 Minutes</a></li>
<li><a href="https://www.wired.com/story/the-dollar63-billion-binance-hack-was-pulled-off-in-just-20-minutes/">The $ 6 . 3 Billion Binance Hack Was Pulled Off in Just 20 Minutes</a></li>
<li><a href="https://www.cnbc.com/2026/10/29/circle-tether-freeze-funds-impacted-by-potential-binance-security-issue.html">Binance hack: $6.3 billion impacted in record crypto theft - CNBC</a></li>

</ul>
</details>

**标签**: `#security`, `#cryptocurrency`, `#blockchain`, `#software‑engineering`

---

<a id="item-tech-news-4"></a>
### [Multi-Token Prediction Done Right \[R\]](https://www.reddit.com/r/MachineLearning/comments/1xjnz40/multitoken_prediction_done_right_r/) ⭐️ 8.0/10

A new paper presents a simple fix that extracts a useful KL gradient in Multi‑Token Prediction, promising better performance for language model training and decoding.

reddit · r/MachineLearning · /u/jayden\_teoh\_ · 10月30日 18:53

**标签**: `#Multi-Token Prediction`, `#Language Models`, `#Speculative Decoding`, `#Machine Learning Research`

---

<a id="item-tech-news-5"></a>
### [Apple 智能功能 11 月 4 日在中国开启测试](https://www.apple.com.cn/newsroom/2026/10/apple-intelligence-features-are-coming-to-users-in-china/) ⭐️ 8.0/10

Apple 宣布首批 Apple 智能功能将在 11 月 4 日随最新 iOS 开发者 Beta 版在中国开放测试，正式版计划随 iOS 27.3 于 12 月面向中国用户发布。功能包括实时翻译、照片消除工具和写作工具，均通过与阿里巴巴的千问大模型集成实现。仅对在中国购买或设备定位、Apple 账户地区设置为中国的 iPhone 用户开放，其他平台需待监管审批后推出。此次更新不包含下一代 Siri AI。

telegram · zaihuapd · 10月30日 21:44

**「背景」** Apple 在 2025 年启动的 “Apple Intelligence” 计划已将 AI 功能嵌入 iOS 系统，并在 iOS 27 中加入实时翻译、照片消除和写作等工具。此前，Apple 与阿里巴巴的千问（Qwen）大语言模型达成合作，将该模型用于 Siri、写作和视觉智能等功能，为本次在中国的功能测试提供技术支撑。

**「影响」** 符合条件的中国 iPhone 用户可提前体验 AI 翻译和内容生成等功能，开发者需在 iOS 27.3 正式版前适配这些 API，并关注后续监管审批对跨平台支持的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://parliamentnews.co.uk/qwen-mac-integration-apple-china-2026/">Qwen Mac Integration Brings Alibaba AI to Apple</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AI`, `#iOS`, `#China`, `#Machine Learning`

---

<a id="item-tech-news-6"></a>
### [Tangled 推出联邦代码托管平台](https://tangled.org/blog/forge/) ⭐️ 7.0/10

Tangled 正式发布了名为 Tangled Forge 的联邦代码托管平台，支持完整的自托管部署，并内置对 AT Protocol 的兼容。平台已上线组织（organization）功能，且在接下来数周内将推出私有仓库（private repo）支持。该服务旨在为开源项目和开发者提供去中心化的代码协作选项，能够与现有的 GitHub、GitLab 等平台互补。

hackernews · zlliang · 10月30日 15:44 · [社区讨论](https://news.ycombinator.com/item?id=50305573)

**「背景」** AT Protocol 是由 Bluesky 社区推出的去中心化社交协议，近年来被用于构建跨平台的身份和内容互操作。在此之前，芬兰初创公司 Tangled 已在 2026 年完成 380 万欧元种子轮融资，旨在打造去中心化的 Git 协作网络并提供欧洲版的 GitHub 替代方案。这些先前的融资和对去中心化协作的定位为本次推出支持自托管和 AT Protocol 的联邦代码锻造平台奠定了基础。

**「影响」** 开发者现在可以在自己的服务器上运行 Tangled Forge，利用 AT Protocol 实现跨实例的代码、发布和 CI 流程同步，从而降低对中心化平台的依赖；在私有仓库功能上线前，公开仓库已可直接使用。

**「社区讨论」** 有用户表示希望将目前在自托管 Gitea 上的项目迁移到 Tangled，以统一代码、发布和潜在的 CI，保持 GitHub 仅用于发现和备份；平台联合创始人则回应已稳定 AT Protocol 词表并简化了自托管流程，组织支持已上线，私有仓库即将推出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.vestbee.com/insights/articles/tangled-raises-3-8-m">Finnish startup Tangled raises € 3 . 8 M to reinvent code collaboration</a></li>

</ul>
</details>

**标签**: `#code collaboration`, `#federated systems`, `#open source`, `#dev tools`

---

<a id="item-tech-news-7"></a>
### [Show HN: A working Nintendo in ~1GB of Qwen weights](https://github.com/dbreunig/nesformer) ⭐️ 7.0/10

A hack shows an NES emulator built from ~1 GB of Qwen LLM weights, highlighting creative but currently niche applications of LLMs in system emulation.

hackernews · dbreunig · 10月30日 16:40 · [社区讨论](https://news.ycombinator.com/item?id=50306442)

**标签**: `#LLM`, `#emulation`, `#hardware`, `#software engineering`, `#open source`

---

<a id="item-tech-news-8"></a>
### [Bunny CDN Security Incident](https://status.bunny.net/incidents/p6gf1by9kr7m) ⭐️ 7.0/10

Bunny CDN disclosed a security incident involving a compromised third‑party provider, prompting rapid traffic rerouting and certificate re‑issuance.

hackernews · SondreDag · 10月30日 19:05 · [社区讨论](https://news.ycombinator.com/item?id=50308697)

**标签**: `#CDN`, `#Security`, `#Infrastructure`, `#TLS`

---

<a id="item-tech-news-9"></a>
### [AI 导致 SRE 技能退化而非取代](https://newsletter.signoz.io/p/ai-isnt-replacing-sres-its-deskilling) ⭐️ 7.0/10

在近期的讨论中，作者指出 AI 并未取代站点可靠性工程师（SRE），而是通过自动化处理日志分析、云资源查询等日常任务，使 SRE 的实际操作经验逐渐下降。评论中提到，AI 代理已经能够以超人速度使用 AWS CLI 等工具，导致人类工程师难以保持同等水平的手动技能。

hackernews · dorianniemiec · 10月30日 15:52 · [社区讨论](https://news.ycombinator.com/item?id=50305693)

**「AI SRE 概念概述」** AI SRE（AI‑powered Site Reliability Engineering）是指使用人工智能代理在生产系统中自动完成监控、告警分流、根因分析、事后报告和引导修复等核心可靠性任务，而不是仅依赖预设的“if X then Y”脚本。该概念在 2025‑2026 年已被多篇行业指南阐述，标志着 SRE 工作正被 AI 自动化所渗透。

**「影响」** 组织可能需要刻意保留部分故障或手动操作作为练习，以防止团队在长期依赖 AI 后失去关键的故障排查和系统理解能力。

**「社区讨论」** 一位评论者将此类做法类比航空业的手动飞行要求，主张保留人工处理的机会；另一位则指出 Terraform 已导致基础设施配置技能退化，认为应在 AI 辅助的同时继续培养人工检测和恢复能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.augmentcode.com/guides/ai-sre-ai-powered-site-reliability-engineering">AI SRE: The 2026 Guide to AI-Powered Site Reliability Engineering</a></li>
<li><a href="https://dev.to/siddharth_singh_409bd5267/ai-sre-the-complete-guide-for-engineering-teams-in-2026-51ba">AI SRE: The Complete Guide for Engineering Teams in 2026</a></li>
<li><a href="https://wetheflywheel.com/en/guides/what-is-ai-sre/">What is AI SRE? The Complete Guide to AI-Powered Site ...</a></li>

</ul>
</details>

**标签**: `#SRE`, `#AI`, `#DevOps`, `#Automation`

---

<a id="item-tech-news-10"></a>
### [🤖 Claude 语音模式接入 🍏 苹果 CarPlay](https://www.macrumors.com/2026/09/04/anthropics-claude-is-coming-to-carplay/) ⭐️ 7.0/10

Claude’s voice mode now supports Apple CarPlay, expanding AI assistant capabilities in vehicles.

telegram · zaihuapd · 10月30日 07:25

**标签**: `#AI assistants`, `#CarPlay`, `#Anthropic`, `#voice interaction`

---

<a id="item-tech-news-11"></a>
### [百度网盘 iOS 摇一摇广告改用磁力计绕过运动权限](https://www.landian.news/archives/127843.html) ⭐️ 7.0/10

百度网盘 iOS 版 13.36.0 将摇一摇广告的触发逻辑从 CoreMotion 换成 Core Location 的 CLHeading，读取磁力计数据判断手机晃动（内部代号 NoShake）。该实现绕过了对陀螺仪和加速度计的权限检查，即使用户关闭运动传感器权限，仍会在约 1 秒的特定参数等待后自动触发广告点击。

telegram · zaihuapd · 10月30日 15:00

**「磁力计与 iOS 摇一摇广告的技术背景」** 在 iOS 中，访问加速度计和陀螺仪等运动传感器需要 CoreMotion 框架并获得用户的运动权限；而磁力计（用于指南针）则通过 Core Location 的 CLHeading 接口在获取位置权限后即可读取。此前，Apple 曾在 2023 年提醒中国开发者避免使用陀螺仪实现的摇一摇广告，以规避平台政策（见 Grokipedia 报道）。因此，百度网盘改用磁力计来判断手机晃动，能够在用户拒绝运动权限后仍触发广告跳转。

**「影响」** 此做法让广告能够在用户拒绝运动传感器授权的情况下仍然触发，增加了隐私泄露风险，并提示 iOS 开发者和审查机构需将磁力计视为可能的运动感知渠道，以防止类似的权限规避。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Shake_advertisement">Shake advertisement — Grokipedia</a></li>
<li><a href="https://www.fluxmagnetometer.com/blog/what-is-a-magnetometer-and-how-does-it-work">What Is a Magnetometer? How Your iPhone Detects Magnetic ...</a></li>

</ul>
</details>

**标签**: `#iOS`, `#privacy`, `#ad-tech`, `#mobile-security`

---

<a id="item-tech-news-12"></a>
### [小米开源 0.8B 参数文档理解模型](https://x.com/XiaomiTech_/status/2116154468358316380) ⭐️ 7.0/10

Xiaomi open‑sourced a 0.8B OCR/document‑understanding model, offering a lightweight, high‑performing tool for the community.

telegram · zaihuapd · 10月30日 16:00

**标签**: `#document-understanding`, `#open-source`, `#OCR`, `#machine-learning`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Anthropic 成为 SpaceX 最大单一客户，每月贡献约 31 亿美元](https://www.cls.cn/detail/2519914) ⭐️ 8.0/10

Anthropic 将成为 SpaceX 最大单一客户，合同最高支出 1205 亿美元，等同于自 2024 年 12 月起每月约 31 亿美元收入，占 SpaceX 上季度营收约 34.5%。

telegram · zaihuapd · 10月30日 06:20

**「背景」** SpaceX 在 2024 年设立了名为 Super Intelligence 的 AI 计算部门，并在其 2026 年的 IPO 文件中披露，Anthropic 同意在 2026‑2029 年间为该部门支付最高 1205 亿美元的算力费用，约合每月 31 亿美元。

**「影响」** SpaceX 约三分之一的收入来自 Anthropic，导致公司对单一客户的依赖加大，投资者面临收入波动风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/ai/articles/anthropic-discloses-120-5-billion-140613686.html?fr=sycsrp_catchall">Anthropic discloses up to $120.5 billion in SpaceX compute ... Anthropic’s IPO Filing Reveals Up to $120.5 Billion in ... Anthropic Reveals It Will Pay SpaceX Up to $120.5B for AI Compute IPO BOMBSHELL: Anthropic Discloses $120.5B in Computing ... Anthropic to Pay SpaceX Up to $120.5B for AI Compute Through 2029 Anthropic to Pay SpaceXAI Up to $120.5B for Nvidia Compute Anthropic agrees to spend up to $120.5 billion on SpaceX ...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/spacex-relies-anthropic-third-revenue-184410766.html?fr=sycsrp_catchall">SpaceX Relies on Anthropic for a Third of Its Revenue</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/anthropic-accounts-over-third-spacex-014451805.html?fr=sycsrp_catchall">Anthropic accounts for over a third of SpaceX revenue in Q3 ...</a></li>
<li><a href="https://completeaitraining.com/news/anthropic-generated-345-of-spacex-quarterly-revenue/">Anthropic Generated 34.5% of SpaceX Quarterly Revenue</a></li>

</ul>
</details>

**标签**: `#AI compute`, `#SpaceX`, `#Anthropic`, `#Corporate partnership`, `#Revenue impact`

---

<a id="item-finance-news-2"></a>
### [证监会强调稳市场、深化投融资改革](https://view.inews.qq.com/k/20261030A0ASEC00?scene=wap&amp;amp;no-redirect=1) ⭐️ 7.0/10

证监会党委书记吴清于 10 月 30 日主持党委（扩大）会议，要求全力稳市场、稳预期并深化投融资综合改革，以提升资本市场韧性和信心。

telegram · zaihuapd · 10月30日 10:00

**「背景」** 此前，中国证监会在 2026 年 1 月已承诺把维护资本市场稳定、防止大幅波动作为全年核心任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://english.www.gov.cn/news/202601/16/content_WS696a4287c6d00ca5f9a089f4.html">China&#x27;s securities regulator stresses market stability in ...</a></li>

</ul>
</details>

**标签**: `#China`, `#Regulation`, `#Capital Markets`, `#Policy`

---

<a id="item-finance-news-3"></a>
### [日系车企在华产量跌至 2020 峰值的 40%以下](https://weibo.com/1642634100/Rp6qUwLKa) ⭐️ 7.0/10

2026 年 4 月至 9 月，丰田、本田、日产和马自达在华合计产量约 102 万辆，同比下降 32%，仅为 2020 年同期峰值的约 40%。

telegram · zaihuapd · 10月30日 13:38

**「背景说明」** 2020 年是这四家日系车企在华产量的最高点，随后因需求放缓和行业环境变化，产量逐步下滑至 2026 年 4‑9 月的约 40%。

**标签**: `#automotive`, `#China`, `#Japanese manufacturers`, `#production decline`

---