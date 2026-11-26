---
layout: default
title: "Horizon Summary: 2026-11-26 (EN)"
date: 2026-11-26
lang: en
---

> From 35 items, 8 important content pieces were selected

---

**Technology News**
1. [Anthropic reduces GRH Lean proof from 17 M to 76 k lines](#item-tech-news-1) ⭐️ 8.0/10
2. [OpenAI positions cybersecurity as larger business than coding with GPT‑6 Cyber](#item-tech-news-2) ⭐️ 8.0/10
3. [OpenAI Begins Private Inference Service Test for Select Enterprise Customers](#item-tech-news-3) ⭐️ 8.0/10
4. [Ubuntu security patches lag behind, prompting concerns](#item-tech-news-4) ⭐️ 7.0/10
5. [Asian Data Centers Shift AI Compute Sales to US After US Tightens Chip Export Loophole](#item-tech-news-5) ⭐️ 7.0/10
6. [Anthropic CEO Dario Amodei denies giving human free will to AI, calls for democratic oversight](#item-tech-news-6) ⭐️ 7.0/10

**Financial News**
1. [US to add new Section 301 tariffs on 14 partners, 20% extra on China](#item-finance-news-1) ⭐️ 9.0/10
2. [iQIYI receives Nasdaq non‑compliance notice, 180‑day deadline to fix](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Anthropic reduces GRH Lean proof from 17 M to 76 k lines](https://github.com/lsernau/grh-lean) ⭐️ 8.0/10

Anthropic&\#x27;s AI‑driven techniques have compressed the Lean formalization of the Generalized Riemann Hypothesis from roughly 17 million lines to about 76 thousand lines, a reduction of over 99.5%. The new version is organized with clear &quot;known math&quot; versus &quot;new math&quot; sections and extensive human‑readable documentation, making the proof far more approachable for formal verification researchers. This result demonstrates a concrete advance in using large language models to streamline massive formal proofs.

hackernews · nb-t · Nov 25, 21:48 · [Discussion](https://news.ycombinator.com/item?id=50648050)

**「Background」** The Generalized Riemann Hypothesis \(GRH\) has been formalized in the Lean 4 proof assistant, originally requiring over 17 million lines of code. Anthropic’s recent release provides two Lean projects— a readable edition of roughly 300 k lines and a compact edition of about 76 k lines—both built with Lean v4.35.0 and a specific Mathlib commit, dramatically shrinking the proof size.

**「Reduced proof size eases verification effort」** Shrinking the GRH Lean proof from about 17 million to 76 000 lines cuts the proof size by over 99%, dramatically lowering the manual effort needed to review, maintain, and extend such large formalizations and making AI‑assisted formal verification more practical for extensive mathematical results.

**「Community discussion」** Commenters highlighted the practical benefits: one noted the proof is now more readable with a clear split between established and novel mathematics, while another quantified the line‑count reduction, and a third asked whether this undermines concerns about large, opaque proofs lacking insight.

<details><summary>References</summary>
<ul>
<li><a href="https://stackfutures.com/blog/anthropic-riemann-lean-proof-17m-to-76k-lines-shorter-grh-nov-2026/">The Riemann Hypothesis Lean Proof Just Shrank From 17 Million ...</a></li>
<li><a href="https://ashutoshai.com/ai-compass/2026/11/25/anthropic-compact-lean-4-grh-proofs/">Anthropic releases 76k-line compact Lean 4 proofs of RH and GRH</a></li>
<li><a href="https://ai-tldr.dev/releases/anthropic-grh-lean-short-proof/">GRH in Lean — Anthropic staff and Claude shrink… | AI/TLDR</a></li>
<li><a href="https://dev.to/technoblogger14o3/ai-will-make-formal-verification-go-mainstream-9g3">AI will make formal verification go mainstream - DEV Community</a></li>

</ul>
</details>

**Tags**: `#formal verification`, `#Lean`, `#AI-assisted proofs`, `#software engineering`

---

<a id="item-tech-news-2"></a>
### [OpenAI positions cybersecurity as larger business than coding with GPT‑6 Cyber](https://www.theinformation.com/newsletters/ai-agenda/openais-roadmap-making-cyber-bigger-coding-remains-blurry) ⭐️ 8.0/10

OpenAI announced that cybersecurity will become its biggest business segment, overtaking its coding products, and its CFO said the market size of over $300 billion is still underestimated. The company has launched GPT‑6 Cyber for security research and is expanding its Daybreak trusted‑access program, which by September 2026 covered thousands of vetted defenders and roughly 2,000 approved organizations and workspaces for tasks such as vulnerability discovery, code‑base analysis, and binary reverse engineering. These moves signal a strategic shift toward AI‑driven security tools, though access remains limited to participants in the Daybreak program.

telegram · zaihuapd · Nov 25, 04:51

**「Prerequisite context」** OpenAI previously introduced the Daybreak trusted‑access program, which gives vetted security researchers limited use of its models for vulnerability research, and it has built a strong enterprise presence with products such as Codex and GPT‑4 that target software development. The cybersecurity market has long been estimated at over $3 trillion, a figure the company’s CFO says remains underestimated, making the new GPT‑6 Cyber offering a logical extension of its existing AI‑driven tooling.

<details><summary>References</summary>
<ul>
<li><a href="https://xtendedview.com/openai-statistics/">OpenAI Statistics 2026: Users, Revenue, Growth</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Cybersecurity`, `#AI`, `#EnterpriseAI`, `#TechIndustry`

---

<a id="item-tech-news-3"></a>
### [OpenAI Begins Private Inference Service Test for Select Enterprise Customers](https://x.com/sama/status/2125638790593274259) ⭐️ 8.0/10

OpenAI announced that it is piloting a Private Inference service with a small group of enterprise customers. The offering, part of the OpenAI Private Intelligence portfolio, runs under a Zero Data Retention \(ZDR\) model and includes Private Safety Processing that automatically handles safety reviews without OpenAI staff accessing the underlying data. This test phase is limited to a few clients and is not yet a general‑availability product.

telegram · zaihuapd · Nov 26, 01:44

**「Background」** Private inference refers to running AI models on user data without transmitting that data to the provider, thereby keeping the raw inputs confidential. OpenAI previously introduced the OpenAI Private Intelligence suite, which includes zero‑data‑retention \(ZDR\) options and private safety processing that let the model perform safety checks without human review of the underlying content. This prior work underpins the current test of a private inference service for a limited set of enterprise customers.

**「Impact」** Enterprises that join the pilot can evaluate cutting‑edge AI models while keeping their proprietary data completely private, but they must adopt the ZDR workflow and cannot rely on OpenAI personnel for data handling.

**Tags**: `#OpenAI`, `#Private Inference`, `#AI Privacy`, `#Enterprise AI`

---

<a id="item-tech-news-4"></a>
### [Ubuntu security patches lag behind, prompting concerns](https://www.openwall.com/lists/oss-security/2026/11/25/9) ⭐️ 7.0/10

Ubuntu has been reported to delay the release of security patches, leaving users and administrators waiting longer for fixes to known vulnerabilities. The slowdown affects systems that depend on timely updates to maintain security posture.

hackernews · gslin · Nov 25, 20:38 · [Discussion](https://news.ycombinator.com/item?id=50647181)

**「Ubuntu kernel backporting and patch timeline」** Ubuntu LTS releases backport security fixes onto an older kernel series \(e.g., 7.0.0‑44\) rather than adopting newer upstream kernels, which adds an extra integration step before a patch can be released. This backport process can lengthen the time between a vulnerability’s public disclosure and the availability of an Ubuntu security update, especially compared with distributions that ship upstream kernels directly.

**「Impact」** Organizations may shift to alternative distributions such as Debian or adjust their update policies to include non‑security updates, mitigating the risk of unpatched vulnerabilities.

**「Community Discussion」** Several commenters noted they have migrated server images to Debian due to Ubuntu&\#x27;s slower response, while others pointed out that extensive regression testing can cause delays, though they consider the trade‑off necessary.

<details><summary>References</summary>
<ul>
<li><a href="https://www.openwall.com/lists/oss-security/2026/11/25/9">oss-security - Slow Ubuntu security response times</a></li>
<li><a href="https://hn.today/s/slow-ubuntu-security-response-times">Slow Ubuntu security response times - hn.today</a></li>

</ul>
</details>

**Tags**: `#linux`, `#security`, `#ubuntu`, `#open-source`

---

<a id="item-tech-news-5"></a>
### [Asian Data Centers Shift AI Compute Sales to US After US Tightens Chip Export Loophole](https://www.bloomberg.com/news/articles/2026-11-25/asia-data-centers-sound-out-us-clients-to-replace-china-demand) ⭐️ 7.0/10

The United States tightened a loophole that had allowed Chinese technology firms to obtain Nvidia’s most advanced AI accelerators. In response, data‑center operators across Asia with surplus AI compute are actively seeking to sell that capacity to U.S. customers, a shift noted by Liquid Compute CEO Ronit Jain.

telegram · zaihuapd · Nov 25, 11:35

**「Background」** The United States has long restricted exports of its most advanced AI accelerators, such as Nvidia’s H100 GPUs, but a loophole let foreign data‑center operators buy the chips and lease the resulting compute to Chinese firms, effectively sidestepping the controls. Asian data‑center providers built surplus capacity to serve Chinese customers under this arrangement, so the recent tightening of the loophole forces them to seek new buyers, notably U.S. clients.

**「Impact」** Asian providers that previously relied on Chinese clients must now market their excess compute to U.S. buyers, potentially expanding U.S. access to AI‑accelerated resources while reducing Chinese availability.

<details><summary>References</summary>
<ul>
<li><a href="https://epoch.ai/publications/huawei-horinger-china-compute-gap">What Huawei’s Horinger data center reveals about China ’s compute ...</a></li>

</ul>
</details>

**Tags**: `#AI compute`, `#data centers`, `#geopolitics`, `#cloud infrastructure`

---

<a id="item-tech-news-6"></a>
### [Anthropic CEO Dario Amodei denies giving human free will to AI, calls for democratic oversight](https://x.com/DarioAmodei/status/2125656399392690605) ⭐️ 7.0/10

Anthropic CEO Dario Amodei posted on X to refute any claim that he advocated handing human free will over to AI, calling the idea absurd. He reiterated that AI development should be subject to legitimate democratic oversight, and warned that allowing Claude or other models to autonomously create next‑generation systems without substantial human supervision would be unsafe. Amodei also suggested that in scenarios where end‑to‑end AI could cause severe employment disruption, slowing or pausing deployments may be reasonable.

telegram · zaihuapd · Nov 26, 02:27

**「Context of Anthropic’s AI Governance Stance」** Anthropic develops the Claude series of large language models, and its leadership has long participated in debates over how AI should be overseen. Dario Amodei has repeatedly argued that AI must be governed by legitimate democratic institutions rather than by the systems themselves, rejecting claims that the company supports “machine‑led” governance and emphasizing the need for human oversight in recursive self‑improvement scenarios. These positions provide the backdrop for his recent clarification that surrendering human free will to AI is “absurd.”

<details><summary>References</summary>
<ul>
<li><a href="https://interestingengineering.com/ai-robotics/anthropic-ceo-rejects-machine-led-governance">Anthropic CEO rejects giving machines control over human ...</a></li>
<li><a href="https://x.com/DarioAmodei/status/2125656399392690605">Dario Amodei on X: &quot;No, I do not believe that we should ...</a></li>
<li><a href="https://openthemagazine.com/world/anthropic-ceo-says-ai-governance-must-remain-democratic-warns-against-surrendering-human-control">Anthropic CEO Advocates Democratic AI Governance, Warns ...</a></li>

</ul>
</details>

**Tags**: `#AI governance`, `#Anthropic`, `#AI safety`

---

## Financial News

<a id="item-finance-news-1"></a>
### [US to add new Section 301 tariffs on 14 partners, 20% extra on China](https://www.cnbc.com/2026/11/25/us-tariffs-trump-section-301.html) ⭐️ 9.0/10

The United States announced it will levy new Section 301 tariffs on 14 trading partners, including a 20% additional duty on Chinese goods that already face a 25% tariff.

telegram · zaihuapd · Nov 25, 13:59

**「Background」** Section 301 of the 1974 Trade Act gives the USTR authority to impose tariffs to counter foreign trade practices deemed unfair, such as subsidized overcapacity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Section_301_of_the_Trade_Act_of_1974">Section 301 of the Trade Act of 1974 - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#US trade policy`, `#Tariffs`, `#China`, `#EU`, `#International trade`

---

<a id="item-finance-news-2"></a>
### [iQIYI receives Nasdaq non‑compliance notice, 180‑day deadline to fix](https://weibo.com/1640337222/Rt7hFla8e) ⭐️ 7.0/10

iQIYI said it has received a Nasdaq non‑compliance notice and must regain compliance within 180 days to avoid delisting.

telegram · zaihuapd · Nov 26, 04:00

**「Nasdaq minimum bid price rule」** Nasdaq requires listed companies to maintain a closing bid price of at least $1 for 30 consecutive trading days; falling below that triggers a non‑compliance notice and gives the company up to 180 days to regain compliance.

**「Impact」** Shareholders and ADS investors face the risk of losing Nasdaq listing if the company does not meet the requirements within the deadline.

<details><summary>References</summary>
<ul>
<li><a href="https://waterfrontonline.blog/wp-content/uploads/2022/10/delistingrules.pdf">Nasdaq Delisting Rules</a></li>

</ul>
</details>

**Tags**: `#iQIYI`, `#Nasdaq listing`, `#Corporate compliance`, `#Delisting risk`

---