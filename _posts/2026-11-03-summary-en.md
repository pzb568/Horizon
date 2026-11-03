---
layout: default
title: "Horizon Summary: 2026-11-03 (EN)"
date: 2026-11-03
lang: en
---

> From 47 items, 13 important content pieces were selected

---

**Technology News**
1. [vllm-project/vllm released v0.33.0rc3](#item-tech-news-1) ⭐️ 8.0/10
2. [Ubuntu LTS Kernels Unpatched for Critical CVE‑2026‑98432 After Three Weeks](#item-tech-news-2) ⭐️ 8.0/10
3. [ChatGPT Share‑Link Vulnerability Fixed After Enabling Account Takeover](#item-tech-news-3) ⭐️ 8.0/10
4. [Wired exposes 400+ AI apps hiding pornographic deepfake features, prompting removals](#item-tech-news-4) ⭐️ 8.0/10
5. [Abu Dhabi signs four agreements with OpenAI for machine‑readable government](#item-tech-news-5) ⭐️ 8.0/10
6. [sgl-project/sglang released v0.5.23](#item-tech-news-6) ⭐️ 7.0/10
7. [Astra claims direct weight editing to boost Qwen model performance](#item-tech-news-7) ⭐️ 7.0/10
8. [Cloudflare halves DNS build delay, cuts memory use by 85%](#item-tech-news-8) ⭐️ 7.0/10
9. [llm 0.37](#item-tech-news-9) ⭐️ 7.0/10
10. [LightMIS: 131K‑parameter medical image segmentation runs 10.5× faster on edge GPU](#item-tech-news-10) ⭐️ 7.0/10
11. [xAI launches Data Bot to give every team an AI data scientist](#item-tech-news-11) ⭐️ 7.0/10

**Technology Blog**
1. [LLMs aren’t superhuman at reading or editing neural network weights](#item-tech-blog-1) ⭐️ 8.0/10

**Financial News**
1. [Texas governor race odds tighten, Abbott leads with 60% chance](#item-finance-news-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [vllm-project/vllm released v0.33.0rc3](https://github.com/vllm-project/vllm/releases/tag/v0.33.0rc3) ⭐️ 8.0/10

vLLM 0.33.0rc3 introduces numerous new models and key infrastructure upgrades, making it a high‑value update for AI/ML developers.

github · khluu · Nov 2, 10:10

**Tags**: `#vLLM`, `#PyTorch`, `#CUDA`, `#LLM inference`, `#Open source`

---

<a id="item-tech-news-2"></a>
### [Ubuntu LTS Kernels Unpatched for Critical CVE‑2026‑98432 After Three Weeks](https://freenode.net/article/ubuntu-lts-kernels-still-unfixed-for-critical-cve-2026-98432) ⭐️ 8.0/10

Ubuntu’s LTS kernel packages still lack a fix for CVE‑2026‑98432, a critical remote‑code‑execution vulnerability in the Linux kernel, nearly three weeks after the issue was disclosed. The Ubuntu security page lists the issue with a “High” priority rather than “Critical,” and no official mitigation or patch has been published.

hackernews · majorchord · Nov 2, 18:39 · [Discussion](https://news.ycombinator.com/item?id=50341462)

**「Prerequisite context」** CVE‑2026‑98432 is a critical remote‑code‑execution flaw in the Linux kernel that lets an attacker run arbitrary code with kernel privileges. Ubuntu normally backports upstream kernel fixes into its LTS releases and issues out‑of‑schedule updates only for vulnerabilities marked “Critical”; the CVE is listed as “High” priority on Ubuntu’s security page, which explains the delayed patch. The flaw has been fixed upstream and Red Hat provides an interim mitigation, but Ubuntu’s kernel packages have not yet incorporated the fix.

**「Impact」** Systems running Ubuntu LTS kernels remain exposed to remote code execution attacks; administrators should apply temporary work‑arounds such as the iptables U32 drop rule suggested in community comments or consider upgrading to a newer kernel from another distribution until Ubuntu releases an official patch.

**「Community Discussion」** Commenters note the absence of any mitigation guidance from Ubuntu and question why the fix is delayed, while one user points out that iptables or nftables rules can drop the exploit traffic as a short‑term defense.

<details><summary>References</summary>
<ul>
<li><a href="https://brandefense.io/security-news/cve-2026-98432-ubuntu-kernel-status/">CVE-2026-98432 Ubuntu Kernel Status - Brandefense</a></li>
<li><a href="https://github.com/soroushneshati/cve-2026-98432-ubuntu-mitigation">GitHub - soroushneshati/cve-2026-98432-ubuntu-mitigation ...</a></li>
<li><a href="https://netest.in/blogsPub/cve-2026-98432-ubuntu-kernel-status-host-triage.html">CVE-2026-98432 Ubuntu Kernel Status &amp; Host Triage - netest.in</a></li>

</ul>
</details>

**Tags**: `#Linux`, `#Security`, `#Ubuntu`, `#Kernel Vulnerability`

---

<a id="item-tech-news-3"></a>
### [ChatGPT Share‑Link Vulnerability Fixed After Enabling Account Takeover](https://www.parameter.ai/labs/we-found-a-gap-at-openai) ⭐️ 8.0/10

Parameter’s research team disclosed a critical vulnerability in ChatGPT’s share‑link feature that allowed an attacker to execute code in a logged‑in user’s session, read private conversations, and exfiltrate the data to an external server. The flaw stemmed from a message‑handling error between the preview function and the chart component. OpenAI patched the issue on October 26, classified it as a P1 severity bug, and paid a $5,000 bounty to the researchers.

telegram · zaihuapd · Nov 2, 10:24

**「ChatGPT share‑link feature and its security model」** ChatGPT provides a “share link” that lets users generate a public URL to preview a conversation without requiring the recipient to log in; the link renders the chat in a sandboxed preview page that processes messages from the conversation and displays charts. The vulnerability arose because the preview page’s message handling between the preview component and the chart widget allowed injected code to execute in the context of a signed‑in user’s session, enabling account takeover. This background explains why the flaw could be triggered simply by opening the link.

**「Impact」** Before the fix, any user who clicked a malicious share link could have their ChatGPT account hijacked, exposing personal data and enabling unauthorized actions; users must ensure they are running the updated client released after October 26 to remain protected.

<details><summary>References</summary>
<ul>
<li><a href="https://rrtechpulse.com/stories/chatgpt-shared-link-account-flaw/">ChatGPT shared link flaw, fixed Oct. 26 | RR Tech Pulse</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI`, `#ChatGPT`, `#vulnerability`

---

<a id="item-tech-news-4"></a>
### [Wired exposes 400+ AI apps hiding pornographic deepfake features, prompting removals](https://www.wired.com/story/hundreds-of-mundane-ai-apps-are-hiding-abusive-deepfake-features/) ⭐️ 8.0/10

Wired reported that more than 400 AI‑powered apps and websites were secretly delivering pornographic deepfake content. The investigation linked the apps—many presented as pet‑portrait generators or language‑learning tools—to a Hong‑Kong‑registered operator and found that they could, under certain triggers, load a page that let users upload photos to generate explicit images or videos. After the report, Apple removed 19 of the apps from its store, Google had already taken down most of the remaining ones, and Meta blocked advertising for 209 of the apps.

telegram · zaihuapd · Nov 2, 12:45

**「Background」** Deepfake technology can generate realistic synthetic images and videos, and has previously been embedded covertly in consumer apps—such as the hidden deep‑fake maker discovered in TikTok’s code by researchers \(see CellularNews\). This background explains why a network of seemingly benign AI tools could exploit the same technique to serve pornographic content without users’ knowledge.

**「Impact」** App developers whose products rely on remotely loaded content now face removal from major stores and must implement stricter controls to prevent post‑approval content changes, while users lose access to those apps.

<details><summary>References</summary>
<ul>
<li><a href="https://cellularnews.com/mobile-apps/bytedance-hides-deepfake-maker-feature-within-tiktok-code/">ByteDance Hides Deepfake Maker Feature Within... | CellularNews</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#deepfake abuse`, `#app store policy`, `#security`

---

<a id="item-tech-news-5"></a>
### [Abu Dhabi signs four agreements with OpenAI for machine‑readable government](https://thenextweb.com/news/openai-abu-dhabi-deals-machine-readable-government-mubadala) ⭐️ 8.0/10

Abu Dhabi signed four multi‑year agreements with OpenAI, including a &quot;machine‑readable government&quot; initiative that converts regulations and licences into AI‑readable formats. The pilot, already running on food‑import permits, lets officials query AI for verification while retaining final decision authority. Separate deals involve Mubadala and G42’s Inception42 collaborating on investment‑analysis tools, a five‑year contract to supply models to UAE government, enterprises and schools, and ADNOC becoming the first energy firm to use OpenAI’s Frontier platform.

telegram · zaihuapd · Nov 2, 15:55

**「Prerequisite concept」** Machine‑readable government involves converting statutes, regulations and licensing rules into structured data that AI models can parse and reason over, a practice previously limited to pilot compliance databases. Abu Dhabi’s Department of Government Enablement is extending this approach by partnering with OpenAI to translate its policies into AI‑readable format, launching the world’s first AI‑native “Machine‑Readable Government” initiative alongside four broader agreements.

**「Impact」** Government departments in Abu Dhabi will need to adopt the new AI‑readable policy format and integrate OpenAI APIs to automate permit checks, potentially speeding up approvals and reducing manual review workload.

<details><summary>References</summary>
<ul>
<li><a href="https://rrtechpulse.com/stories/abu-dhabi-openai-four-agreements/">OpenAI Abu Dhabi : 4 agreements signed | RR Tech Pulse</a></li>
<li><a href="https://www.khaleejtimes.com/uae/abu-dhabi-crown-prince-openai-altman-4-deals-key-sectors">Abu Dhabi Crown Prince meets OpenAI &#x27;s Sam Altman... | Khaleej Times</a></li>

</ul>
</details>

**Tags**: `#AI governance`, `#OpenAI partnerships`, `#Government technology`, `#Enterprise AI`, `#Middle East tech`

---

<a id="item-tech-news-6"></a>
### [sgl-project/sglang released v0.5.23](https://github.com/sgl-project/sglang/releases/tag/v0.5.23) ⭐️ 7.0/10

sglang v0.5.23 introduces many new models and shows active community involvement, offering useful tools for AI developers.

github · Fridge003 · Nov 2, 22:14

**Tags**: `#LLM`, `#Diffusion`, `#Open-source`, `#ModelRelease`

---

<a id="item-tech-news-7"></a>
### [Astra claims direct weight editing to boost Qwen model performance](https://rikiyat.github.io/blog/weight-space-programming/) ⭐️ 7.0/10

A blog post introduced a technique called Astra that purportedly reads and writes the weights of the Qwen large language model to improve its abilities, such as math performance. The claim is based on the authors’ experiments and has not been independently verified, and the post acknowledges that the results are still debated within the community.

hackernews · dbreunig · Nov 2, 18:21 · [Discussion](https://news.ycombinator.com/item?id=50341174)

**「Weight Editing Background」** Weight‑space programming is a technique that directly reads and modifies a language model’s parameters instead of using prompts, and it has been demonstrated in recent research. Earlier work such as the “Sparks of Weight‑Space Programming” blog and the Astra‑WeightEdit experiments on Qwen 3.5‑0.8B showed that specific weight “knobs” can be identified and altered to boost capabilities like math reasoning. These prior demonstrations provide the technical foundation for Astra’s claim to read and write weights to improve Qwen.

**「Impact」** If Astra’s weight‑editing approach proves reliable, AI engineers could fine‑tune or enhance specific capabilities of LLMs without full retraining, potentially reducing compute costs and development time, though current evidence is limited.

**「Community Discussion」** Commenters expressed mixed reactions: one user warned the blog overstates results and urged reading the underlying paper, another praised the apparent 5× math improvement, while others suggested the capability may stem from training on weight data rather than a new emergent ability.

<details><summary>References</summary>
<ul>
<li><a href="https://rikiyat.github.io/blog/weight-space-programming/">Sparks of Weight - Space Programming : LLMs can natively read...</a></li>
<li><a href="https://huggingface.co/JonathanColetti/Qwen3.5-0.8B-Astra-WeightEdit">JonathanColetti/ Qwen 3.5-0.8B- Astra -WeightEdit · Hugging Face</a></li>
<li><a href="https://cryptobriefing.com/gpt-6-astra-edits-qwen-weights-math/">GPT-6 Astra reportedly boosts Qwen 3.5-0.8B math up to sixfold by...</a></li>

</ul>
</details>

**Tags**: `#weight-editing`, `#LLM`, `#Qwen`, `#AI-tools`

---

<a id="item-tech-news-8"></a>
### [Cloudflare halves DNS build delay, cuts memory use by 85%](https://blog.cloudflare.com/dns-targeted-zone-builds/) ⭐️ 7.0/10

Cloudflare’s engineering team announced that they have reduced the time required to build DNS zones by 50% and lowered the memory consumption of the process by 85% through targeted optimizations. The improvements apply to Cloudflare’s internal DNS zone‑build pipeline and are now live in production, affecting all zones managed by the service.

hackernews · wondersky · Nov 2, 14:47 · [Discussion](https://news.ycombinator.com/item?id=50337558)

**「Background」** Previously, any change to a zone setting at Cloudflare triggered a full rebuild of the entire DNS zone, even for zones with tens of millions of records, leading to high memory consumption and long build times. This architecture meant that incremental updates still required processing the whole zone, which limited scalability and efficiency. The new targeted build planner changes this by rebuilding only the parts of a zone that actually changed, enabling substantial reductions in memory use and build latency.

**「Impact」** The lower latency and memory footprint allow Cloudflare to process more zone‑build operations on the same hardware, decreasing operational costs and freeing resources for additional workloads on edge servers.

**「Community Discussion」** Commenters noted that the reported rate of roughly 700 zone changes per second seemed low for Cloudflare’s scale, questioning whether the optimization fully addresses their massive domain portfolio.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/dns-targeted-zone-builds/">How we halved DNS build delay and cut memory use by 85%</a></li>

</ul>
</details>

**Tags**: `#DNS`, `#PerformanceOptimization`, `#CloudInfrastructure`

---

<a id="item-tech-news-9"></a>
### [llm 0.37](https://simonwillison.net/2026/Nov/2/llm/) ⭐️ 7.0/10

Simon Willison’s llm 0.37 release introduces new model options, improved endpoint configuration, and broader embedding support, offering useful upgrades for LLM‑focused developers.

rss · Simon Willison · Nov 2, 23:49

**Tags**: `#LLM`, `#Python`, `#CLI`, `#OpenAI-compatible`, `#Embeddings`

---

<a id="item-tech-news-10"></a>
### [LightMIS: 131K‑parameter medical image segmentation runs 10.5× faster on edge GPU](https://www.reddit.com/r/MachineLearning/comments/1xm8dbo/lightmis_ultralightweight_medical_image/) ⭐️ 7.0/10

LightMIS is a 2‑D binary medical image segmentation model with only 131 K parameters that aggregates multi‑scale encoder features without a learned decoder. Compared with nnWNet, it uses 98.14 % fewer parameters and 94.58 % fewer GFLOPs while achieving almost the same modality‑macro Dice and IoU scores under the nnU‑Net v2.3.1 protocol. On an Arm Mali‑G52 MC2 GPU, the full model runs about 10.5× faster than nnWNet and achieves 100 % GPU operator coverage, eliminating CPU fallback. The code, checkpoints, and training details are publicly released for reproducibility.

reddit · r/MachineLearning · /u/OkLion2068 · Nov 2, 20:22

**「Background」** nnU‑Net is an automatically configured biomedical image segmentation framework that standardizes preprocessing, data augmentation, and training hyper‑parameters, and is widely used as a benchmark for new segmentation models. Earlier lightweight architectures such as nnWNet, a transformer‑enhanced encoder‑decoder, have served as reference points but remain relatively large in parameters and FLOPs. LightMIS was trained and evaluated under the same nnU‑Net v2.3.1 protocol to enable a direct comparison with these established models.

**「Impact」** ML engineers can now deploy accurate medical image segmentation on resource‑constrained edge devices, reducing hardware costs and latency while maintaining near‑state‑of‑the‑art performance.

<details><summary>References</summary>
<ul>
<li><a href="https://ieeexplore.ieee.org/abstract/document/11092944">nnWNet: Rethinking the Use of Transformers in Biomedical ...</a></li>
<li><a href="https://github.com/Yanfeng-Zhou/nnWNet">GitHub - Yanfeng-Zhou/nnWNet: [CVPR 2025] nnWNet: Rethinking ...</a></li>

</ul>
</details>

**Tags**: `#medical-imaging`, `#edge-computing`, `#lightweight-models`, `#segmentation`

---

<a id="item-tech-news-11"></a>
### [xAI launches Data Bot to give every team an AI data scientist](https://x.ai/news/data-bot) ⭐️ 7.0/10

xAI announced the Data Bot, a new AI assistant built into its Grok Bot platform that can query a team‑maintained shared skill data warehouse, run analyses, and generate charts or reports according to user preferences. The bot also integrates with Slack, where it can join channels and proactively participate in discussions. xAI says the bot performed roughly 70 hours of work last week that would otherwise have required a human data scientist. This is an announced capability, not an independently verified measurement.

telegram · zaihuapd · Nov 3, 02:44

**「Prerequisite concepts」** Data Bot is built on xAI&\#x27;s Grok Bot platform, which already supports Team Bots that act as shared AI teammates that learn as they work. These bots use shared, read‑only credentials to query approved tables in a Databricks data warehouse and can generate analyses, charts, or reports via natural‑language queries. This existing Grok Bot capability enables Data Bot to automate routine data‑science tasks for any team, reducing the workload that would otherwise fall to human data scientists.

**「Impact」** Teams that adopt Data Bot can offload routine data‑science tasks to the assistant, potentially reducing the time spent by human data scientists on queries and report generation and freeing them for higher‑value work. Organizations will need to configure the shared skill repository and Slack integration to use the bot effectively.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unite.ai/xai-introduces-data-bot-to-bring-shared-analytics-skills-to-grok-bot/">xAI Introduces Data Bot to Bring Shared Analytics Skills to ...</a></li>
<li><a href="https://x.ai/news/data-bot">Giving every team a data scientist with Grok Bot | SpaceXSI</a></li>
<li><a href="https://x.ai/news/team-bots">Team Bots: shared AI teammates that learn as they work</a></li>

</ul>
</details>

**Tags**: `#AI`, `#DataScience`, `#CollaborationTools`, `#Bots`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [LLMs aren’t superhuman at reading or editing neural network weights](https://seangoedecke.com/llms-are-not-superhuman-at-reading-and-writing-neural-network-weights/) ⭐️ 8.0/10

rss · Sean Goedecke · Nov 3, 00:00

**「Background」** A recent paper claims that a frontier LLM \(GPT‑6 Astra\) can directly read and edit neural‑network weights, presenting the ability as superhuman. The authors highlight tasks such as identifying the game a tiny network was trained on and improving a 0.8 B Qwen model’s math performance by weight manipulation.

**「Solution」** The rebuttal shows that the game‑identification task is trivial because the network’s input channels are explicitly labeled and correspond to each 8×8 grid cell, allowing a three‑line Python heatmap to reveal the relevant regions; any attentive researcher could infer the game from that visualization. The Qwen improvement, meanwhile, targets a specific looping bug that appears after 32 k tokens, not a fundamental math deficiency, and is fixed by a “steering” procedure—writing looping and non‑looping texts, measuring residual differences, and ablating the top‑contributing weights—a technique already known to competent ML engineers. This mirrors the “Heretic abliteration” playbook rather than a novel, general‑purpose weight‑editing capability. Consequently, while Astra can perform the weight updates, the process is analogous to an LLM emitting machine code: an impressive trick that still relies on conventional programming or training pipelines for robust development.

**「Takeaway」** Weight‑reading and -editing by LLMs are clever hacks but not a transformative, superhuman ability; future AI research will continue to depend on standard training and human‑guided methods rather than direct weight manipulation.

**Tags**: `#LLM weight manipulation`, `#Neural network interpretability`, `#AI research methodology`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Texas governor race odds tighten, Abbott leads with 60% chance](https://www.cnbc.com/2026/11/02/texas-governor-prediction-markets-abbott-hinojosa.html) ⭐️ 7.0/10

Prediction markets put Gov. Greg Abbott at a 60% chance of winning Texas’s gubernatorial race, while Democratic challenger Gina Hinojosa’s odds have risen to about 40%.

rss · CNBC Finance · Nov 2, 21:13

**「Context on Texas data‑center policy」** Governor Greg Abbott had promoted a $40 billion Google data‑center investment in Texas in November 2025, but in August 2026 ordered an audit and halted all new data‑center permits, shifting his stance on the industry.

**「Impact」** The halt of all data‑center permits and a proposed moratorium could delay AI data‑center projects and affect investors in that sector.

<details><summary>References</summary>
<ul>
<li><a href="https://gov.texas.gov/news/post/governor-abbott-google-announce-40-billion-investment-in-texas">Governor Abbott, Google Announce $40 Billion Investment In Texas</a></li>

</ul>
</details>

**Tags**: `#politics`, `#prediction‑markets`, `#AI‑data‑centers`, `#Texas‑economy`

---