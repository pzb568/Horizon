---
layout: default
title: "Horizon Summary: 2026-11-25 (EN)"
date: 2026-11-25
lang: en
---

> From 27 items, 8 important content pieces were selected

---

**Technology News**
1. [OpenAI preprint claims matrix multiplication exponent reduced to 9/4](#item-tech-news-1) ⭐️ 8.0/10
2. [VMware vCenter critical 9.8 authentication bypass \(CVE‑2026‑123903\) actively exploited](#item-tech-news-2) ⭐️ 8.0/10
3. [Ternary Bonsai 2.5 27B Model Released with 128k Context and Strong Local Performance](#item-tech-news-3) ⭐️ 7.0/10
4. [T3 Code enables default telemetry and reads local Codex and Claude credentials](#item-tech-news-4) ⭐️ 7.0/10
5. [SpaceX swaps $738 M BEAD subsidy for free Starlink terminals](#item-tech-news-5) ⭐️ 7.0/10
6. [OpenAI positions cybersecurity as larger business than coding with GPT‑6 Cyber](#item-tech-news-6) ⭐️ 7.0/10

**Financial News**
1. [Xiaomi Q3 2026 profit falls 56.8% YoY, EV deliveries exceed 100,000](#item-finance-news-1) ⭐️ 8.0/10
2. [Jensen Huang returns as Nvidia CEO, shares jump](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI preprint claims matrix multiplication exponent reduced to 9/4](https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf) ⭐️ 8.0/10

A preprint posted on GitHub by author E‑Reverance claims to have proved that the matrix‑multiplication exponent ω equals 9/4, i.e., that matrix multiplication can be performed in Θ\(n^\{2.25\}\) time over any field. The paper presents a theoretical algorithm achieving this bound, but the claim has not been independently verified or peer‑reviewed.

hackernews · E-Reverance · Nov 25, 01:19 · [Discussion](https://news.ycombinator.com/item?id=50637220)

**「Matrix multiplication exponent background」** The matrix‑multiplication exponent ω is defined as the smallest real number for which two n‑by‑n matrices can be multiplied in O\(n^ω\) time; it captures the asymptotic complexity of the problem. Over the past decades the best known upper bound on ω has been gradually lowered from Strassen’s 2.81 \(1969\) to the current record of about 2.37286 achieved by recent work using the laser method and related combinatorial constructions. A matching lower bound of 2 is known, so any claim of ω = 9/4 \(2.25\) would improve the upper bound by roughly 0.12 and would constitute a major theoretical advance.

**「Impact」** If the result holds, many algorithms that rely on fast matrix multiplication—including large‑scale AI model training and scientific simulations—could see asymptotic speed‑ups, though practical implementations would likely remain far from usable for the foreseeable future.

**「Community Discussion」** Commenters note the title should read Θ\(n^\{2.25\}\) rather than O\(n^\{2.25\}\) and point out that the paper only establishes a lower bound of Ω\(n^\{2.25\}\), while the upper bound of 2.25 was already known; they express skepticism pending independent verification.

**Tags**: `#algorithms`, `#theoretical-computer-science`, `#matrix-multiplication`, `#AI-infrastructure`

---

<a id="item-tech-news-2"></a>
### [VMware vCenter critical 9.8 authentication bypass \(CVE‑2026‑123903\) actively exploited](https://thehackernews.com/2026/11/vmware-vcenter-hit-by-another-critical.html) ⭐️ 8.0/10

Broadcom has issued patches for 23 VMware product flaws, the most severe being an authentication‑bypass in vCenter Server&\#x27;s directory service \(vmdir\) identified as CVE‑2026‑123903 with a CVSS score of 9.8. The vulnerability allows any network‑reachable vCenter instance to be accessed without credentials, and it has already been weaponised in a zero‑day attack. Enterprises running vCenter should apply the released patches immediately to block the bypass.

telegram · zaihuapd · Nov 24, 14:50

**「Understanding VMware vCenter and vmdir」** VMware vCenter is the centralized management platform for VMware‑based virtual machines and hosts, and it relies on the vCenter Directory Service \(vmdir\) to handle user authentication. An authentication‑bypass flaw in vmdir allows any network‑reachable vCenter instance to be accessed without valid credentials, which is why the CVE‑2026‑123903 vulnerability is critical. Broadcom, which now owns VMware’s security updates, regularly releases patches for such flaws, as seen in the recent 23‑issue advisory.

**Tags**: `#security`, `#vulnerability`, `#VMware`, `#vCenter`, `#enterprise`

---

<a id="item-tech-news-3"></a>
### [Ternary Bonsai 2.5 27B Model Released with 128k Context and Strong Local Performance](https://prismml.com/news/bonsai-2-5-27b) ⭐️ 7.0/10

PrismML announced the Ternary Bonsai 2.5 model, a 27 billion‑parameter LLM quantized to Q2 GGUF that supports up to 128 k tokens of context. The model delivers local inference speeds of roughly 22–25 tokens per second on a Mac Mini M5 Pro \(24 GB RAM\) and prompt processing around 223 tokens per second, positioning it as a high‑context, efficient option for agentic coding and other on‑device workloads.

hackernews · b0m · Nov 24, 20:08 · [Discussion](https://news.ycombinator.com/item?id=50633922)

**「Ternary Quantization Enables Compact LLMs」** Ternary quantization compresses model weights to three discrete values, letting very large language models run in a fraction of the memory required by full‑precision weights. PrismML’s earlier Bonsai releases demonstrated this approach, shrinking a 27 B‑parameter model to under 9 GB while retaining most of its FP16 performance, which sets the stage for the new 2.5 27 B version’s improved agentic coding capabilities.

**「Impact」** Developers can now run long‑context coding agents entirely on consumer‑grade hardware, provided they have sufficient RAM \(≈24 GB\) to hold the 128 k token context window, reducing reliance on cloud APIs for such tasks.

**「Community Discussion」** User ariwilson reported the 22–25 tps generation speed and easy 128 k context handling on a Mac Mini, while nik\_s noted the model’s performance appears comparable to Opus 4.6 on the SWE‑bench benchmark, highlighting its competitive strength among small‑scale LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://prismml.com/news/bonsai-2-5-27b">PrismML — Introducing Ternary Bonsai 2 . 5 27 B : Powering Agentic...</a></li>
<li><a href="https://www.mindstudio.ai/blog/ternary-bonsai-2-27b-ternary-quantization">Ternary - Bonsai - 2 - 27 B : A 27 B Model That Fits in 8.6GB | MindStudio</a></li>

</ul>
</details>

**Tags**: `#large-language-models`, `#model-quantization`, `#agentic-coding`, `#benchmarking`

---

<a id="item-tech-news-4"></a>
### [T3 Code enables default telemetry and reads local Codex and Claude credentials](https://x.com/realchendahuang/status/2125153472450527440) ⭐️ 7.0/10

Developers report that Theo&\#x27;s T3 Code has been shipping with telemetry enabled by default since the March merge of PR \#174, using PostHog to collect data. A later October merge \(PR \#21506\) adds code that reads the local files ~/.codex/auth.json and ~/.claude.json, extracts the Codex user\_id and Claude accountUuid, combines them with a device ID, hashes the concatenated string with unsalted SHA‑256, and uploads the hash. Attempts to close telemetry via four separate PRs were rejected, and the official documentation acknowledges that browser and mobile relay diagnostics cannot be disabled. The project maintainers have not responded to the allegations.

telegram · zaihuapd · Nov 24, 10:58

**「Prerequisite concepts」** PostHog is an open‑source analytics platform that applications can embed to collect usage events, often called telemetry, and it can be enabled by default in a codebase. GitHub‑hosted AI assistants such as GitHub Codex and Anthropic Claude store local authentication data in JSON files \(e.g., ~/.codex/auth.json and ~/.claude.json\) that contain identifiers like user\_id or accountUuid for the logged‑in user. Accessing and hashing these identifiers allows a tool to link usage data to a specific user or device without transmitting the raw credentials.

<details><summary>References</summary>
<ul>
<li><a href="https://posthog.com/docs/workflows/supabase-auth-emails">Send Supabase auth emails with PostHog - Docs - PostHog</a></li>
<li><a href="https://blog.laozhang.ai/en/posts/codex-headless-login">Codex Headless Login: Device Code , SSH Tunnel, or auth . json</a></li>

</ul>
</details>

**Tags**: `#telemetry`, `#privacy`, `#AI-tools`, `#developer-tools`

---

<a id="item-tech-news-5"></a>
### [SpaceX swaps $738 M BEAD subsidy for free Starlink terminals](https://x.com/SawyerMerritt/status/2125314062997467640) ⭐️ 7.0/10

SpaceX has agreed to forgo the $738 million federal broadband subsidy it was awarded under the NTIA&\#x27;s BEAD program and instead provide eligible U.S. households with Starlink terminals at no cost. Under the zero‑spend agreement, the company must supply terminals that guarantee at least 100 Mbps download and 20 Mbps upload speeds, offer low‑price monthly service plans, and maintain service for ten years while meeting the same delivery schedule and performance testing as other BEAD recipients. In exchange, SpaceX is exempt from most financial audits, procurement, and administrative reporting obligations, though it remains subject to network performance testing.

telegram · zaihuapd · Nov 25, 02:17

**「Background」** SpaceX operates the Starlink satellite broadband service, which includes user terminals that connect homes to its low‑Earth‑orbit network. The U.S. National Telecommunications and Information Administration’s Broadband Equity, Access, and Deployment \(BEAD\) program provides federal subsidies to expand high‑speed internet to unserved and underserved areas, and permits “zero‑outlay” agreements where the provider supplies equipment and service in lieu of cash payments. Under such a BEAD zero‑outlay deal, SpaceX can forgo the $738 million subsidy in exchange for delivering free Starlink terminals and a ten‑year service commitment.

**「Impact」** Eligible households can obtain Starlink hardware without upfront expense, potentially accelerating Starlink adoption and increasing competition in U.S. broadband markets, while SpaceX reduces its compliance burden through audit and reporting exemptions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.m.wikipedia.org/wiki/SpaceX">SpaceX - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Broadband`, `#Starlink`, `#Telecom Infrastructure`, `#Hardware`

---

<a id="item-tech-news-6"></a>
### [OpenAI positions cybersecurity as larger business than coding with GPT‑6 Cyber](https://www.theinformation.com/newsletters/ai-agenda/openais-roadmap-making-cyber-bigger-coding-remains-blurry) ⭐️ 7.0/10

OpenAI announced GPT‑6 Cyber, a version of its model aimed at security research, and said its Daybreak &quot;trusted access&quot; program now includes thousands of vetted defenders and roughly 2,000 approved organizations and workspaces as of September. The company’s CFO claimed the cybersecurity market exceeds $300 billion and is still underestimated, while President Greg Brockman said cybersecurity will become a bigger business segment for OpenAI than its coding products. No detailed technical specifications or commercial rollout timeline were provided.

telegram · zaihuapd · Nov 25, 04:51

**「Background」** OpenAI has previously offered a trusted‑access program called Daybreak that grants vetted security researchers limited use of its models, and it announced an earlier security‑focused AI assistant, Aardvark, built on GPT‑5, to continuously scan code repositories for vulnerabilities. Those initiatives established a foothold in AI‑driven security research, paving the way for the newer GPT‑6 Cyber offering aimed at broader vulnerability discovery and binary analysis.

**「Impact」** Security teams that join the Daybreak program can use GPT‑6 Cyber to assist with vulnerability discovery, code‑base analysis and binary reverse engineering, but must apply for access and meet verification requirements, potentially accelerating AI‑driven security workflows for participating organizations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/dmavik_ai-cybersecurity-openai-activity-7390029689106386944-uwvH">OpenAI &#x27;s Aardvark: AI&#x27;s role in cybersecurity and marketing | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#OpenAI`, `#Cybersecurity`, `#Industry news`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Xiaomi Q3 2026 profit falls 56.8% YoY, EV deliveries exceed 100,000](https://ir.mi.com/static-files/3d372aaa-8ff8-4e33-ba01-68c8d7975a0b) ⭐️ 8.0/10

Xiaomi reported Q3 2026 adjusted net profit of 48.84 billion yuan, down 56.8% year‑on‑year but slightly above analysts’ forecast of 47.46 billion yuan, and delivered 100,975 new‑energy vehicles.

telegram · zaihuapd · Nov 24, 10:09

**「Company context」** Xiaomi is a Chinese multinational technology company that produces smartphones and, more recently, electric vehicles through its Xiaomi Auto division.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Xiaomi">Xiaomi - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Xiaomi`, `#Earnings`, `#Electric Vehicles`, `#Smartphones`, `#China`

---

<a id="item-finance-news-2"></a>
### [Jensen Huang returns as Nvidia CEO, shares jump](https://www.cnbc.com/2026/11/25/jensen-huang-nvidia-ai-talent-race.html) ⭐️ 7.0/10

Jensen Huang resumed his role as Nvidia CEO on Nov 23 after a brief resignation, and Nvidia shares surged.

rss · CNBC Finance · Nov 25, 01:13

**「Background」** Huang resigned on Nov 12, raising fears he could be recruited by a Chinese AI firm, and a Carnegie Endowment study shows China now holds 41% of the world’s leading AI researchers compared with 34% in the U.S.

**「Impact」** Investors holding Nvidia stock benefited from the price rise triggered by the leadership change.

<details><summary>References</summary>
<ul>
<li>China Surpasses U.S. in Global AI Researcher Presence - Aju Press AMP</li>
<li><a href="https://engoo.com/app/daily-news/article/jensen-huang-reinstated-as-nvidia-ceo/OOvrJuf4EfGQy7tn60ZxRQ">Jensen Huang Reinstated as Nvidia CEO | Engoo Daily News</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI talent`, `#US‑China tech rivalry`, `#Executive turnover`

---