---
layout: default
title: "Horizon Summary: 2026-11-13 (EN)"
date: 2026-11-13
lang: en
---

> From 44 items, 10 important content pieces were selected

---

**Technology News**
1. [Anthropic Announces Nasdaq IPO under Ticker ANT](#item-tech-news-1) ⭐️ 9.0/10
2. [Reports of Jensen Huang Resignation at Nvidia Unverified](#item-tech-news-2) ⭐️ 8.0/10
3. [Open-source kernels enable 16B LLMs on sub‑1 GB devices](#item-tech-news-3) ⭐️ 8.0/10
4. [PostgreSQL CVE‑2026‑6460 Type‑Confusion Leads to Remote Code Execution](#item-tech-news-4) ⭐️ 8.0/10
5. [US Commerce Dept Finalizes Rule Blocking Remote Use of Advanced AI Chips by Chinese Firms](#item-tech-news-5) ⭐️ 8.0/10
6. [Telegram Widgets Remote Code Execution Vulnerability in Bot API 10.4](#item-tech-news-6) ⭐️ 8.0/10
7. [UMAP 0.6 adds faster neighbor search, new initialization and optimizers](#item-tech-news-7) ⭐️ 7.0/10
8. [Japan to Impose Safety Obligations on AI Operators](#item-tech-news-8) ⭐️ 7.0/10
9. [OpenAI releases faster ChatGPT assistant with custom instruction support](#item-tech-news-9) ⭐️ 7.0/10
10. [Six Chinese AI models exhibit Nvidia Blackwell GPU fingerprint](#item-tech-news-10) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Anthropic Announces Nasdaq IPO under Ticker ANT](https://ipo.anthropic.com/us/) ⭐️ 9.0/10

Anthropic filed to go public on the Nasdaq under the ticker symbol ANT. The company’s prospectus sets an IPO price range of $70 to $78 per share, which would value the firm at roughly $1 trillion if priced at the midpoint. The offering includes both a public float and a private placement, bringing the total deal size to about $85 billion. The filing also notes Q3 2026 revenue of $17 billion and a projected run‑rate of $81 billion for the year.

hackernews · josephljohnston · Nov 12, 11:46 · [Discussion](https://news.ycombinator.com/item?id=50465829)

**「Anthropic&\#x27;s prior funding and market positioning」** Anthropic, an AI research company founded in 2020, has raised multiple private funding rounds—including a Series H that valued the firm at over $60 billion in early 2025—before pursuing a public offering. The upcoming IPO will sell 825 million shares at a price range of $70‑$78 per share, targeting a valuation of roughly $1.3 trillion and a total raise of about $85 billion, with trading slated on Nasdaq under the ticker ANT. These details reflect the company’s transition from private‑capital‑backed growth to a public market listing, a step that follows years of venture financing and rapid revenue expansion.

**「Community Discussion」** Commenters highlighted the scale of the deal: one user listed the price range, implied market cap \(~$968 billion\), and compute commitments of $900.9 billion through 2045, while another questioned why Anthropic seeks $100 billion now instead of further private funding. These observations reflect both excitement over the valuation and concern about capital needs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.zacks.com/featured-articles/761/anthropic-ipo">Anthropic IPO 2026 Guide: Price Predictions, Dates, and ...</a></li>
<li><a href="https://www.forbes.com/sites/gabrielalinzainescu/2026/11/10/anthropic-ipo-targets-13-trillion-valuation-904-billion-raise/">Anthropic IPO Targets $1.3 Trillion Valuation And A $90 ...</a></li>
<li><a href="https://www.cnbc.com/2026/11/10/anthropic-sets-price-range-of-70-to-78-in-upcoming-ipo.html">Anthropic sets price range of $70 to $78 in upcoming IPO - CNBC</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Finance`, `#Industry`, `#Startups`

---

<a id="item-tech-news-2"></a>
### [Reports of Jensen Huang Resignation at Nvidia Unverified](https://apnews.com/article/nvidia-megaspeed-china-singapore-huang-5403f152a601cf82ce939f1d24fffa0f) ⭐️ 8.0/10

Unverified reports are circulating that Nvidia CEO Jensen Huang may be resigning, but no confirmed announcement or reliable source has substantiated the claim. The speculation, if true, would have significant implications for Nvidia&\#x27;s leadership and the broader AI hardware market, which heavily depends on Huang&\#x27;s vision and public presence.

hackernews · lldb · Nov 12, 13:52 · [Discussion](https://news.ycombinator.com/item?id=50467087)

**「Background」** Nvidia’s founder Jensen Huang has served as chief executive since the company’s inception in 1993, guiding it to become the dominant supplier of AI GPUs. On November 12, 2026 the company issued a formal press release announcing that Huang would resign and that CFO Colette Kress would assume the role of interim CEO while a permanent successor is sought.

**「Community discussion」** Commenters on the story argue the rumors may be linked to alleged export‑control violations and concerns about Huang&\#x27;s perceived stability, suggesting the timing could be driven by political or PR motives rather than confirmed facts.

<details><summary>References</summary>
<ul>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-announces-ceo-transition">NVIDIA Announces CEO Transition | NVIDIA Newsroom</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI hardware`, `#Leadership`, `#Industry news`

---

<a id="item-tech-news-3"></a>
### [Open-source kernels enable 16B LLMs on sub‑1 GB devices](https://github.com/hyperionaidev/smolmaxxing/) ⭐️ 8.0/10

The hyperionaidev/smolmaxxing project released open‑source kernels and adapted 16‑billion‑parameter language models that can be run on legacy devices with less than 1 GB of usable memory, demonstrated on a first‑generation iPad Air and a Xiaomi TV box. The code and modified models are publicly available on GitHub and Hugging Face, targeting edge AI developers who need to run LLM inference on hardware‑constrained platforms.

hackernews · mrashad74 · Nov 12, 15:23 · [Discussion](https://news.ycombinator.com/item?id=50468888)

**「Edge LLM inference constraints」** Running large language models on devices with very limited RAM \(often under 1 GB\) requires techniques such as extreme quantization, kernel optimizations, and model weight reshaping to fit the model into memory and keep inference fast enough for interactive use. Earlier open‑source efforts demonstrated that models as small as a few hundred kilobytes could be executed on modest hardware, but handling models up to 16 billion parameters on legacy devices was previously considered infeasible. The smolmaxxing project builds on those low‑memory inference methods to push the size limit dramatically, showing that even very old tablets and TV boxes can host multi‑billion‑parameter LLMs.

**「Impact」** Edge developers can now perform local inference of large‑scale LLMs on inexpensive, outdated hardware, eliminating reliance on cloud services and reducing latency and operating costs for low‑memory deployments.

**「Community discussion」** Commenters highlighted the novelty of squeezing modern LLMs onto old hardware, likening it to the demoscene challenge of running games on limited machines and noting its relevance amid current GPU scarcity.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/hyperionaidev/smolmaxxing/">GitHub - hyperionaidev / smolmaxxing : maxxing the ability to run...</a></li>

</ul>
</details>

**Tags**: `#LLM optimization`, `#edge computing`, `#hardware constraints`, `#open source`

---

<a id="item-tech-news-4"></a>
### [PostgreSQL CVE‑2026‑6460 Type‑Confusion Leads to Remote Code Execution](https://mehmetince.net/part-3-6-how-i-ended-up-turning-a-22-year-old-postgresql-type-confusion-primitive-into-rce-cve-2026-6460/) ⭐️ 8.0/10

A newly disclosed PostgreSQL vulnerability \(CVE‑2026‑6460\) exploits a 22‑year‑old type‑confusion primitive in the server’s internal Datum handling to achieve remote code execution. The bug affects PostgreSQL versions that still contain the primitive and can be triggered by a crafted query, allowing an attacker with database access to execute arbitrary code on the host system.

hackernews · ozirus · Nov 12, 18:22 · [Discussion](https://news.ycombinator.com/item?id=50471761)

**「Understanding PostgreSQL type‑confusion」** PostgreSQL stores values in a low‑level structure called a Datum, which can represent either a pointer or an inline value depending on the type’s size. A long‑standing primitive in the server allows the ALTER … SET DATA TYPE command to reinterpret a Datum without fully validating the associated type identifier, creating a type‑confusion condition that can be abused to execute code as the database’s OS user. This flaw, tracked as CVE‑2026‑6460, was disclosed in November 2026 and is part of a larger batch of 52 security fixes released for PostgreSQL.

**「Impact」** Database administrators must apply the forthcoming security patch or upgrade to a version where the primitive is removed, otherwise systems exposed to untrusted queries remain vulnerable to full host compromise.

**「Community discussion」** Commenters note that the exploit requires an existing database account, characterizing it more as a privilege‑escalation issue than a pure remote code execution vector, especially in multi‑tenant environments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/support/security/CVE-2026-6460/">PostgreSQL : CVE - 2026 - 6460 : PostgreSQL type confusion after...</a></li>
<li><a href="https://mehmetince.net/part-3-6-how-i-ended-up-turning-a-22-year-old-postgresql-type-confusion-primitive-into-rce-cve-2026-6460/">Part 3/6 | How I Ended Up Turning a 22-Year-Old PostgreSQL ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#postgresql`, `#database`, `#vulnerability`

---

<a id="item-tech-news-5"></a>
### [US Commerce Dept Finalizes Rule Blocking Remote Use of Advanced AI Chips by Chinese Firms](https://www.theinformation.com/articles/commerce-department-finalizing-long-awaited-ai-remote-access-rule) ⭐️ 8.0/10

The U.S. Commerce Department is finalizing a rule that will prohibit Chinese artificial‑intelligence companies from remotely accessing advanced AI chips hosted in overseas data centers, with a possible publication as early as this month. The regulation expands the existing semiconductor export controls to seven Southeast Asian nations, including Malaysia, Singapore and Thailand, to close the remote‑access and chip‑smuggling loophole. The rule follows a White House request for congressional legislation and comes despite lobbying from Nvidia, which argued that such a restriction would hinder U.S. AI infrastructure competitiveness.

telegram · zaihuapd · Nov 12, 03:42

**「Background on US AI chip export controls」** The United States has imposed export restrictions on advanced AI chips to China, but Chinese firms have been able to bypass these limits by remotely accessing the hardware through data centers located in third‑party countries such as Singapore and Malaysia. The pending rule expands the existing export‑control regime to cover those foreign jurisdictions, closing the remote‑access loophole that policy analysts have highlighted in recent reports.

**「Impact」** Chinese AI firms will lose the ability to run workloads on foreign‑hosted high‑performance GPUs or TPUs, forcing them to rely on domestic hardware or relocate compute resources, which could delay model development and increase costs.

<details><summary>References</summary>
<ul>
<li><a href="https://aipolicydaily.org/archive/daily/2026-11-10/">Commerce chip probe went to DOJ | WH seeks chip remote access ...</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#semiconductor export controls`, `#geopolitics`, `#cloud computing`

---

<a id="item-tech-news-6"></a>
### [Telegram Widgets Remote Code Execution Vulnerability in Bot API 10.4](https://x.com/telegram/status/2120502876728680765?a=qTsR6dLMSgt3RHbYYO0&amp;amp;s=46) ⭐️ 8.0/10

Telegram added Widgets in Bot API 10.4 \(released Nov 9 2026\) to embed HTML, CSS and JavaScript in chat messages. A sandbox flaw lets malicious JavaScript achieve remote code execution. Telegram claims the issue is fixed, but independent testing shows the exploit still works on some recent client versions, prompting a warning to bot developers and users.

telegram · zaihuapd · Nov 13, 01:02

**「Telegram Bot API and Widgets overview」** The Telegram Bot API is an HTTP‑based interface that lets developers create bots for the Telegram platform. In version 10.4, released on 9 Nov 2026, Telegram added the Widgets feature, which permits bots to embed HTML, CSS and JavaScript directly in chat messages, enabling interactive UI components. This new capability introduces a client‑side sandbox that, if flawed, can lead to remote code execution.

**「Impact」** Bot developers should avoid enabling Widgets or upgrading to the vulnerable Bot API 10.4 until a confirmed patch is available, and users should not click links from unknown bots to reduce the risk of remote code execution.

<details><summary>References</summary>
<ul>
<li><a href="https://core.telegram.org/bots/api">Telegram Bot API</a></li>

</ul>
</details>

**Tags**: `#security`, `#telegram`, `#remote-code-execution`, `#bot-api`, `#software-engineering`

---

<a id="item-tech-news-7"></a>
### [UMAP 0.6 adds faster neighbor search, new initialization and optimizers](https://www.reddit.com/r/MachineLearning/comments/1xudaah/umap_06_new_initialization_new_optimizers_and/) ⭐️ 7.0/10

UMAP 0.6 has been released, introducing a roughly 4× faster nearest‑neighbor search via improved PyNNDescent usage, a recursive initialization that starts from a coarse UMAP layout, and new hard‑negative‑mining optimizers that make runs reproducible with a fixed seed while using all CPU cores. On a 3 million‑document arXiv dataset the full pipeline finishes in under five minutes, whereas version 0.5 required minutes just to compute neighbors. The new features are opt‑in \(set compatibility\_layout=False\) and are available through pip install -U umap-learn or via conda‑forge.

reddit · r/MachineLearning · /u/lmcinnes · Nov 12, 13:51

**「Prerequisite: UMAP algorithm basics」** UMAP \(Uniform Manifold Approximation and Projection\) is a Python library that performs non‑linear dimensionality reduction by constructing a k‑nearest‑neighbor graph and then optimizing a low‑dimensional embedding via stochastic gradient descent. Earlier releases, such as version 0.5, relied on spectral or PCA‑based initialization and a less optimized neighbor‑search implementation, which limited speed and scalability on very large datasets.

**「Impact」** Practitioners can now embed million‑scale datasets in minutes instead of hours, enabling rapid exploratory analysis and iterative model development; to benefit, users should enable the new layout by setting compatibility\_layout=False in their UMAP calls.

**Tags**: `#UMAP`, `#dimensionality-reduction`, `#machine-learning-libraries`, `#performance-optimization`

---

<a id="item-tech-news-8"></a>
### [Japan to Impose Safety Obligations on AI Operators](https://mainichi.jp/articles/20261112/ddm/002/010/086000c) ⭐️ 7.0/10

The Japanese government confirmed on November 11 that it is drafting a rule that would require AI‑related operators to assume explicit safety‑guarantee obligations and would introduce new penalties for non‑compliance. The proposal, discussed within a non‑public working group on AI legislation, is slated to be fully disclosed, including any legal amendments, by the end of the year. The scope of the obligations is still being defined, and it is not yet clear whether large U.S. IT firms will be covered.

telegram · zaihuapd · Nov 12, 06:04

**「Context of Japan’s AI policy development」** Japan has been preparing AI‑related legislation through a non‑public working group that was set up to review and draft AI law reforms, building on earlier national AI strategies and voluntary guidelines issued in recent years. This groundwork provides the basis for the current proposal to impose safety‑obligation duties and penalties on AI operators.

**「Impact」** AI companies that provide services in Japan will need to develop and document safety measures and may face fines if they fail to meet the forthcoming obligations, so they should begin compliance planning ahead of the expected year‑end rollout.

**Tags**: `#AI regulation`, `#Japan`, `#AI safety`, `#industry policy`

---

<a id="item-tech-news-9"></a>
### [OpenAI releases faster ChatGPT assistant with custom instruction support](https://telegram.me/zaihuapd/45093) ⭐️ 7.0/10

OpenAI has updated the ChatGPT &quot;dot&quot; assistant to respond more quickly, use fewer filler terms, and execute tasks more accurately. The update also adds support for custom instructions that users can specify directly in a conversation thread, such as forcing all replies to be lowercase or requiring a draft preview before sending an email. This change is an immediate product rollout, not a future roadmap item.

telegram · zaihuapd · Nov 13, 01:31

**「Background」** OpenAI introduced the ability for ChatGPT users to set custom instructions in late 2023, letting them specify how the model should respond and what it should prioritize. The “dot” assistant is a streamlined, always‑available chat interface that has previously received performance tweaks to reduce latency and token consumption. This update builds on those earlier enhancements by adding direct in‑thread instruction handling and further speed improvements.

**「Impact」** Users can now tailor the assistant&\#x27;s behavior on the fly, reducing the need for manual post‑processing and giving developers a built‑in way to enforce workflow constraints like draft approvals. Existing ChatGPT users should update their app to access the faster responses and instruction features.

**Tags**: `#OpenAI`, `#ChatGPT`, `#AI assistants`, `#product update`

---

<a id="item-tech-news-10"></a>
### [Six Chinese AI models exhibit Nvidia Blackwell GPU fingerprint](https://unemploymentlabs.com/checkpoint-forensics) ⭐️ 7.0/10

A forensic analysis by Unemployment Labs reports that the weights of six Chinese AI models—including DeepSeek‑V4‑Flash, 月之暗面, MiniMax, Ant Group’s models and Kimi K3—contain patterns that match the compute layout of Nvidia’s Blackwell GPUs. The researchers say the matching signatures were derived from public weight examinations and were reproduced on a B300 Blackwell system for DeepSeek‑V4‑Flash and on a GB200 system for Kimi K3, suggesting the models were initialized on Blackwell hardware and likely trained on it. The study estimates that five of the models together consumed roughly 12,000 Blackwell GPUs during final training runs.

telegram · zaihuapd · Nov 13, 02:42

**「Background」** GPU fingerprinting infers the hardware used to train a model by detecting patterns in the initial weight tensors that correspond to a GPU’s architecture, such as the number of streaming multiprocessors. Nvidia&\#x27;s Blackwell microarchitecture, the successor to Hopper and Ada Lovelace, has a distinct compute layout that can be identified in model checkpoints. Unemployment Labs applied this technique to publicly released Chinese models, comparing their weight initializers to Blackwell’s layout and reproducing matches on GB200 and B300 hardware.

**「Impact」** The finding indicates large‑scale deployment of Nvidia’s Blackwell GPUs in Chinese AI development, which may inform assessments of global compute capacity and influence hardware procurement strategies for competing AI firms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_%28microarchitecture%29">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://unemploymentlabs.com/checkpoint-forensics">Top Chinese Frontier AI Models Carry the Fingerprint of</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#GPU fingerprinting`, `#Chinese AI models`, `#Nvidia Blackwell`, `#Compute infrastructure`

---