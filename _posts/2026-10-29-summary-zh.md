---
layout: default
title: "Horizon Summary: 2026-10-29 (ZH)"
date: 2026-10-29
lang: zh
---

> 从 38 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [Apple&\#x27;s git still trusts the compromised eMudhra certificates](#item-tech-news-1) ⭐️ 8.0/10
2. [Google 推出 Gemini 4 Carbon 大模型](#item-tech-news-2) ⭐️ 8.0/10
3. [Dayjob: Tax 评估 AI 代理在 50 项专业税务任务中的表现](#item-tech-news-3) ⭐️ 8.0/10
4. [GitHub Octoverse 2026](#item-tech-news-4) ⭐️ 8.0/10
5. [ChatGPT 推出 iCloud 邮件与日历插件](#item-tech-news-5) ⭐️ 8.0/10
6. [长鑫存储计划限量量产 HBM3E，良率仅 20‑30%](#item-tech-news-6) ⭐️ 8.0/10
7. [MacBook Pro with PROLED XDR Display and Touch](#item-tech-news-7) ⭐️ 7.0/10
8. [How Much Does the Hint Matter? A generic feedback line matches self-written critiques in hindsight self-distillation \(ACM ICAIF &\#x27;26\) \[R\]](#item-tech-news-8) ⭐️ 7.0/10
9. [Discord 公开服务器对话将可被网络搜索](#item-tech-news-9) ⭐️ 7.0/10
10. [韩国罚苹果 1550 万、谷歌 3200 万美元](#item-tech-news-10) ⭐️ 7.0/10
11. [ChatGPT Pro 与 Business 用户每月最高 500 美元 API 额度](#item-tech-news-11) ⭐️ 7.0/10
12. [Google 将 AI 模式搜索广告扩展至全球](#item-tech-news-12) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Apple&\#x27;s git still trusts the compromised eMudhra certificates](https://emudhra.we-have-a-problem.com/apple.html) ⭐️ 8.0/10

Apple’s macOS utilities still trust compromised eMudhra certificates, requiring urgent patches for developers.

hackernews · galadran · 10月28日 11:03 · [社区讨论](https://news.ycombinator.com/item?id=50271640)

**标签**: `#security`, `#macOS`, `#git`, `#certificates`, `#devops`

---

<a id="item-tech-news-2"></a>
### [Google 推出 Gemini 4 Carbon 大模型](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/) ⭐️ 8.0/10

Google 于 2026 年 10 月发布 Gemini 4 Carbon，定位为其最强的前沿大模型，专注网络安全与长时程任务。相较于前代 Argon，安全代码生成成功率提升超过 2 倍，幻觉和高严重性错位警报下降约 80%，在 SEC‑bench Pro 基准上取得 88.2% 的得分。该模型以每输入 1 万 token 2 美元、每输出 1 万 token 10 美元的引入价向部分网络安全防御者、可信合作伙伴（含美国政府预发布测试）开放，后续将逐步面向开发者、企业和消费者提供。

hackernews · acossta · 10月28日 17:01 · [社区讨论](https://news.ycombinator.com/item?id=50276792)

**「背景说明」** Gemini 4 Carbon 是 Google Gemini 系列的最新大模型，继承并升级了前代 Gemini 4 Argon 的能力。该系列模型旨在提升在长时程任务（如多步工程问题、代码库漏洞定位与修复）以及网络安全基准上的表现，并采用与 Argon 相同的按 token 计费模式。

**「影响」** 安全团队可利用 Gemini 4 Carbon 实现多天自主的漏洞定位与修复、系统调试等复杂工程任务，但需先通过 Google 的受限合作伙伴计划才能获取访问权限。

**「社区讨论」** 部分用户报告实际吞吐量远低于官方宣称的约 100 tps，实际测得不到 30 tps，并质疑在模型未正式发布前公开的基准成绩的可信度。

**标签**: `#AI models`, `#large language models`, `#Google Gemini`, `#machine learning`

---

<a id="item-tech-news-3"></a>
### [Dayjob: Tax 评估 AI 代理在 50 项专业税务任务中的表现](https://surgehq.ai/blog/dayjob-tax) ⭐️ 8.0/10

Dayjob 项目对 50 项真实的专业税务任务使用 AI 代理进行评估，展示了这些模型在税务自动化中的潜力与局限。测试结果显示，部分模型能够正确完成复杂的报税计算并发现错误，但也出现了显著的漏报和填错字段，导致退款金额偏差数千美元。文章指出，尽管 AI 能在税务工作流中提供辅助，但仍需人工复核以确保准确性。

hackernews · landonxi · 10月28日 15:46 · [社区讨论](https://news.ycombinator.com/item?id=50275626)

**「背景」** Dayjob 是 Surge AI 推出的用于评估经济价值型 AI 代理的基准套件，提供真实的专业任务场景并要求端到端的判断。该套件在其博客中被介绍，旨在让模型在复杂环境中处理文档、计算和合规等工作。

**「影响」** 税务专业人士在采用 AI 辅助工具时应将其视为初步审查层，必须在提交前进行人工核对，以防止因模型错误导致的财务损失。

**「社区讨论」** 评论者报告称，使用 Astra+Codex 时出现了数千美元的退款误差，而 Claude 能够识别汇率错误并提供纠正建议，显示不同模型的表现差异并强调了人工监督的重要性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://upstract.com/x/6876ee0f1d7cdf06">Dayjob : Tax – evaluating AI agents on 50 professional tax ...</a></li>
<li><a href="https://surgehq.ai/blog">Blog | Surge AI</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#tax automation`, `#LLM evaluation`, `#software engineering`

---

<a id="item-tech-news-4"></a>
### [GitHub Octoverse 2026](https://simonwillison.net/2026/Oct/28/github-octoverse-2026/) ⭐️ 8.0/10

GitHub’s 2026 Octoverse report delivers important, timely insight into developer activity trends.

rss · Simon Willison · 10月28日 16:45

**标签**: `#GitHub`, `#Developer Trends`, `#Open Source`

---

<a id="item-tech-news-5"></a>
### [ChatGPT 推出 iCloud 邮件与日历插件](https://x.com/ChatGPT/status/2115139248458191070) ⭐️ 8.0/10

OpenAI 在连续 28 天更新的第 23 天为所有 ChatGPT 方案（网页、桌面和 iOS）上线 iCloud 邮件与日历插件，用户可在对话中让模型搜索邮件、梳理收件箱、查看即将到来的日程或更新日历事件，功能面向全部用户开放。

telegram · zaihuapd · 10月28日 03:26

**「背景」** ChatGPT 自 2023 年推出插件平台后，允许开发者为模型接入外部服务，如 Gmail、Google Calendar 等。插件通过 API 让模型在对话中执行查询、创建或修改数据的操作。此次加入 iCloud 邮件和日历插件，意味着 iOS 用户也能在同一插件框架下直接访问苹果的邮件和日历服务。

**「影响」** iCloud 用户现在可以直接在 ChatGPT 对话里管理邮件和日历，省去切换应用的步骤；开发者也可基于该插件在自己的插件生态中提供类似的 iCloud 集成。

**标签**: `#ChatGPT`, `#iCloud Integration`, `#AI Plugins`, `#Product Update`

---

<a id="item-tech-news-6"></a>
### [长鑫存储计划限量量产 HBM3E，良率仅 20‑30%](https://www.reuters.com/world/china/chinas-cxmt-start-advanced-ai-memory-production-despite-poor-yields-sources-say-2026-10-28/) ⭐️ 8.0/10

长鑫存储（CXMT）计划在未来两个月内向国内 AI 芯片设计公司交付样品并启动限量量产 HBM3E，但其良率仅约 20% 至 30%，远低于 SK 海力士约 70% 的水平。该 HBM3E 的性能更接近 SK 海力士上一代 HBM3，预计售价高于海外同类产品。此举是在美国出口管制导致国内 AI 内存严重短缺的背景下进行的。

telegram · zaihuapd · 10月28日 06:19

**「HBM3E 与良率背景」** HBM（高带宽存储）是一种将多个 DRAM 芯片堆叠并通过硅通孔直接连接到 AI 处理器的存储技术，HBM3E 是该系列的最新代际，提供更高带宽。芯片良率指每片硅晶圆中通过测试并可出售的芯片比例，通常约为 70% 才能支撑大规模量产。受美国出口管制限制，中国在高端 AI 内存上依赖自主研发，而 CXMT 的首批 HBM3E 预计良率仅 20%‑30%，远低于行业常规水平。

**「影响」** 由于良率低，国内 AI 加速器厂商可能面临 HBM3E 供应紧张和成本上升，需在芯片设计或预算上做出调整以应对潜在的价格和交付风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thenextweb.com/news/cxmt-hbm3e-ai-memory-low-yields-reuters">China’s CXMT will make AI memory despite yields as low as 20 ...</a></li>
<li><a href="https://cryptobriefing.com/cxmt-hbm3e-production-low-yields/">CXMT plans HBM 3 E production even as most of its chips fail quality...</a></li>

</ul>
</details>

**标签**: `#HBM3E`, `#AI hardware`, `#memory manufacturing`, `#China semiconductor`

---

<a id="item-tech-news-7"></a>
### [MacBook Pro with PROLED XDR Display and Touch](https://www.apple.com/macbook-pro/proled-xdr-display/) ⭐️ 7.0/10

New MacBook Pro with ProLED XDR display and touch offers significant hardware upgrades but no major software impact.

hackernews · etothet · 10月28日 17:10 · [社区讨论](https://news.ycombinator.com/item?id=50276940)

**标签**: `#hardware`, `#macOS`, `#display`, `#laptops`

---

<a id="item-tech-news-8"></a>
### [How Much Does the Hint Matter? A generic feedback line matches self-written critiques in hindsight self-distillation \(ACM ICAIF &\#x27;26\) \[R\]](https://www.reddit.com/r/MachineLearning/comments/1xhv8yp/how_much_does_the_hint_matter_a_generic_feedback/) ⭐️ 7.0/10

A new study shows generic feedback matches detailed critiques in hindsight self‑distillation, improving efficiency for large language model training.

reddit · r/MachineLearning · /u/jhzyu · 10月28日 17:52

**标签**: `#self-distillation`, `#large-language-models`, `#training-efficiency`

---

<a id="item-tech-news-9"></a>
### [Discord 公开服务器对话将可被网络搜索](https://techcrunch.com/2026/10/27/discord-is-making-its-public-communities-more-searchable-and-people-have-concerns/) ⭐️ 7.0/10

Discord 于 2026 年 10 月 27 日宣布，将从 11 月 16 日起为每个可发现的公开服务器生成独立网页，并在 12 月中旬开始在网络搜索中显示部分公开频道的消息摘要。管理员可以自行选择哪些频道被索引，成员可选择退出，且展示的内容不包含用户名和头像。该功能因欧盟、英国等地区的法律限制默认关闭，且未向未成年人开放。

telegram · zaihuapd · 10月28日 03:21

**「背景」** Discord 的“可发现服务器”是指公开列在平台服务器目录中的社区，用户无需邀请即可加入，且这些服务器的聊天内容只能在 Discord 客户端内部搜索，未被外部搜索引擎索引。此前，Discord 并未提供将公开频道的对话生成网页或在网络搜索中展示的功能。

**「影响」** 社区管理员需审查并配置可索引的频道以及成员的退出选项，以防止敏感对话被公开搜索；同时，开发者应考虑其机器人或集成工具在新搜索环境下的数据暴露风险。

**标签**: `#Discord`, `#Searchability`, `#Privacy`, `#Community Platforms`

---

<a id="item-tech-news-10"></a>
### [韩国罚苹果 1550 万、谷歌 3200 万美元](https://appleinsider.com/articles/26/10/28/south-korea-becomes-the-latest-to-fine-apple-and-google-millions-over-their-app-stores) ⭐️ 7.0/10

South Korea fines Apple and Google over restrictive app store payment practices, signaling potential changes for developers.

telegram · zaihuapd · 10月28日 12:30

**标签**: `#app store policy`, `#mobile development`, `#regulation`

---

<a id="item-tech-news-11"></a>
### [ChatGPT Pro 与 Business 用户每月最高 500 美元 API 额度](https://developers.openai.com/api/docs/guides/chatgpt-api-credits) ⭐️ 7.0/10

OpenAI 为符合条件的 ChatGPT Pro 与 Business 用户提供每月最高 500 美元的 API 额度，作为订阅权益直接发放。Pro 用户可根据订阅档位领取等额额度（如 Pro $100 获得 $100，Pro $200 获得 $200，Pro $500 获得 $500），Business 用户则按付费席位计费，Standard 席位每席 $20，Premium 席位每席 $100，整个月工作区上限为 $500。用户需在 ChatGPT 或 API 平台将其拥有的 API 组织关联后才能激活该权益。

telegram · zaihuapd · 10月29日 01:12

**「API 额度背景」** OpenAI 的 ChatGPT Pro 与 Business 是付费订阅套餐，分别面向个人和企业用户，订阅后可在 ChatGPT 或 API 平台使用 OpenAI 的语言模型。此前使用 OpenAI API 需要自行购买使用量，未随订阅提供额外额度。此次将每月最高 500 美元的 API 额度作为订阅权益，需将用户账户关联到相应的 API 组织才能激活。

**「影响」** 开发者可通过此额度抵扣部分 API 使用费用，降低月度成本；在使用前必须完成组织关联，否则无法享受额度。

**标签**: `#OpenAI`, `#API credits`, `#ChatGPT Pro`, `#ChatGPT Business`, `#Developer tools`

---

<a id="item-tech-news-12"></a>
### [Google 将 AI 模式搜索广告扩展至全球](https://techcrunch.com/2026/10/28/google-expands-ai-search-ads-globally-as-core-ad-growth-slows/) ⭐️ 7.0/10

Google 母公司 Alphabet 在 2026 年第三季度财报电话会议上宣布，将 AI 模式搜索广告扩展至全球更多市场，并在美国首次推出支持多轮对话的广告形式。该模式下的赞助商品列表点击率已接近自然搜索结果。与此同时，Alphabet 报告第三季度搜索广告收入同比增长 12%，低于前两季度的 17% 和 19%，显示核心搜索广告业务增速放缓。

telegram · zaihuapd · 10月29日 01:43

**「AI 模式搜索广告的前身与技术基础」** AI 模式搜索广告是谷歌在 2025 年首次在美国测试的，将生成式 AI（基于 Gemini）嵌入搜索结果的赞助商品列表，提供对话式产品推荐和解释。随后在 2025 年底的内部简报中宣布将该功能扩展到更多国家，并在 2026 年 5 月通过 Google Marketing Live 推出 Conversational Discovery 等新格式。此次在第三季度财报电话会议上宣布的全球扩张正是基于这些早期试点和 Gemini 驱动的广告格式。

**「影响」** 广告主现在可以在搜索结果中使用生成式 AI 驱动的多轮对话广告，需要准备适配对话式创意并监测其点击率和转化表现，以评估相较传统搜索广告的效果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/products/ads-commerce/ads-in-ai-mode-global/">Ads in AI Mode expand to 10 new countries - The Keyword</a></li>
<li><a href="https://blog.google/products/ads-commerce/google-marketing-live-search-ads/">New ad formats built with Gemini coming to Google Search</a></li>

</ul>
</details>

**标签**: `#advertising`, `#search`, `#AI`, `#Google`

---