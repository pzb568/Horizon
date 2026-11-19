---
layout: default
title: "Horizon Summary: 2026-11-19 (EN)"
date: 2026-11-19
lang: en
---

> From 44 items, 12 important content pieces were selected

---

**Technology News**
1. [Quad9 Withdraws from France Over DNS Blocking Law](#item-tech-news-1) ⭐️ 8.0/10
2. [Curl’s Rust rewrite adds 200+ bug fixes and security patches](#item-tech-news-2) ⭐️ 8.0/10
3. [Xint discloses five NGINX vulnerabilities enabling root compromise](#item-tech-news-3) ⭐️ 8.0/10
4. [Google DeepMind releases Genie 4 for AI Ultra subscribers](#item-tech-news-4) ⭐️ 7.0/10
5. [RadixArk releases open‑source DaisyRose‑27B 27B‑parameter LLM](#item-tech-news-5) ⭐️ 7.0/10
6. [OpenAI models applied to chip design automation](#item-tech-news-6) ⭐️ 7.0/10
7. [Anthropic launches Claude API linked‑billing beta](#item-tech-news-7) ⭐️ 7.0/10
8. [DeepSeek makes server‑side search and web crawling free, charges only token usage](#item-tech-news-8) ⭐️ 7.0/10
9. [CoolTech 10 Ultra charger OTA firmware fix for 20V over‑voltage bug](#item-tech-news-9) ⭐️ 7.0/10
10. [US Government Considers Requiring Firms to Disclose Use of Chinese AI Models](#item-tech-news-10) ⭐️ 7.0/10

**Financial News**
1. [Fed Governor Waller says half‑point rate hike may be needed](#item-finance-news-1) ⭐️ 8.0/10
2. [Tencent Q3 2026 earnings show revenue rise and record AI spending](#item-finance-news-2) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Quad9 Withdraws from France Over DNS Blocking Law](https://techstackups.com/articles/quad9-leaves-france-dns-blocking/) ⭐️ 8.0/10

Quad9 announced it is exiting the French market after a court order required DNS resolvers to block access to piracy sites, a requirement Quad9 says conflicts with its privacy‑focused service model. The withdrawal means French users will no longer receive Quad9’s DNS resolution, which includes security filtering and no‑logging guarantees.

hackernews · ritzaco · Nov 18, 13:18 · [Discussion](https://news.ycombinator.com/item?id=50545958)

**「Background」** Quad9 is a non‑profit public DNS resolver that provides recursive DNS lookups for users worldwide. In some jurisdictions, governments have tried to curb online piracy by requiring DNS resolvers to block access to specific domains, a practice that relies on the resolver’s role as the first step in translating human‑readable names to IP addresses. Quad9’s earlier encounter with a similar mandate in Germany—where a court fined it for using geo‑IP blocking in the Sony Music v. Quad9 case—illustrates the legal pressure on DNS services to enforce content‑blocking orders, setting the stage for its recent withdrawal from France rather than comply with a beIN Sports blocking order.

**「Impact」** French internet users who relied on Quad9 must switch to another DNS provider to retain the same level of security and privacy, and the move highlights that DNS resolvers cannot be reliably used as a tool for enforcing anti‑piracy legislation.

**「Community Discussion」** One commenter noted that attempts to fight piracy through DNS blocking often serve as a backdoor for suppressing speech the government dislikes, questioning the broader motive of such regulations.

<details><summary>References</summary>
<ul>
<li><a href="https://techstackups.com/articles/quad9-leaves-france-dns-blocking/">Quad 9 Is Leaving France : Why DNS Resolvers Are... | Tech Stackups</a></li>
<li><a href="https://news.ycombinator.com/item?id=50538994">Quad 9 &#x27;s withdrawal from France : A canary in the coal... | Hacker News</a></li>

</ul>
</details>

**Tags**: `#DNS`, `#Internet Policy`, `#Security`

---

<a id="item-tech-news-2"></a>
### [Curl’s Rust rewrite adds 200+ bug fixes and security patches](https://simonwillison.net/2026/Nov/18/daniel-stenberg/) ⭐️ 8.0/10

During a three‑week effort, the effort to rewrite curl’s codebase from C to Rust converted roughly 185,000 lines of C into 340,000 lines of Rust and merged over 300 commits. In that time the upstream curl project received a little over 200 bug‑fixes and several vulnerability patches, with a similar amount expected in the following month. The numbers reflect actual changes to the official curl repository, not just the generated Rust clones.

rss · Simon Willison · Nov 18, 15:58

**「Context: curl and AI‑generated Rust rewrites」** curl is a ubiquitous C‑based library and command‑line tool for transferring data with URLs, and its codebase has long been maintained by its creator Daniel Stenberg. In late 2026, AI coding agents produced Rust rewrites that translated roughly 185,000 lines of curl’s C code into 340,000 lines of Rust, prompting Stenberg to compare those clones with the upstream project’s ongoing maintenance. The upstream project continued to merge over 300 commits, including more than 200 bug‑fixes and several security patches, highlighting the gap between automated rewrites and the active development of the original code.

**「Impact」** Developers who rely on curl now have a version that incorporates a large batch of bug fixes and security updates, reducing the risk of crashes or exploits in applications that embed the library. However, the Rust rewrite is still in progress, so users should continue to track its compatibility and migration status before adopting the Rust‑based build as a drop‑in replacement.

<details><summary>References</summary>
<ul>
<li><a href="https://explainx.ai/blog/daniel-stenberg-curl-rust-agent-rewrites-vs-maintenance-november-2026">curl vs Rust Rewrites: 200 Fixes Agents Missed | explainx.ai Blog</a></li>

</ul>
</details>

**Tags**: `#curl`, `#rust`, `#security`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [Xint discloses five NGINX vulnerabilities enabling root compromise](https://nginx2root.com/) ⭐️ 8.0/10

Xint announced five new NGINX vulnerabilities, including CVE‑2026‑123007 \(an unauthenticated HTTP/2 flow‑control memory corruption that lets an attacker execute commands in the worker process\). Combined with a Linux kernel defect, the chain can give a remote attacker root access to the host. The flaws were patched in NGINX 1.30.7 and 1.31.9 released on 18 Nov 2026, and Rapid7 has published proof‑of‑concept code, though no wild exploits have been observed. Users unable to upgrade should disable external HTTP/2 as a mitigation.

telegram · zaihuapd · Nov 18, 16:21

**「Prerequisite concepts」** NGINX is a widely deployed web server and reverse proxy that supports HTTP/2. The newly disclosed CVE‑2026‑123007 exploits an integer underflow in HTTP/2 flow‑control accounting, causing memory corruption in the worker process and allowing unauthenticated remote code execution, as described by Ubuntu, Rapid7 and Wiz analyses. Similar remote‑code‑execution flaws have been patched in recent NGINX releases \(1.30.7 and 1.31.9\) which addressed ten CVEs on 18 Nov 2026.

**「Impact」** Administrators should upgrade to NGINX 1.30.7 or 1.31.9 immediately, or disable external HTTP/2 if upgrading is not possible, to prevent remote root compromise.

<details><summary>References</summary>
<ul>
<li><a href="https://ubuntu.com/security/CVE-2026-123007">CVE - 2026 - 123007 | Ubuntu</a></li>
<li><a href="https://www.rapid7.com/blog/post/ve-cve-2026-123007-critical-nginx-http-2-integer-underflow-leads-to-rce-fixed/">Rapid7 discloses a critical vulnerability affecting NGINX HTTP / 2 that...</a></li>
<li><a href="https://www.wiz.io/blog/nginx-http2-rce-vulnerabilities">Unauthenticated Remote Code Execution in NGINX ... | Wiz Blog</a></li>

</ul>
</details>

**Tags**: `#security`, `#nginx`, `#vulnerability`, `#linux`, `#devops`

---

<a id="item-tech-news-4"></a>
### [Google DeepMind releases Genie 4 for AI Ultra subscribers](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/genie-4-now-available-project-genie/) ⭐️ 7.0/10

Google DeepMind announced that its latest large language model, Genie 4, is now available, but only to &quot;Eligible Google AI Ultra&quot; subscribers. The release follows Genie 3 and adds a new version to the Genie series, though the announcement provides no technical specifications, performance metrics, or broader availability details.

hackernews · leumon · Nov 18, 18:49 · [Discussion](https://news.ycombinator.com/item?id=50550415)

**「Prerequisite concepts」** Genie is Google DeepMind’s interactive world‑model series that lets users create photorealistic environments from text or image prompts and manipulate them in real time. Access to the latest version, Genie 4, is provided through Project Genie and is limited to subscribers of Google’s AI Ultra tier, a paid offering that grants early access to advanced models.

**「Impact」** Developers who are part of the Google AI Ultra program can begin experimenting with Genie 4 immediately, while others must wait for a wider rollout or additional access options.

**「Community Discussion」** A Hacker News commenter noted that the announcement lacks clarity on pricing and eligibility, stating that their workspace account cannot access Genie 4 and questioning whether regional restrictions or subscription status are the cause.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/genie/">Genie 4 — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/genie-4-now-available-project-genie/">Project Genie update featuring Genie 4</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Large Language Models`, `#Google DeepMind`, `#Model Release`

---

<a id="item-tech-news-5"></a>
### [RadixArk releases open‑source DaisyRose‑27B 27B‑parameter LLM](https://www.radixark.com/blog/daisyrose-27b) ⭐️ 7.0/10

RadixArk announced the open‑source release of DaisyRose‑27B, a 27‑billion‑parameter language model trained on 144 Nvidia H200 GPUs. The model and its weights are now hosted on Hugging Face, allowing AI practitioners to download and run the model without a commercial license. Training required a substantial compute budget, but the release provides a large‑scale reference model for research and fine‑tuning.

hackernews · de\_sty · Nov 18, 19:39 · [Discussion](https://news.ycombinator.com/item?id=50551046)

**「Prerequisite concepts for DaisyRose-27B」** DaisyRose-27B is built on the Qwen‑3.8‑27B model, an open‑source 27‑billion‑parameter transformer that serves as a common base for many recent LLM releases. The new model was further refined with reinforcement‑learning training \(using RadixArk’s Miles framework\) on 1,200 curated long‑horizon tasks, a process similar to RL‑from‑human‑feedback that aims to improve task‑specific behavior. Training such a large model required substantial compute – 144 Nvidia H200 GPUs running for 18 days – illustrating the hardware scale typically needed for post‑training efficiency work.

**「Impact」** Developers can experiment with a state‑of‑the‑art 27B‑parameter model without licensing fees, though reproducing the original training would demand a comparable H200 GPU cluster, limiting full‑scale replication to well‑funded labs.

**「Community Discussion」** Commenters noted the absence of a GGUF‑format download, expressing a desire for more benchmark transparency and details on the training topology, which could aid reproducibility and comparative evaluation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.radixark.com/blog/daisyrose-27b">DaisyRose-27B: Pushing the Frontier of Post-Training Efficiency</a></li>
<li><a href="https://www.radixark.com/blog">Blog · RadixArk</a></li>

</ul>
</details>

**Tags**: `#large-language-models`, `#open-source`, `#hardware`, `#model-training`, `#AI-research`

---

<a id="item-tech-news-6"></a>
### [OpenAI models applied to chip design automation](https://openai.com/index/advancing-chip-design-with-our-models/) ⭐️ 7.0/10

OpenAI announced that its existing language models are being applied to automate and improve chip design workflows, enabling AI‑generated RTL, analog components, and automated EDA flow orchestration for hardware engineers. The announcement describes the models as tools that can write code to generate circuits, run multi‑hour simulations, and assist designers, but does not specify a new product release or version.

hackernews · vighneshiyer · Nov 18, 17:45 · [Discussion](https://news.ycombinator.com/item?id=50549493)

**「Prerequisite concepts」** Chip design depends on electronic design automation \(EDA\) tools that turn RTL and analog specifications into silicon, and recent AI‑assisted workflows have begun using large language models to generate RTL, optimise floorplans, and suggest micro‑architectural tweaks. OpenAI’s earlier GPT‑4‑based models were already used to help draft RISC‑V cores and initial layout work, paving the way for the newer GPT‑6 Astra models that now claim to optimise circuits for the Jalapeño silicon chip.

**「Impact」** Hardware designers can use the AI agents to offload routine circuit generation and simulation tasks, potentially shortening design cycles and reducing manual effort in EDA flows, as reported by early adopters who see the agent handling multi‑hour simulations automatically.

**「Community Discussion」** One commenter \(skyberrys\) reported practical success treating chip design as a software problem, using the AI agent to generate circuits and automate the EDA flow, though they note that only a small fraction of the design is in RTL and most is analog.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/advancing-chip-design-with-our-models/">Advancing chip design with OpenAI models | OpenAI</a></li>
<li><a href="https://openai.com/index/jalapeno-first-results/">Jalapeño’s first results show industry-leading speed and... | OpenAI</a></li>

</ul>
</details>

**Tags**: `#chip design`, `#AI for hardware`, `#OpenAI`, `#EDA`, `#RISC-V`

---

<a id="item-tech-news-7"></a>
### [Anthropic launches Claude API linked‑billing beta](https://thenextweb.com/news/anthropic-linked-billing-claude-api-customers-pay) ⭐️ 7.0/10

Anthropic has released a beta for linked billing on its Claude API, allowing organizations that pay Anthropic directly to have API usage charged to their own Anthropic organization account. Customers can set monthly spend caps or disconnect the link at any time, and any request that fails billing is rejected rather than falling back to the developer’s payment method. The feature is limited to direct‑pay Anthropic organizations and does not apply to usage billed through AWS, Google Cloud, Azure, or subscription‑only accounts; it also does not provide zero‑data‑retention or HIPAA protections for these calls.

telegram · zaihuapd · Nov 18, 07:24

**「Prerequisite: Claude API billing model」** Claude API is Anthropic’s hosted large‑language‑model service accessed via API keys, with usage traditionally billed to the Anthropic account that created the key. Previously, organizations could not directly allocate API costs to their own Anthropic organization, so developers bore the charges. The linked‑billing beta extends Anthropic’s existing organization‑based account structure to let customers bill usage to their own organization account.

**「Impact」** Developers using Claude API must configure a linked‑billing organization and set appropriate spend limits, otherwise API calls may be denied if billing fails, which could interrupt services that rely on the model.

**Tags**: `#AI`, `#APIs`, `#Billing`, `#Anthropic`, `#Claude`

---

<a id="item-tech-news-8"></a>
### [DeepSeek makes server‑side search and web crawling free, charges only token usage](https://www.ithome.com/1/029/058.htm) ⭐️ 7.0/10

Effective 12:00 Beijing time on 18 Nov 2026, DeepSeek stopped charging separate fees for its server‑side search and web‑crawling services. Calls to the model that invoke these functions – including the network tool, Anthropic API’s web\_search tool, and the Responses API web\_search tool – are now billed solely on model token consumption. Previously, the Search and Fetch APIs were priced at 5 CNY per 1,000 successful requests. The change means developers only pay for token usage, not per‑request search fees.

telegram · zaihuapd · Nov 18, 13:44

**「Background」** DeepSeek’s Search and Fetch APIs let developers add server‑side web search and page‑fetching to model calls, and they have been billed separately from model token usage. Until now the APIs were priced at 5 yuan per 1,000 successful requests, while model usage itself is charged per token \(per‑million‑token rates\). This prior per‑request fee is what is being removed in the new policy.

**「Impact」** Developers integrating DeepSeek’s APIs will see lower operational costs for search‑related features, needing only to monitor token usage for budgeting, which may encourage broader adoption of the search and fetch capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/quick_start/pricing/?tool=deepseek">Models &amp; Pricing | DeepSeek API Docs</a></li>
<li><a href="https://www.ababnews.com/en/news/9b98272c-3464-4949-8cac-ae558f22d5be">DeepSeek API Charges 5 Yuan per 1000 Web Searches - ABAB News</a></li>

</ul>
</details>

**Tags**: `#AI`, `#APIs`, `#Cost Management`, `#Machine Learning`

---

<a id="item-tech-news-9"></a>
### [CoolTech 10 Ultra charger OTA firmware fix for 20V over‑voltage bug](https://www.bilibili.com/opus/1272074321303437312) ⭐️ 7.0/10

The CoolTech 10 Ultra charger \(model AD1204U\) was found to have an MCU firmware bug that, in rare cases, caused the protocol chip to stop responding and output up to 20 V instead of the intended low voltage, risking damage to peripherals such as earphones and keyboards. CoolTech identified and corrected the fault, releasing an OTA firmware update on Monday via the Mi Home app’s Bluetooth upgrade path. The first reported damage incident occurred in June 2026, while devices rated for 20 V \(e.g., phones, laptops\) were not affected.

telegram · zaihuapd · Nov 19, 01:30

**「Technical context of charger firmware bugs」** USB‑C Power Delivery chargers rely on a protocol controller \(often called a protocol chip\) that negotiates the voltage with the attached device. If the controller’s firmware fails to respond, the charger may default to its maximum output \(e.g., 20 V\), which can damage low‑voltage peripherals such as headphones, keyboards, or mice. Modern chargers can receive over‑the‑air \(OTA\) firmware updates, typically delivered through a companion app \(e.g., the Mi Home app\) to fix such issues without replacing the hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://onebn.club/en/article/cuktech-issues-firmware-fix-for-10-ultra-charger-over-voltage-bug">CUKTECH Issues Firmware Fix for 10 Ultra Charger Over Voltage Bug</a></li>
<li><a href="https://www.163.com/dy/article/LC3HUBNO0511B8LM.html">酷态科10 Ultra确认存在低压设备损坏隐患，已OTA推送修复固件|充电头|...</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#firmware`, `#embedded`, `#consumer-electronics`

---

<a id="item-tech-news-10"></a>
### [US Government Considers Requiring Firms to Disclose Use of Chinese AI Models](https://www.reuters.com/world/china/trump-administration-weighs-forcing-us-firms-disclose-chinese-ai-use-2026-11-18/) ⭐️ 7.0/10

U.S. officials are weighing a proposal that would require American companies to publicly disclose any use of Chinese artificial‑intelligence models. The Treasury Department and the White House Office of Science and Technology Policy have discussed the idea, and an example cited is Airbnb’s use of Alibaba’s Qwen model for customer‑service functions, which would have to be listed on the company’s website if the rule were adopted. The measure is intended to curb reliance on inexpensive Chinese open‑weight models by “public naming,” not to impose new usage bans, and it remains a policy consideration without confirmed legislative backing.

telegram · zaihuapd · Nov 19, 02:30

**「Context of Chinese AI model usage in the US」** U.S. firms have already begun integrating Chinese AI models into their products; for example, Airbnb has deployed Alibaba’s Qwen model to power parts of its customer‑service AI system. This existing reliance on Chinese‑origin models provides the backdrop for the U.S. government’s consideration of a disclosure requirement.

**「Impact」** If enacted, firms would need to add a compliance process to identify and publicly list Chinese AI models in their products or services, potentially limiting the adoption of cost‑effective Chinese offerings and increasing legal and reporting overhead for affected businesses.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aiusecasehub.com/case/dd44cd65306c24b4d91675442fb4620546c35251dc440569ee9e8fac452c46c2/airbnb-uses-alibaba-qwen-for-customer-service-ai-workloads">Airbnb uses Alibaba Qwen for customer-service AI workloads</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#US-China tech relations`, `#Corporate compliance`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed Governor Waller says half‑point rate hike may be needed](https://www.cnbc.com/2026/11/18/federal-reserve-governor-christopher-waller.html) ⭐️ 8.0/10

Fed Governor Christopher Waller told CNBC a half‑percentage‑point increase in the benchmark rate is probably necessary at the Dec. 8‑9 FOMC meeting to combat rising inflation.

rss · CNBC Finance · Nov 18, 15:13

**「Background」** The Fed had previously cut rates by three‑quarter points in 2025 and has held rates steady since a September hike, while inflation remains above the 2% target.

**Tags**: `#Federal Reserve`, `#Monetary Policy`, `#Inflation`, `#Interest Rates`

---

<a id="item-finance-news-2"></a>
### [Tencent Q3 2026 earnings show revenue rise and record AI spending](https://api3.cls.cn/share/article/2537922?os=android&amp;amp;sv=8.8.5&amp;amp;app=cailianpress&amp;amp;selected=) ⭐️ 8.0/10

Tencent posted Q3 2026 revenue of 2073 亿元, up 8% YoY, but capital expenditure surged to 814.33 亿元, well above the 554 亿元 market estimate, and free cash flow was a negative 691 亿元; its WorkBuddy AI service used more than 100 trillion tokens per day, the highest in China.

telegram · zaihuapd · Nov 18, 09:20

**「Background」** WorkBuddy is Tencent&\#x27;s AI agent for office tasks that, before the Q3 report, already had over 10 million daily active users and was noted for the highest daily token consumption among Chinese large‑language‑model products.

<details><summary>References</summary>
<ul>
<li><a href="https://www.workbuddy.ai/">WorkBuddy - AI Agent for Everyday Office Work</a></li>
<li><a href="https://finance.sina.com.cn/tech/digi/2026-11-18/doc-inizeacc1577026.shtml">腾讯 WorkBuddy 日活跃用户数超 1000 万，成为中国大语言模型日均 Tok...</a></li>

</ul>
</details>

**Tags**: `#Tencent`, `#Earnings`, `#AI Spending`, `#Capital Expenditure`, `#Chinese Tech`

---