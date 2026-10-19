---
layout: default
title: "Horizon Summary: 2026-10-19 (EN)"
date: 2026-10-19
lang: en
---

> From 34 items, 12 important content pieces were selected

---

**Technology News**
1. [vllm-project/vllm released v0.32.0](#item-tech-news-1) ⭐️ 8.0/10
2. [Hybrid Reasoning Agents Combine Latent‑Space Thinking with Text‑Based Actions](#item-tech-news-2) ⭐️ 8.0/10
3. [Linux kernel CVE‑2026‑99999 enables KVM guest escape, patch merged](#item-tech-news-3) ⭐️ 8.0/10
4. [Google 开源递归智能体框架 Harness²](#item-tech-news-4) ⭐️ 8.0/10
5. [Anthropic pushes AI safety bill limiting shutdowns to extreme damage thresholds](#item-tech-news-5) ⭐️ 8.0/10
6. [DeepSeek launches $0.75 per 1k requests search API](#item-tech-news-6) ⭐️ 7.0/10
7. [TempoPFN: Synthetic Pre-training of Linear RNNs for Zero-shot Time Series Forecasting \[R\]](#item-tech-news-7) ⭐️ 7.0/10
8. [Proof Before Reuse: showing agents only what later sessions reproduced keeps a poisoned skill out of procedural memory \[R\]](#item-tech-news-8) ⭐️ 7.0/10
9. [Anthropic works with law firms to draft AI agent negotiation rules](#item-tech-news-9) ⭐️ 7.0/10
10. [Nvidia vLLM optimization speeds up Kimi K3 inference 1.68×](#item-tech-news-10) ⭐️ 7.0/10

**Financial News**
1. [China adds medical exoskeleton rehab to regional insurance pilots](#item-finance-news-1) ⭐️ 8.0/10
2. [China food‑delivery platforms profit rebound, but merchants and riders face tighter margins](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [vllm-project/vllm released v0.32.0](https://github.com/vllm-project/vllm/releases/tag/v0.32.0) ⭐️ 8.0/10

vllm 0.32.0 introduces new API features and wide low‑precision KV‑cache support, delivering important performance and usability improvements for LLM inference.

github · khluu · Oct 18, 06:50

**Tags**: `#LLM inference`, `#vllm`, `#performance optimization`, `#API updates`

---

<a id="item-tech-news-2"></a>
### [Hybrid Reasoning Agents Combine Latent‑Space Thinking with Text‑Based Actions](https://arxiv.org/abs/2610.18861) ⭐️ 8.0/10

The paper introduces a hybrid agent architecture that lets large language models perform reasoning in a latent‑space representation while still interacting with the world through ordinary text prompts and outputs. The authors release open‑source code \(github.com/togethercomputer/HybridAgent\) and model checkpoints on HuggingFace, and provide early evaluation results showing the approach works on standard reasoning benchmarks. This design is aimed at AI researchers and engineers who want to experiment with agents that can separate internal computation from external communication. The work is presented as a research prototype, not a production‑ready system.

hackernews · allinonai · Oct 18, 20:48 · [Discussion](https://news.ycombinator.com/item?id=50145337)

**「Prerequisite concepts」** LLM agents have typically acted by producing text that is parsed as commands for external tools or as direct responses, a pattern seen in prior tool‑calling frameworks such as ReAct. Latent‑space reasoning refers to performing inference directly on the model’s internal vector embeddings rather than converting thoughts to text first. The new hybrid design builds on these two strands by keeping the reasoning inside the latent representations while still using text for observable actions.

**「Impact」** Developers can now prototype and benchmark hybrid agents using the publicly available repository, potentially accelerating research into more efficient or capable AI agents that combine latent reasoning with text‑based tool use.

**「Community Discussion」** Commenter amluto questions the computational cost, noting that the latent‑mode model runs alongside text generation and suggesting a design that merges the two representations to avoid duplicate expense.

**Tags**: `#LLM agents`, `#latent space reasoning`, `#AI research`, `#agent architectures`

---

<a id="item-tech-news-3"></a>
### [Linux kernel CVE‑2026‑99999 enables KVM guest escape, patch merged](http://pwn.ai/) ⭐️ 8.0/10

PWN.AI researchers disclosed Linux kernel vulnerability CVE‑2026‑99999, which lets a KVM guest rewrite IPv4 header metadata after checksum verification, leaking 32 bytes of host memory and enabling a guest‑to‑host escape. The team demonstrated the escape in their own KVM setup. Linux maintainers merged a fix to the mainline kernel on 14 October 2026.

telegram · zaihuapd · Oct 18, 09:47

**「Prerequisite: KVM and checksum offload trust model」** KVM \(Kernel-based Virtual Machine\) lets Linux run virtual machines with the host kernel handling privileged operations. The disclosed CVE‑2026‑99999 exploits a long‑standing trust‑boundary flaw in the kernel’s networking stack where checksum‑offload metadata \(CHECKSUM\_PARTIAL\) is accepted from a guest after the IPv4 header has already been validated, allowing the guest to rewrite the header and leak host memory. This post‑validation mutation enables the guest to execute code on the host, resulting in a guest‑to‑host escape.

**「Impact」** Systems running vulnerable kernel versions must be updated to the patched release immediately, or risk remote compromise of the host through compromised virtual machines.

<details><summary>References</summary>
<ul>
<li>PwnEscape: Guest-to-Host KVM Escape (CVE-2026-99999) - pwn.ai</li>
<li>PwnEscape Hid in the Kernel Network Stack for 18 Years - TuxCare</li>

</ul>
</details>

**Tags**: `#Linux`, `#KVM`, `#Security`, `#Vulnerability`

---

<a id="item-tech-news-4"></a>
### [Google 开源递归智能体框架 Harness²](https://github.com/google-research/harness2) ⭐️ 8.0/10

Google Research releases Harness², a recursive LLM agent framework with performance improvements and open‑source tooling

telegram · zaihuapd · Oct 18, 11:24

**Tags**: `#LLM`, `#agent-framework`, `#recursive-optimization`, `#open-source`, `#Google-Research`

---

<a id="item-tech-news-5"></a>
### [Anthropic pushes AI safety bill limiting shutdowns to extreme damage thresholds](https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropics-proposed-ai-safety-bill-only-kicks-in-if-50-deaths-or-usd1-billion-in-damages-are-on-the-line-proposal-would-effectively-make-the-commerce-department-the-only-agency-capable-of-stopping-an-ai-model) ⭐️ 8.0/10

Anthropic is lobbying a U.S. AI safety bill that would permit the government to halt the release of an AI model only if the model could cause at least $1 billion in damages or result in 50 or more deaths or injuries. The proposal places the authority to evaluate labs and models with an independent third party registered with the Commerce Department, and restricts any shutdown order to the Commerce Department, with a federal judge making the final decision. The bill also requires a 72‑hour report to the Commerce Department if a model is found to pose bioweapon, AI‑enabled cyber‑attack, or runaway risk. The measure is currently a lobbying effort and has not been enacted into law.

telegram · zaihuapd · Oct 18, 12:40

**「Background」** The United States has been considering AI safety legislation that would allow the federal government to intervene when an artificial‑intelligence model is deemed a serious risk. Existing proposals have generally given multiple agencies the ability to request a model’s suspension, but the current draft would tie that power to specific thresholds of projected damage or casualties.

**「Impact」** If enacted, AI developers and companies would face a higher threshold before regulators could force a model shutdown, concentrating enforcement power in the Commerce Department and potentially limiting rapid intervention in less severe but still harmful scenarios, prompting firms to reassess compliance and risk‑assessment strategies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropics-proposed-ai-safety-bill-only-kicks-in-if-50-deaths-or-usd1-billion-in-damages-are-on-the-line-proposal-would-effectively-make-the-commerce-department-the-only-agency-capable-of-stopping-an-ai-model">Anthropic’s proposed AI safety bill only kicks in if 50 ...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#Regulation`, `#Anthropic`, `#Policy`

---

<a id="item-tech-news-6"></a>
### [DeepSeek launches $0.75 per 1k requests search API](https://api-docs.deepseek.com/guides/search/) ⭐️ 7.0/10

DeepSeek announced a new search API priced at $0.75 for every 1,000 successful requests, positioning it as a low‑cost option for AI and software developers who need web‑search capabilities in their applications. The pricing is presented as a cheaper alternative to existing commercial search APIs such as Brave \($5 per 1k\) and Kagi \($12 per 1k\).

hackernews · fagnerbrack · Oct 18, 06:50 · [Discussion](https://news.ycombinator.com/item?id=50138531)

**「Background」** Search and fetch APIs let applications retrieve web search results or page content programmatically, a capability often used to augment large language models with up‑to‑date information. Prior to DeepSeek’s announcement, mainstream providers such as Brave Search and Kagi charged $5–$12 per 1,000 calls, and Google does not offer a paid search API. DeepSeek’s new endpoints \(/v1/tools/search and /v1/tools/fetch\) are priced at $0.75 per 1,000 successful requests, billing only for HTTP 200 responses with non‑empty results.

**「Impact」** Developers can integrate web search into retrieval‑augmented generation or agent systems at a fraction of the cost of competing services, potentially lowering operating expenses and making such features more accessible for smaller projects.

**「Community discussion」** Commenters noted the price advantage over Brave and Kagi APIs and mentioned free self‑hosted options like searxng‑ai‑kit as even cheaper alternatives for personal use.

<details><summary>References</summary>
<ul>
<li><a href="https://threatfrontier.com/articles/deepseek-search-fetch-api-pricing-october-31">DeepSeek Search and Fetch API Pricing: $0.75 per 1,000</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/deepseek-monetizes-agent-retrieval-layer-185236272.html?fr=sycsrp_catchall">DeepSeek Monetizes the Agent Retrieval Layer at $0.75 per ...</a></li>

</ul>
</details>

**Tags**: `#search API`, `#LLM integration`, `#cost optimization`, `#AI agents`

---

<a id="item-tech-news-7"></a>
### [TempoPFN: Synthetic Pre-training of Linear RNNs for Zero-shot Time Series Forecasting \[R\]](https://www.reddit.com/r/MachineLearning/comments/1x97v19/tempopfn_synthetic_pretraining_of_linear_rnns_for/) ⭐️ 7.0/10

NeurIPS 2026 paper presents a synthetic pre‑training library and linear RNN model for zero‑shot time‑series forecasting, providing a useful new tool for the community.

reddit · r/MachineLearning · /u/Yossarian\_1234 · Oct 18, 16:43

**Tags**: `#time-series`, `#synthetic-data`, `#linear-RNN`, `#forecasting`, `#machine-learning`

---

<a id="item-tech-news-8"></a>
### [Proof Before Reuse: showing agents only what later sessions reproduced keeps a poisoned skill out of procedural memory \[R\]](https://www.reddit.com/r/MachineLearning/comments/1x975ea/proof_before_reuse_showing_agents_only_what_later/) ⭐️ 7.0/10

A Reddit case study introduces &\#x27;proof before reuse&\#x27; to block poisoned code from entering an agent&\#x27;s procedural memory, showing promising results.

reddit · r/MachineLearning · /u/maa\_\_\_\_z · Oct 18, 16:14

**Tags**: `#AI safety`, `#code generation`, `#agent memory`, `#machine learning`

---

<a id="item-tech-news-9"></a>
### [Anthropic works with law firms to draft AI agent negotiation rules](https://www.ft.com/content/f7c26ac0-f5f2-443a-86b2-39d62f7920a9?syn-25a6b1a6=1) ⭐️ 7.0/10

Anthropic is consulting law firms and other legal bodies to create formal rules for AI agents that negotiate on users&\#x27; behalf, such as bargaining prices, handling disputes, or negotiating salaries. The company is researching a &quot;negotiation protocol&quot; and is considering requiring agents to carry user‑signed authorization documents. In September 2026, Anthropic staff used a Claude‑based agent in a virtual book‑trading marketplace, finding that a &quot;ruthless&quot; negotiation style gave a slight edge, and a Harvard study of over 180,000 agent negotiations identified new tactics that can weaken opponents.

telegram · zaihuapd · Oct 18, 07:07

**「Earlier Anthropic AI‑agent negotiation work」** Anthropic has previously run internal experiments where Claude‑based agents negotiated purchases inside its San Francisco office, and it recently partnered with the global law firm Freshfields, which has over 2,800 lawyers, to study the ethics and legal frameworks for AI‑mediated bargaining. These prior efforts provide the context for the current discussions with law firms on formal negotiation rules.

**「Impact」** Developers of AI negotiation agents will need to embed legal compliance mechanisms and possibly integrate user‑signed authorizations, which could add design complexity and affect how such agents are deployed in commercial or consumer settings.

<details><summary>References</summary>
<ul>
<li><a href="https://tech-insider.org/anthropic-freshfields-ai-agents-legal-deals-2026/">Anthropic Taps 2,800 Lawyers to Watch AI Agent Deals [2026]</a></li>
<li><a href="https://www.winzheng.com/en/article/anthropic-freshfields-claude-agents-negotiation-ethics-bound">Anthropic Teams With 2,800 Lawyers to Set AI Agent ...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#negotiation`, `#AI policy`, `#legal tech`

---

<a id="item-tech-news-10"></a>
### [Nvidia vLLM optimization speeds up Kimi K3 inference 1.68×](https://x.com/SemiAnalysis_/status/2111627094878790023) ⭐️ 7.0/10

Nvidia applied an upstream vLLM optimization to the 2.8‑trillion‑parameter Kimi K3 large language model, achieving 423 tokens per user per second on the same hardware—a 1.68× speed increase over the prior baseline. The work involved CentML engineer Benjamin writing a decode‑specific kernel with Cute DSL and merging it via a Megakernel fusion. Nvidia is also extending vLLM support to other models such as DeepSeek v4.1.

telegram · zaihuapd · Oct 18, 08:20

**「Background」** Kimi K3 is a 2.8‑trillion‑parameter multimodal Mixture‑of‑Experts model with a 1 million‑token context window and specialized attention mechanisms such as KDA, making it one of the largest open‑source LLMs currently available. vLLM is an open‑source high‑throughput inference engine that batches token generation and can be extended with custom kernels, so upstream vLLM optimizations can directly affect the per‑token throughput of large models like Kimi K3.

**「Impact」** Deployers of Kimi K3 can expect roughly 68% higher inference throughput per GPU, allowing more concurrent requests or reducing the number of GPUs needed for a given load, which can lower operational costs for large‑model services.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.ai/ai-models/kimi-k3">Kimi K3: 2.8T Open Model for Coding &amp; Knowledge Work</a></li>
<li><a href="https://arxiv.org/pdf/2607.24653">Kimi K3: Open Frontier Intelligence - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#inference optimization`, `#vLLM`, `#large language models`, `#Nvidia`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China adds medical exoskeleton rehab to regional insurance pilots](https://wap.eastmoney.com/a/202610173899077871.html) ⭐️ 8.0/10

China has included medical‑exoskeleton rehabilitation training in insurance or long‑term care pilot schemes in Beijing, Shanghai, Jiangsu and Zhejiang, and IDC estimates the 2025 Chinese market for such devices at roughly 14.2 billion yuan.

telegram · zaihuapd · Oct 18, 10:38

**「Policy context」** The National Healthcare Security Administration’s 15‑year “Universal Medical Security” plan calls for adding new technologies to insurance, and IDC estimated the Chinese medical‑rehab exoskeleton market at about 1.42 billion yuan in 2025.

**Tags**: `#Healthcare policy`, `#Medical devices`, `#Rehabilitation technology`, `#China`

---

<a id="item-finance-news-2"></a>
### [China food‑delivery platforms profit rebound, but merchants and riders face tighter margins](https://www.latepost.com/news/dj_detail?id=3762) ⭐️ 7.0/10

One year after the subsidy war, daily orders on Meituan and Alibaba’s platforms combined reached about 140 million in September 2026, roughly 50% higher than the pre‑war level of 90 million, and platform operating profit has recovered as sales‑expense ratios return to pre‑war levels.

telegram · zaihuapd · Oct 18, 07:40

**「Background」** The 2025 delivery‑subsidy war, sparked by JD.com’s launch of a food‑delivery service and prompting Meituan and Alibaba’s Ele.me to offer large subsidies, drove order volumes up dramatically and strained platform margins.

**「Impact」** The shift away from subsidies has squeezed merchants, whose store revenues and profits have fallen, and reduced average rider earnings in first‑ and second‑tier cities to 7–8.5 yuan per order, about a 50% drop in income.

<details><summary>References</summary>
<ul>
<li><a href="https://hellochinatech.com/p/meituan-delivery-war-limits-of-scale">Meituan and the Limits of Scale: China&#x27;s Delivery War Aftermath</a></li>

</ul>
</details>

**Tags**: `#Food Delivery`, `#Chinese Market`, `#Platform Economics`, `#Rider Income`, `#Merchant Impact`

---