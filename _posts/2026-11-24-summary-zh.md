---
layout: default
title: "Horizon Summary: 2026-11-24 (ZH)"
date: 2026-11-24
lang: zh
---

> 从 38 条内容中筛选出 8 条重要资讯。

---

**科技新闻**
1. [Codex2api 供应链投毒，v3.1.11 带后门，建议回退至 3.1.9](#item-tech-news-1) ⭐️ 8.0/10
2. [鸿蒙终端突破 1 亿台，应用服务超 46 万项](#item-tech-news-2) ⭐️ 8.0/10
3. [新加坡总理表态不做美国芯片禁运规避通道](#item-tech-news-3) ⭐️ 8.0/10
4. [Nvidia 董事会恢复黄仁勋为首席执行官](#item-tech-news-4) ⭐️ 7.0/10
5. [Stalwart 成为 Microsoft Exchange 的即插即用替代方案](#item-tech-news-5) ⭐️ 7.0/10
6. [AI 生成的黎曼猜想证明代码被作者承认无效](#item-tech-news-6) ⭐️ 7.0/10

**财经新闻**
1. [美联储纽约分行行长约翰·威廉姆斯暗示将逐步加息](#item-finance-news-1) ⭐️ 8.0/10
2. [Anthropic 创纪录 IPO 引发全球抛售，冲击中国 AI 公司上市计划](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Codex2api 供应链投毒，v3.1.11 带后门，建议回退至 3.1.9](https://github.com/WormW/codex2api-incident-2026-11) ⭐️ 8.0/10

Codex2api 项目作者账号被入侵，攻击者绕过 main 分支直接推送 tag，导致 v3.1.11 发行版移除鉴权并可无密码远程执行命令，同时通过 workflow 将仓库中 16 条 Actions secrets 泄露，波及同一账号下至少 21 个仓库。已安装或更新至 3.1.10‑3.1.12 版本的用户应立即停用该版本，回退至 3.1.9，并更换所有 GitHub token、SSH key、数据库凭证以及 DeepSeek 等相关密钥。

telegram · zaihuapd · 11月23日 11:21

**「Codex2api 项目概述」** Codex2api 是一个开源的 API 代理服务器，旨在把 OpenAI Codex、Anthropic、Gemini 等模型的请求统一转发到 Codex Responses API，并提供账户池、流式传输和滥用防护等功能。它以 Node.js 实现，代码托管在 GitHub 上，供开发者在自己的服务中直接使用。

**「影响」** 受影响的开发者若不及时回退并轮换凭证，将面临未授权的远程代码执行和泄露的密钥被滥用的风险，可能导致其系统被攻击者控制或数据被窃取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/rokyplay/codex2api">GitHub - rokyplay/codex2api: OpenAI Codex API proxy with ...</a></li>
<li><a href="https://github.com/ZHX08/codex2api/blob/main/README.md">codex2api/README.md at main · ZHX08/codex2api · GitHub</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#AI-tools`, `#open-source`

---

<a id="item-tech-news-2"></a>
### [鸿蒙终端突破 1 亿台，应用服务超 46 万项](https://www.xinhuanet.com/20261124/68842538167d4e59a875056d5eb885ad/c.html) ⭐️ 8.0/10

华为终端有限公司于 2026 年 11 月 24 日宣布，搭载 HarmonyOS 5、6、7 的手机、平板和电脑设备累计已突破 1 亿台。同时，HarmonyOS 可获取的应用和服务数量超过 46 万项，注册开发者超过 1200 万人。该系统自 2019 年首次发布，2024 年 10 月推出原生鸿蒙后，至 2026 年实现上述规模。开源社区已聚集约 1.4 万名贡献者，形成 120 余个行业发行版。

telegram · zaihuapd · 11月24日 01:46

**「背景」** 鸿蒙操作系统于 2019 年首次发布，2024 年 10 月推出原生鸿蒙版本，随后逐步在手机、平板和电脑等终端上部署。此前的发布奠定了其跨设备统一系统的基础，也为后续的开源社区贡献和行业发行版的形成提供了技术和生态支撑。

**「影响」** 超过 1 亿台的用户基数为开发者提供了巨大的潜在市场，意味着针对 HarmonyOS 的应用可以直接触达数以千万计的终端用户，提升了在中国及部分海外市场的商业价值。

**标签**: `#Operating Systems`, `#Huawei`, `#Open Source`, `#Mobile Development`

---

<a id="item-tech-news-3"></a>
### [新加坡总理表态不做美国芯片禁运规避通道](https://www.bloomberg.com/news/articles/2026-11-24/singapore-won-t-be-conduit-to-skirt-us-chip-curbs-wong-says) ⭐️ 8.0/10

新加坡总理黄循财在 2026 年 11 月 24 日表示，新加坡不会被用作企业规避美国芯片出口管制的通道，并称当局正调查 Megaspeed 采购英伟达芯片的交易。此前美国商务部已将 Megaspeed 及另外六家东南亚企业列入贸易黑名单，指其存在向未获授权用户转移先进计算产品的重大风险。黄循财强调，新加坡将阻止任何帮助绕过美国禁令的行为。

telegram · zaihuapd · 11月24日 05:03

**「背景」** 美国商务部通过《联邦公报》将包括 Megaspeed 在内的多家东南亚企业列入实体清单，禁止它们在未获授权的情况下获取先进计算芯片，这是一项针对高性能 AI 及半导体技术的出口管制措施。该清单旨在防止这些企业将受限的芯片转售给禁运对象，而新加坡因其在区域供应链中的枢纽地位，成为美国关注的潜在规避通道。黄循财总理的声明正是对美国此类管制的直接回应，表明新加坡不会提供帮助以规避这些出口限制。

**「影响」** 受此表态影响，试图通过新加坡转移受限芯片的公司需重新评估供应链，若继续违规可能面临美国制裁或被列入黑名单。

**标签**: `#chip export controls`, `#hardware`, `#AI compute`, `#geopolitics`

---

<a id="item-tech-news-4"></a>
### [Nvidia 董事会恢复黄仁勋为首席执行官](https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html) ⭐️ 7.0/10

Nvidia 董事会已于 2026 年 11 月 23 日正式恢复黄仁勋为公司首席执行官，结束了他在过去两周被迫离职的短暂期间，此决定适用于公司全球业务。

hackernews · jaz · 11月23日 14:00 · [社区讨论](https://news.ycombinator.com/item?id=50611576)

**「背景说明」** 在 2026 年初，英伟达董事会因对公司治理和潜在国家安全担忧而罢免了创始人兼首席执行官黄仁勋，随后由临时管理团队接管公司运营。这一罢免在业界和政府间引发了广泛讨论，成为本次董事会决定恢复黄仁勋职务的直接前提。

**「影响」** 此领导层的恢复为投资者和合作伙伴提供了治理稳定性的信号，可能提升市场对 Nvidia AI 硬件路线图的信心并促使分析师上调业绩预期。

**「社区讨论」** 一位评论者指出，董事会在做出决定时已收到美国政府高级官员的意见，并确信黄仁勋的复职不会构成国家安全风险。

**标签**: `#Nvidia`, `#Leadership`, `#AI hardware`, `#Industry news`

---

<a id="item-tech-news-5"></a>
### [Stalwart 成为 Microsoft Exchange 的即插即用替代方案](https://stalw.art/blog/microsoft-exchange-replacement/) ⭐️ 7.0/10

Stalwart 现在提供一个开源、可本地部署的邮件服务器，声称可以直接替代 Microsoft Exchange，满足 Microsoft 正在逐步停止对本地 Exchange 的支持的需求。该方案兼容 Exchange 使用的主要协议，面向需要保留本地邮件系统的系统管理员和企业用户。虽然提供了实用的迁移路径，但并未带来根本性的技术突破。

hackernews · shaunpud · 11月23日 22:32 · [社区讨论](https://news.ycombinator.com/item?id=50620349)

**「背景说明」** Microsoft Exchange 多年来一直是企业内部邮件服务器的标准，配合 Outlook 客户端通过 MAPI、EWS、ActiveSync 等专有协议提供完整的邮件、日历和协作功能。近期微软宣布逐步停止对本地 Exchange 的支持，转向基于云的 Office 365 服务，这迫使需要保留本地部署的组织寻找兼容的替代方案。Stalwart 1.2.0 在此背景下实现了对 MAPI、EWS、ActiveSync 和 Autodiscover 的支持，因而能够在不更改客户端配置的情况下取代 Exchange。

**「需要考虑合规和客户端兼容性」** 使用 Stalwart 替代本地 Exchange 可让管理员在 Microsoft 停止对本地 Exchange 支持后继续使用本地邮件服务器，但组织必须自行解决合规存档（如德国 GoBD 要求的不可删除、长期保存）以及 Outlook 对 Exchange 专有功能的依赖，可能需要额外的归档工具或改用支持 IMAP 的客户端。

**「社区讨论」** 有评论指出，Stalwart 在德国等地区缺乏符合 GoBD 要求的不可删除、长期存档功能，这可能限制其在受监管行业的使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://stalw.art/blog/microsoft-exchange-replacement/">Stalwart is now a drop-in replacement for Microsoft Exchange</a></li>
<li><a href="https://www.learn.telusko.com/newsletter/stalwart-1-2-0-is-now-a-drop-in-replacement-for-microsoft-exchange">Stalwart 1.2.0 is now a drop-in replacement for Microsoft ...</a></li>
<li><a href="https://stalw.art/blog/microsoft-exchange-replacement/">Stalwart is now a drop-in replacement for Microsoft Exchange | Stalwart</a></li>

</ul>
</details>

**标签**: `#email`, `#open-source`, `#enterprise`, `#mail-server`

---

<a id="item-tech-news-6"></a>
### [AI 生成的黎曼猜想证明代码被作者承认无效](https://x.com/i/web/status/2124987173439209561) ⭐️ 7.0/10

Alpöge 与 Claude 宣称利用 Lean 生成约 1700 万行、17.5 万文件的代码，声称证明了黎曼猜想及其广义形式，但未提供人类可读的证明文本。Lean 与 Mathlib 社区最初对代码的可编译性表示有信心，随后研究者指出关键定义被写成恒真，实际证明可能是空转。23 日，Alpöge 承认其中约 25 万页代码是“玩笑”，代码“满是垃圾但能编译”，并接受了批评。

telegram · zaihuapd · 11月24日 01:29

**「背景」** 2026 年 11 月 20 日，Anthropic 研究员 Levent Alpöge 宣布他与 AI 模型 Claude 共同在 Lean 形式化语言中生成了约 1700 万行、17.5 万文件的代码，声称已证明黎曼猜想及其广义形式，引发数学界和科技圈的广泛关注。Lean 是一种用于形式化数学证明的交互式定理证明器，配套的 Mathlib 库提供了大量已验证的数学定义和定理，因而被视为验证此类宏大声明的技术平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.clarin.com/us-news/who-is-levent-alpoge-the-anthropic-mathematician-who-claims-solved-the-riemann-hypothesis-with-claude_0_2WdGvYKBVM.html">Who is Levent Alpöge ? The Anthropic mathematician who claims he...</a></li>
<li><a href="https://www.npr.org/2026/11/21/g-s1-154922/anthropic-worker-claims-to-have-solved-a-holy-grail-of-math-problems-with-the-help-of-ai">Anthropic worker claims to have solved a Holy Grail of math... : NPR</a></li>

</ul>
</details>

**标签**: `#AI`, `#Formal Verification`, `#Theorem Proving`, `#Lean`, `#Riemann Hypothesis`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储纽约分行行长约翰·威廉姆斯暗示将逐步加息](https://www.cnbc.com/2026/11/23/john-williams-fed-inflation-rate-hikes.html) ⭐️ 8.0/10

约翰·威廉姆斯表示，为将通胀恢复至 2%目标，可能在未来逐步加息，市场已计入 12 月会议将升息 0.25 个百分点至 3.75%-4%区间。

rss · CNBC Finance · 11月23日 21:02

**「背景」** 美国通胀仍高于 2%目标，联邦公开市场委员会（FOMC）将在 12 月 8-9 日召开会议决定利率走向。

**「影响」** 家庭和企业的贷款利率可能上升，增加借贷成本。

**标签**: `#monetary policy`, `#inflation`, `#Federal Reserve`

---

<a id="item-finance-news-2"></a>
### [Anthropic 创纪录 IPO 引发全球抛售，冲击中国 AI 公司上市计划](https://www.bloomberg.com/news/articles/2026-11-23/china-s-next-ai-deals-clouded-by-selloff-after-anthropic-ipo) ⭐️ 7.0/10

Anthropic 以 1195 亿美元的创纪录 IPO 引发全球股市抛售，中国科技股自 6 月底累计蒸发 1.7 万亿美元，导致 DeepSeek 与月之暗面等公司上市计划受阻。

telegram · zaihuapd · 11月23日 09:31

**「背景」** DeepSeek 正在准备最迟 2026 年底提交 IPO 申请，目标 2027 年上市；月之暗面已在香港进行保密上市备案，计划明年第一季度上市，但 Anthropic 于 11 月底完成 1195 亿美元创纪录的 AI IPO，随后引发全球科技股抛售，使自 6 月底以来中国科技股市值蒸发约 1.7 万亿美元。

**「影响」** 筹备上市的 DeepSeek、月之暗面等中国 AI 企业因市场情绪恶化可能被迫推迟或取消发行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.straitstimes.com/business/deepseek-preparing-for-ipo-filing-as-soon-as-end-2026">DeepSeek IPO plans: Filing by end-2026 for 2027 debut | The ...</a></li>
<li><a href="https://chinaaicompass.com/companies/moonshot-ai">Moonshot AI（月之暗面（Kimi）） — China AI Compass</a></li>

</ul>
</details>

**标签**: `#AI`, `#IPO`, `#ChineseTech`, `#MarketSelloff`

---