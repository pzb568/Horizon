---
layout: default
title: "Horizon Summary: 2026-11-16 (EN)"
date: 2026-11-16
lang: en
---

> From 36 items, 6 important content pieces were selected

---

**Technology News**
1. [Old Bitly Links Hijacked, Raising Security Concerns](#item-tech-news-1) ⭐️ 8.0/10
2. [Microsoft 365 outage linked to chlorine gas poisoning of hotel guests](#item-tech-news-2) ⭐️ 8.0/10
3. [Huawei Cloud launches open-source openPangu-2.1-Pro model on MaaS](#item-tech-news-3) ⭐️ 8.0/10
4. [In‑depth guide to positional embeddings in modern LLMs](#item-tech-news-4) ⭐️ 7.0/10
5. [Reports Suggest Jensen Huang May Return as Nvidia CEO](#item-tech-news-5) ⭐️ 7.0/10

**Financial News**
1. [US, China, Russia leaders to meet in Shenzhen during APEC](#item-finance-news-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Old Bitly Links Hijacked, Raising Security Concerns](https://ransomnews.com/burger-king-tweet-bitly-link-hijack-2026/) ⭐️ 8.0/10

Reports indicate that legacy Bitly short URLs are being redirected to malicious destinations, exposing developers and internet users to phishing and malware risks. The hijacking affects previously created links that were assumed to remain stable, highlighting a vulnerability in the URL‑shortening service’s ownership and redirection controls.

hackernews · hspeiser · Nov 15, 22:11 · [Discussion](https://news.ycombinator.com/item?id=50511395)

**「Background」** Bitly is a widely used URL shortening service that maps long web addresses to short, shareable links. When a Bitly account is inactive, deleted, or its domain expires, the service may recycle the short URLs, allowing new owners to control the previously created links. This recycling can enable malicious actors to hijack old Bitly links and redirect users to phishing or malware sites, raising security concerns for developers and internet users who rely on the stability of shortened URLs.

**「Impact」** Users who click compromised Bitly links may be sent to harmful sites, so organizations should audit any critical Bitly URLs, consider replacing them with self‑hosted shorteners, and monitor for unexpected redirects.

**「Community Discussion」** Commenters warned that outsourced shorteners can become unreliable over time and suggested using in‑house or alternative services to avoid permanent link breakage and security issues.

**Tags**: `#security`, `#url-shortening`, `#phishing`, `#infrastructure`

---

<a id="item-tech-news-2"></a>
### [Microsoft 365 outage linked to chlorine gas poisoning of hotel guests](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 8.0/10

An outage of Microsoft 365 on 15 November 2026 prevented an email alert about a malfunctioning chlorine dosing system from reaching hotel staff, allowing excessive chlorine to be released and causing irritation or injury to 15 guests. The incident shows that reliance on a single cloud‑based email channel for safety‑critical monitoring can directly affect public safety.

hackernews · DeepLogin · Nov 15, 18:36 · [Discussion](https://news.ycombinator.com/item?id=50509411)

**「Background」** Automated chlorination systems in commercial settings often rely on electronic monitoring that sends safety alerts through email, assuming continuous connectivity to the messaging service. When a cloud‑based email platform such as Microsoft 365 experiences an outage, those alerts can be delayed or lost, preventing operators from responding to over‑dispensing of chlorine in real time. This dependency on a single cloud email channel is a known design risk for safety‑critical monitoring systems.

**「Impact」** Facilities that use cloud email for alarm notifications should implement redundant alert paths—such as SMS, on‑premise paging, or direct sensor alarms—to ensure critical failures are communicated even during cloud service disruptions.

**「Community Discussion」** Commenters argued that the hotel’s design was unsafe for depending solely on email, blaming both the hotel’s lack of backup procedures and the broader practice of using cloud services for safety‑critical alerts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/data-centers/microsoft-365-outage-leads-to-chlorine-gas-poisoning-of-15-hotel-guests-email-warning-system-fails-40-first-responders-deployed-for-triage-four-hospitalized">Microsoft 365 outage leads to chlorine gas poisoning of 15 hotel ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=50509411">Microsoft 365 outage leads to chlorine gas poisoning of 15 hotel ...</a></li>

</ul>
</details>

**Tags**: `#cloud-computing`, `#system-reliability`, `#safety-critical`

---

<a id="item-tech-news-3"></a>
### [Huawei Cloud launches open-source openPangu-2.1-Pro model on MaaS](https://mp.weixin.qq.com/s/8JfFmscBTDl_mPQMycD8Nw) ⭐️ 8.0/10

Huawei Cloud’s MaaS \(Model-as-a-Service\) platform added the open‑source large language model openPangu‑2.1‑Pro on November 15. The model is tuned on more than 100,000 specialized data items to support three capability areas: Agent development, AI‑assisted coding, and inference optimization. Pricing is disclosed as 0.8 CNY per million input tokens, 3.2 CNY per million output tokens, and 0.016 CNY per million tokens for cache‑hit input. The offering is integrated with Huawei’s ecosystem, including HarmonyOS ArkTS development, Ascend operator generation, and products such as Zhiguo AgentArts, CodeArts, and OfficeAce.

telegram · zaihuapd · Nov 15, 16:03

**「Prerequisite: openPangu series and MaaS platform」** Huawei’s openPangu family is an open‑source large‑language‑model line that debuted with openPangu 2.0 Pro, a 505‑billion‑parameter model featuring a 512,000‑token context window and targeted at Huawei’s ecosystem. The MaaS \(Model‑as‑a‑Service\) platform on Huawei Cloud already offers model hosting and inference billing, providing the infrastructure for the newly announced openPangu‑2.1‑Pro.

**「Impact」** Software engineers and AI practitioners can now run open‑source LLM workloads on Huawei Cloud with clear token‑based costs, but must budget for the higher output‑token rate and ensure their code targets the supported ArkTS and Ascend environments to benefit from the model’s optimizations.

<details><summary>References</summary>
<ul>
<li><a href="https://1y.hk/en/post/11-15-openpangu-2-1-2jsl">Huawei Cloud to Launch openPangu - 2 . 1 - Pro on November 15 · AI...</a></li>
<li><a href="https://forgeeks.dev/huawei-openpangu-2-0-pro/">Huawei unveils 505-billion-parameter openPangu 2 .0 Pro — for(geeks)</a></li>

</ul>
</details>

**Tags**: `#large-language-model`, `#cloud-platform`, `#open-source`, `#AI-coding`, `#Huawei`

---

<a id="item-tech-news-4"></a>
### [In‑depth guide to positional embeddings in modern LLMs](https://magazine.sebastianraschka.com/p/understanding-positional-embeddings) ⭐️ 7.0/10

The article offers a detailed technical guide to positional embeddings in contemporary large language models, explaining how they are implemented \(e.g., rotary embeddings\) and how they enable models to encode token order. It is aimed at engineers and researchers who need a practical understanding of these mechanisms.

hackernews · vismit2000 · Nov 15, 12:14 · [Discussion](https://news.ycombinator.com/item?id=50506376)

**「Background」** Positional embeddings are a mechanism that injects token order information into transformer models, which otherwise treat inputs as a set without inherent sequence. Early LLMs used absolute sinusoidal or learned embeddings, while newer models often adopt rotary \(RoPE\) embeddings—a relative encoding introduced in 2022 and now common in open‑weight models such as LLaMA and PaLM.

**「Community discussion」** programjames notes that while the article covers implementation details, a full grasp of positional embeddings also requires understanding their theoretical foundation as group representations, especially for rotary embeddings tied to the translation group.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=o29P0Kpobz0">Rotary Positional Embeddings : Combining Absolute and Relative</a></li>
<li><a href="https://medium.com/ai-insights-cobet/rotary-positional-embeddings-a-detailed-look-and-comprehensive-understanding-4ff66a874d83">Rotary Positional Embeddings : A Detailed Look and... | Medium</a></li>

</ul>
</details>

**Tags**: `#positional embeddings`, `#large language models`, `#machine learning`, `#deep learning`

---

<a id="item-tech-news-5"></a>
### [Reports Suggest Jensen Huang May Return as Nvidia CEO](https://www.ft.com/content/0f30a230-4d66-481b-a4fd-3a4ed0c45855) ⭐️ 7.0/10

Financial Times reports that Nvidia co‑founder Jensen Huang is discussing a possible return to the CEO role with close allies, after resigning last week amid personal scandal. Allies are forming a Silicon Valley &quot;war room&quot; to lobby the board and have gathered over 156,000 petition signatures while seeking White House support. The board is also in talks with Arm CEO Rene Haas as an alternative candidate.

telegram · zaihuapd · Nov 16, 01:06

**「Background」** Jensen Huang co‑founded Nvidia in 1993 and has served as its chief executive, guiding the company to dominate the GPU market for AI workloads. In November 2026 he resigned after reports of two extramarital affairs, one involving a person alleged to be a Chinese spy, which sparked board and regulatory scrutiny. This context explains why any talk of his possible return as CEO is noteworthy.

**「Impact」** If Huang were to resume the CEO position, Nvidia could see renewed strategic direction and investor confidence, potentially stabilising its stock after recent volatility caused by the leadership upheaval.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/world/china/jensen-huang-discusses-comeback-nvidia-ceo-with-allies-ft-reports-2026-11-15/">Jensen Huang discusses comeback as Nvidia CEO with allies, FT ...</a></li>
<li><a href="https://tech.yahoo.com/general/breaking-news/article/jensen-huang-weighs-comeback-as-nvidia-ceo-as-allies-lobby-board-ft-reports-bessent-calls-for-dramatic-shakeup-204839950.html">Jensen Huang weighs comeback as Nvidia CEO as allies lobby ...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI hardware`, `#Corporate leadership`

---

## Financial News

<a id="item-finance-news-1"></a>
### [US, China, Russia leaders to meet in Shenzhen during APEC](https://apnews.com/article/trump-xi-putin-summit-china-5fe92253ef38100bae913834a9b74d72) ⭐️ 7.0/10

US, Chinese and Russian leaders will hold their first trilateral meeting on the sidelines of the APEC summit in Shenzhen on Nov 19, according to the Chinese foreign ministry.

telegram · zaihuapd · Nov 16, 01:38

**「APEC summit context」** The Asia‑Pacific Economic Cooperation \(APEC\) leaders’ meeting, hosted by China in Shenzhen on Nov 18‑19 2026, provides a venue for bilateral talks, and the three‑way meeting is being held on the sidelines, outside the formal APEC agenda.

<details><summary>References</summary>
<ul>
<li><a href="https://www.arabnews.com/world/trump-xi-putin-to-hold-historic-meeting-in-china-white-house-3011775">Trump, Xi, Putin to hold historic meeting in China : White House</a></li>
<li><a href="https://en.wikipedia.org/wiki/APEC_China_2026">APEC China 2026 - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#International Relations`, `#Diplomacy`, `#APEC`, `#US-China-Russia`, `#Geopolitics`

---