---
layout: default
title: "Horizon Summary: 2026-10-18 (EN)"
date: 2026-10-18
lang: en
---

> From 37 items, 8 important content pieces were selected

---

**Technology News**
1. [DeepSeek-v4.1-Flash-1017](#item-tech-news-1) ⭐️ 8.0/10
2. [Qualcomm denies Snapdragon 8 Elite Gen 6 thermal issues amid Samsung’s warning](#item-tech-news-2) ⭐️ 8.0/10
3. [OpenCode 遭攻击，🤖 OpenAI 和 🤖 Anthropic等 API 密钥外泄](#item-tech-news-3) ⭐️ 8.0/10
4. [Pele – Themeable SVG Rendering for Mermaid Diagrams](#item-tech-news-4) ⭐️ 7.0/10
5. [Estonia publishes source code of its online voting system](#item-tech-news-5) ⭐️ 7.0/10
6. [Llmspeed lets developers estimate local LLM performance before buying hardware](#item-tech-news-6) ⭐️ 7.0/10
7. [China Mobile Hong Kong and Macau Operators Deploy First U6GHz 5G‑A/6G Networks](#item-tech-news-7) ⭐️ 7.0/10

**Financial News**
1. [Berkshire Hathaway invests over $900 million in Bending Spoons](#item-finance-news-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [DeepSeek-v4.1-Flash-1017](https://huggingface.co/deepseek-ai/DeepSeek-V4.1-Flash-1017) ⭐️ 8.0/10

DeepSeek V4.1 Flash delivers notable speed and coding benchmark gains, making it a valuable update for developers.

hackernews · theykk · Oct 17, 08:21 · [Discussion](https://news.ycombinator.com/item?id=50129045)

**Tags**: `#large-language-model`, `#code-generation`, `#open-source`, `#deepseek`

---

<a id="item-tech-news-2"></a>
### [Qualcomm denies Snapdragon 8 Elite Gen 6 thermal issues amid Samsung’s warning](https://www.163.com/dy/article/L9EFR7ID051191D6.html) ⭐️ 8.0/10

Qualcomm’s chief marketing officer publicly refuted claims that the Snapdragon 8 Elite Gen 6 \(also referenced as Snapdragon 8EE6\) has a systemic overheating problem, saying that pre‑release platform tuning by OEMs is normal to balance performance and power. The denial follows a Korean media report that a Samsung Galaxy S27 Ultra prototype using the chip exhibited high‑load heat and throttling, prompting Samsung to demand a fix by mid‑October or consider shifting its orders to its own 2 nm Exynos 2700 processor.

telegram · zaihuapd · Oct 17, 04:12

**「Technical context」** Snapdragon 8 Elite Gen 6 is Qualcomm’s latest high‑end mobile SoC, marketed as the Snapdragon 8 Elite Mobile Platform and offered in an Extreme variant \(8EE6\) that targets flagship performance. Qualcomm typically performs platform‑level tuning with OEMs before volume shipment to balance performance and power consumption, a process that can surface temporary thermal throttling under heavy load. Samsung’s upcoming Exynos 2700, built on a 2 nm process node, is being readied for the Galaxy S27 Ultra as an alternative to Qualcomm’s chip, and Samsung has warned it may shift orders if the Snapdragon’s heat issues are not resolved.

**「Impact」** If Qualcomm does not resolve the reported thermal concerns, Samsung may move future flagship orders to its in‑house Exynos 2700, potentially altering supply‑chain dynamics for Android OEMs and requiring developers to adapt to a different SoC for performance‑critical applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2_nm_process">2 nm process - Wikipedia</a></li>
<li><a href="https://nokiapoweruser.com/samsung-exynos-2700-mass-production-galaxy-s27-ultra/">Samsung Begins Exynos 2700 Mass Production: 2 nm Power for...</a></li>
<li><a href="https://www.qualcomm.com/smartphones/products/8-series/snapdragon-8-elite-mobile-platform">Snapdragon 8 Elite Mobile Platform | Qualcomm</a></li>

</ul>
</details>

**Tags**: `#mobile hardware`, `#SoC`, `#thermal management`, `#industry news`

---

<a id="item-tech-news-3"></a>
### [OpenCode 遭攻击，🤖 OpenAI 和 🤖 Anthropic等 API 密钥外泄](https://startupfortune.com/opencode-breach-exposes-stored-openai-and-anthropic-keys-prompts-urgent-key-rotation/) ⭐️ 8.0/10

OpenCode suffered a large‑scale attack leaking OpenAI, Anthropic, and Google API keys, urging developers to revoke and rotate credentials promptly.

telegram · zaihuapd · Oct 17, 23:43

**Tags**: `#security`, `#api-keys`, `#openai`, `#anthropic`, `#opencode`

---

<a id="item-tech-news-4"></a>
### [Pele – Themeable SVG Rendering for Mermaid Diagrams](https://pele.run/) ⭐️ 7.0/10

Pele is a web tool that renders Mermaid diagrams as themeable SVG files, allowing developers to style and embed diagrams more easily without dealing with the usual Mermaid styling limitations. The service is publicly available at https://pele.run/.

hackernews · dchest · Oct 17, 15:55 · [Discussion](https://news.ycombinator.com/item?id=50132193)

**「Background」** Mermaid is a JavaScript‑based diagram definition language that normally renders diagrams by executing its layout engine in a browser or headless Chromium environment, producing SVG that is not readily themeable with external CSS. This reliance on a full browser runtime makes it difficult for developers to embed Mermaid diagrams in static tools or to customize their appearance without modifying the library itself.

**「Impact」** Developers can now generate SVG output for Mermaid diagrams that can be customized via CSS, simplifying integration into documentation, developer tools, and other environments that do not support a full or headless browser for Mermaid rendering.

**「Community Discussion」** Commenters noted that the official Mermaid library often requires a browser environment for layout, and Pele’s SVG output could eliminate that need \(nickmain\). Another user confirmed the project is open‑source on GitHub \(Imustaskforhelp\).

<details><summary>References</summary>
<ul>
<li><a href="https://pele.run/">Pele · Mermaid diagrams as themeable SVG</a></li>
<li><a href="https://elsolitario.org/en/2026/10/17/pele-render-mermaid-diagrams-svg/">Mermaid Diagrams to SVG: What Is Pele and How to Use It</a></li>

</ul>
</details>

**Tags**: `#mermaid`, `#svg`, `#developer-tools`, `#documentation`

---

<a id="item-tech-news-5"></a>
### [Estonia publishes source code of its online voting system](https://github.com/valimised/ivxv) ⭐️ 7.0/10

The Estonian national e‑voting platform \(ivxv\) has been released as open‑source code on GitHub \(https://github.com/valimised/ivxv\). The repository contains the full software stack used for nationwide online elections that have been in operation since 2007, making the code available to security researchers, developers, and policymakers for review and study. This release does not introduce new functionality but provides transparency into a large‑scale, real‑world cryptographic voting system.

hackernews · theanonymousone · Oct 17, 03:18 · [Discussion](https://news.ycombinator.com/item?id=50127586)

**「Estonia’s internet voting background」** Estonia has been conducting internet voting since the early 2000s, initially for local elections and expanding to national parliamentary votes from 2007 onward. The system relies on the national ID card for voter authentication and has retained core cryptographic designs across multiple revisions. The recent GitHub repository makes the IVXV source code publicly available for review, continuing a long‑standing practice of openness in Estonia’s e‑voting infrastructure.

**「Impact」** Security analysts and academic researchers can now directly audit the implementation, potentially uncovering design strengths or weaknesses that inform the development of future e‑voting solutions and standards.

**「Community Discussion」** Commenter cryptonector cautioned that even with open‑source software, election security also depends on trustworthy hardware and firmware, noting that software alone cannot guarantee correct operation of voting machines.

<details><summary>References</summary>
<ul>
<li><a href="https://hal.science/hal-04216242/document">On the Auditability of the Estonian IVXV System and an Attack on...</a></li>
<li><a href="https://github.com/valimised/ivxv">GitHub - valimised/ ivxv : IVXV online voting system · GitHub</a></li>
<li><a href="https://link.springer.com/chapter/10.1007/978-3-031-48806-1_2">On the Auditability of the Estonian IVXV System | Springer Nature Link</a></li>

</ul>
</details>

**Tags**: `#e‑voting`, `#open‑source`, `#security`, `#cryptography`, `#software‑engineering`

---

<a id="item-tech-news-6"></a>
### [Llmspeed lets developers estimate local LLM performance before buying hardware](https://llmspeed.dev/) ⭐️ 7.0/10

Llmspeed \(llmspeed.dev\) is a newly released web tool that predicts token‑per‑second throughput for a given large language model on specified local hardware, allowing AI engineers to gauge how fast a model will run before purchasing GPUs or CPUs. The service provides benchmark‑derived estimates for a range of models and hardware configurations, and is publicly accessible as of the post date.

hackernews · albinstman · Oct 17, 04:36 · [Discussion](https://news.ycombinator.com/item?id=50127979)

**「Estimating Local LLM Performance」** Running large language models on personal or on‑premise hardware requires enough GPU memory, compute, and appropriate software stacks \(e.g., LM Studio, Ollama\) to achieve acceptable inference speed. Because hardware capabilities vary widely, developers often need a way to predict token‑per‑second throughput before purchasing a GPU or configuring a system. Tools such as the LLM Speed Check estimator provide model‑specific performance predictions based on a device’s specifications, helping users gauge whether a given open‑source model will run locally at a usable speed.

**「Impact」** Developers can use the estimates to size hardware purchases more accurately, potentially avoiding over‑provisioning and reducing upfront costs for LLM deployments.

**「Community Discussion」** Commenters note that benchmark‑based estimates may differ from real‑world workloads, emphasizing the importance of inference‑engine tuning and the rapid pace of software optimizations that can make static numbers quickly outdated.

<details><summary>References</summary>
<ul>
<li><a href="https://lm-calc-azure.vercel.app/">LLM Speed Check - AI Model Performance Estimator</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#performance‑benchmarking`, `#hardware‑selection`, `#inference‑optimization`

---

<a id="item-tech-news-7"></a>
### [China Mobile Hong Kong and Macau Operators Deploy First U6GHz 5G‑A/6G Networks](https://www.hk.chinamobile.com/tc/home/news/20261018pr) ⭐️ 7.0/10

China Mobile Hong Kong \(CMHK\) has built the region’s first U6GHz network, completing test verification at its Mong Kok flagship store, while Macau’s CTM launched one of the world’s first commercial U6GHz scenarios at the MGM Macau venue and CTMO installed a U6G demo base station for field testing. The U6GHz band, described as a key spectrum for 5G‑A and future 6G evolution, enables continuous large bandwidth; CMHK achieved up to 3 Gbps downlink using carrier aggregation, and CTM’s VitaAAU base station claims that 256TRx and RetinaMIMO technologies can match the coverage of existing 5G n78 \(3.5 GHz\) deployments. Both operators say the rollout will serve as a foundation for further 6G development in Hong Kong and Macau.

telegram · zaihuapd · Oct 17, 13:02

**「Prerequisite: 6GHz spectrum auction and band role」** The Upper 6 GHz \(U6GHz\) band, identified as a key spectrum resource for 5G‑Advanced \(5G‑A\) and future 6G, became available after Hong Kong’s 6/7 GHz spectrum auction on 29 November 2024, where China Mobile Hong Kong secured 100 MHz of continuous spectrum. This auction enabled operators to deploy U6GHz networks that can deliver multi‑gigabit speeds through spectrum aggregation and advanced antenna techniques such as 256 TRx and RetinaMIMO.

**「Impact」** Device manufacturers and network equipment vendors will need to add U6GHz RF front‑ends and support for 256TRx/RetinaMIMO to enable smartphones and IoT devices to exploit the higher bandwidth and capacity now available in Hong Kong and Macau.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ecjobsonline.com/news/d/14648/China-Mobile-Hong-Kong-Establishes-Hong-Kong-s-First-U6G-Network/">China Mobile Hong Kong Establishes Hong Kong&#x27;s First U6G Network</a></li>

</ul>
</details>

**Tags**: `#5G`, `#Telecom`, `#Hardware`, `#Network Infrastructure`, `#6GHz`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Berkshire Hathaway invests over $900 million in Bending Spoons](https://www.cnbc.com/2026/10/17/bending-spoons-wants-to-revive-software-castoffs-berkshire-investing.html) ⭐️ 7.0/10

Berkshire Hathaway has invested over $900 million in Bending Spoons, including a disclosed $330 million stake.

rss · CNBC Finance · Oct 17, 15:11

**「Background」** Bending Spoons, which raised about $1.7 billion in its July 2026 IPO and has been acquiring distressed SaaS firms such as Airtable and Miro, previously received a $600 million investment from Berkshire Hathaway at the IPO, and the latest $330 million infusion brings Berkshire’s total stake to roughly 4% of the company.

<details><summary>References</summary>
<ul>
<li><a href="https://investors.bendingspoons.com/newsroom/berkshire-hathaway-invests-further-in-bending-spoons">Berkshire Hathaway invests further $330 million in Bending ...</a></li>
<li><a href="https://www.cnbc.com/2026/10/17/bending-spoons-wants-to-revive-software-castoffs-berkshire-investing.html">Bending Spoons wants to revive software castoffs. Berkshire ...</a></li>

</ul>
</details>

**Tags**: `#M&amp;A`, `#Berkshire Hathaway`, `#SaaS industry`, `#AI impact`

---