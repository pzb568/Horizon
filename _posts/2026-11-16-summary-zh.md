---
layout: default
title: "Horizon Summary: 2026-11-16 (ZH)"
date: 2026-11-16
lang: zh
---

> 从 36 条内容中筛选出 6 条重要资讯。

---

**科技新闻**
1. [旧 Bitly 短链接被劫持](#item-tech-news-1) ⭐️ 8.0/10
2. [Microsoft 365 邮件中断导致酒店氯气泄漏，15 名客人受害](#item-tech-news-2) ⭐️ 8.0/10
3. [华为云发布开源盘古模型 openPangu-2.1-Pro](#item-tech-news-3) ⭐️ 8.0/10
4. [理解现代大语言模型中的位置嵌入](#item-tech-news-4) ⭐️ 7.0/10
5. [黄仁勋或将回归英伟达 CEO](#item-tech-news-5) ⭐️ 7.0/10

**财经新闻**
1. [中美俄领袖首次在 APEC 期间会晤](#item-finance-news-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [旧 Bitly 短链接被劫持](https://ransomnews.com/burger-king-tweet-bitly-link-hijack-2026/) ⭐️ 8.0/10

近期有报告称，Bitly 平台对已失效或所有者账户被停用的旧短链接进行回收，再指向攻击者控制的恶意站点。此行为导致原本安全的 Bitly 链接在被重新分配后成为钓鱼或恶意软件的入口，影响依赖这些链接的开发者和普通网民。

hackernews · hspeiser · 11月15日 22:11 · [社区讨论](https://news.ycombinator.com/item?id=50511395)

**「URL 缩短服务的基本原理」** Bitly 是一种常用的 URL 缩短服务，它通过将原始的长链接映射到一个短的、唯一的标识符来生成短链接。每个短链接在 Bitly 的数据库中对应一条记录，指向原始目标 URL。若创建短链接的账户被停用、删除或长时间未维护，Bitly 可能会回收这些短标识符并允许新用户重新分配，从而导致原本指向合法站点的旧链接被重新指向恶意页面。了解这种回收机制以及账户管理策略，有助于理解为何旧的 Bitly 链接会被劫持。

**「影响」** 用户点击被劫持的旧 Bitly 链接可能被重定向到钓鱼页面或恶意下载，增加安全风险；开发者应避免在长期使用场景中依赖 Bitly 链接，或采用自建短链服务并监控链接所有权。

**「社区讨论」** 评论者 xp84 认为外包的短链服务风险极高，因为链接随时间可能被回收并被劫持；5kyl4b 则表达了对任何短链服务的根本反感，强调了此类安全隐患。

**标签**: `#security`, `#url-shortening`, `#phishing`, `#infrastructure`

---

<a id="item-tech-news-2"></a>
### [Microsoft 365 邮件中断导致酒店氯气泄漏，15 名客人受害](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 8.0/10

2026 年 11 月 15 日，德国一家酒店的氯气消毒系统因剂量过高导致氯气泄漏，约 15 名客人出现呼吸道刺激，其中 4 人送医。事故调查指出，监控系统通过 Microsoft 365 邮件发送的警报未能送达，因当时的 Microsoft 365 服务中断，导致工作人员未及时发现并停止过量投药。该报道为新闻稿，未提供独立验证。

hackernews · DeepLogin · 11月15日 18:36 · [社区讨论](https://news.ycombinator.com/item?id=50509411)

**「背景」** 该酒店的氯化剂自动加注系统依赖电子邮件警报来提醒工作人员氯浓度异常；当系统检测到过高浓度时会发送邮件至维护人员。2026 年 11 月 12 日的 Microsoft 365 大规模宕机导致 Outlook 和 Exchange Online 无法使用，致使该警报未能送达，进而未能及时关闭加注阀，导致 15 名客人吸入氯气。此类基于云邮件的安全监控在缺乏冗余渠道时极易受到云服务中断的影响。

**「影响」** 酒店及其他依赖云邮件进行安全警报的设施应增加本地或多渠道的备份通知机制，如短信、现场警报或专用监控系统，以防止单点故障导致的安全事故。

**「社区讨论」** 评论者普遍认为事故是酒店设计缺陷，批评仅依赖云邮件进行危害警报，并呼吁采用更具冗余性的监控架构；也有人指出将责任归咎于 Microsoft 365 是不恰当的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/data-centers/microsoft-365-outage-leads-to-chlorine-gas-poisoning-of-15-hotel-guests-email-warning-system-fails-40-first-responders-deployed-for-triage-four-hospitalized">Microsoft 365 outage leads to chlorine gas poisoning of 15 hotel ...</a></li>

</ul>
</details>

**标签**: `#cloud-computing`, `#system-reliability`, `#safety-critical`

---

<a id="item-tech-news-3"></a>
### [华为云发布开源盘古模型 openPangu-2.1-Pro](https://mp.weixin.qq.com/s/8JfFmscBTDl_mPQMycD8Nw) ⭐️ 8.0/10

华为云 MaaS（模型即服务）平台于 11 月 15 日正式上线开源大语言模型 openPangu-2.1‑Pro，面向开发者提供 Agent 开发、AI 编码和推理优化三大能力。该模型基于超过 10 万条专项数据进行 Skills 触发与工具调用，重点适配鸿蒙 ArkTS 开发和升腾算子生成，并已接入智果 AgentArts、码道 CodeArts、果办 OfficeAce 等产品。推理费用为 0.8 元/百万 tokens（输入）和 3.2 元/百万 tokens（输出），缓存命中费用 0.016 元/百万 tokens。

telegram · zaihuapd · 11月15日 16:03

**「背景」** openPangu 系列是华为推出的开源大语言模型。上一代 openPangu‑2.0‑Pro 已于 2025 年发布，拥有约 5050 亿参数和 512 k token 的上下文窗口，展示了华为在大模型规模和开放生态方面的布局。该模型通过华为云的 MaaS（模型即服务）平台提供，MaaS 为用户提供模型托管、推理计费和 API 调用等基础能力，为后续的 openPangu‑2.1‑Pro 在 AI 编码、Agent 开发和推理优化方向的升级奠定了平台和技术基础。

**「影响」** 开发者可直接在华为云 MaaS 上使用 openPangu-2.1‑Pro 进行智能 Agent 与代码生成实验，需根据上述 token 计费模型评估成本并在项目预算中预留相应费用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://1y.hk/en/post/11-15-openpangu-2-1-2jsl">Huawei Cloud to Launch openPangu - 2 . 1 - Pro on November 15 · AI...</a></li>
<li><a href="https://forgeeks.dev/huawei-openpangu-2-0-pro/">Huawei unveils 505-billion-parameter openPangu 2 .0 Pro — for(geeks)</a></li>

</ul>
</details>

**标签**: `#large-language-model`, `#cloud-platform`, `#open-source`, `#AI-coding`, `#Huawei`

---

<a id="item-tech-news-4"></a>
### [理解现代大语言模型中的位置嵌入](https://magazine.sebastianraschka.com/p/understanding-positional-embeddings) ⭐️ 7.0/10

2026 年 11 月 15 日，Sebastian Raschka 的技术专栏发布了一篇题为《Understanding Positional Embeddings in Modern LLMs》的文章，系统阐述了位置嵌入在当代大语言模型中的实现方式，包括绝对、相对以及旋转（Rotary）等主流方法，并解释了它们的数学原理和在 Transformer 中的作用。文章面向工程师和研究者，提供代码示例和实践建议，但并未宣布新的模型或技术突破。

hackernews · vismit2000 · 11月15日 12:14 · [社区讨论](https://news.ycombinator.com/item?id=50506376)

**「位置嵌入的基本概念」** 在基于 Transformer 的语言模型中，注意力机制本身对序列顺序没有感知能力，因此需要通过位置嵌入（positional embeddings）向模型注入位置信息。最早的实现是使用固定的正弦/余弦绝对位置编码，随后出现了相对位置编码以及 2022 年提出的旋转位置编码（Rotary Positional Embedding，RoPE），后者将位置向量视为复数旋转并已被 Google 的 PaLM 和 Meta 的 LLaMA 等开源模型广泛采用。

**「影响」** 阅读该指南的开发者可以更准确地在自己的模型中选择或实现合适的位置嵌入，从而提升模型的序列建模能力。

**「社区讨论」** programjames 认为，仅了解实现细节不足以真正掌握位置嵌入，必须从群表示理论出发，指出旋转位置嵌入对应平移群的表示，并讨论其可微分参数化方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=o29P0Kpobz0">Rotary Positional Embeddings : Combining Absolute and Relative</a></li>
<li><a href="https://medium.com/ai-insights-cobet/rotary-positional-embeddings-a-detailed-look-and-comprehensive-understanding-4ff66a874d83">Rotary Positional Embeddings : A Detailed Look and... | Medium</a></li>

</ul>
</details>

**标签**: `#positional embeddings`, `#large language models`, `#machine learning`, `#deep learning`

---

<a id="item-tech-news-5"></a>
### [黄仁勋或将回归英伟达 CEO](https://www.ft.com/content/0f30a230-4d66-481b-a4fd-3a4ed0c45855) ⭐️ 7.0/10

《金融时报》报道，黄仁勋正与亲信讨论重新担任英伟达 CEO；他上周因两段婚外情曝光已辞职，其中一名涉事者被指为中国间谍，导致外界对华 AI 芯片出口产生担忧。盟友已组建硅谷高管“作战室”，发起请愿并已获约 15.6 万签名，试图游说董事会并争取白宫支持。与此同时，董事会已接触 Arm CEO Rene Haas，视其为潜在继任者。此事仍属讨论阶段，尚未确认正式任命。

telegram · zaihuapd · 11月16日 01:06

**「背景信息」** Jensen Huang 是 Nvidia 的联合创始人兼长期 CEO，自 1993 年起带领公司成为 AI 芯片领域的领军企业。2026 年底因两段婚外情曝光——其中一人被指为中国间谍——而被迫辞职，引发对华 AI 芯片出口的担忧。正是基于其此前的领导地位和近期的辞职争议，媒体才关注其可能回归 CEO 的讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reuters.com/world/china/jensen-huang-discusses-comeback-nvidia-ceo-with-allies-ft-reports-2026-11-15/">Jensen Huang discusses comeback as Nvidia CEO with allies, FT ...</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#AI hardware`, `#Corporate leadership`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中美俄领袖首次在 APEC 期间会晤](https://apnews.com/article/trump-xi-putin-summit-china-5fe92253ef38100bae913834a9b74d72) ⭐️ 7.0/10

美国、俄罗斯和中国领导人计划于 11 月 19 日在深圳 APEC 峰会期间的场边举行首次三方会晤。

telegram · zaihuapd · 11月16日 01:38

**「背景」** APEC（亚太经济合作组织）是亚太地区的多边经济论坛，2026 年由中国在深圳主办，这是中国第三次承办该峰会（2001、2014 年后），会议通常聚焦经济议题而不包括正式的双边或三边会谈。

**「潜在影响」** 会议可能促使美、中、俄就核裁军展开讨论，进而影响全球安全格局和防务市场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/APEC_China_2026">APEC China 2026 - Wikipedia</a></li>
<li><a href="https://www.cbsnews.com/news/trump-putin-xi-jinping-meeting-china-us-russia-talks/">Trump, Putin, Xi Jinping to meet in first trilateral of its kind</a></li>

</ul>
</details>

**标签**: `#International Relations`, `#Diplomacy`, `#APEC`, `#US-China-Russia`, `#Geopolitics`

---