---
layout: default
title: "Horizon Summary: 2026-11-18 (EN)"
date: 2026-11-18
lang: en
---

> From 43 items, 12 important content pieces were selected

---

**Technology News**
1. [Java4Shell RCE vulnerability in OpenJDK Base64 processing](#item-tech-news-1) ⭐️ 8.0/10
2. [ONNX Runtime repository removed from GitHub, breaking pipelines](#item-tech-news-2) ⭐️ 8.0/10
3. [SolidJS 2.0 adds server‑side RPC, live and broadcast features](#item-tech-news-3) ⭐️ 8.0/10
4. [Nvidia stops reporting Singapore subsidiary revenue as $104 B figure disclosed](#item-tech-news-4) ⭐️ 8.0/10
5. [Prime Radiant releases external sandbox servers for AI coding agents](#item-tech-news-5) ⭐️ 8.0/10
6. [US hyperscale data centers consume about 2% of national electricity](#item-tech-news-6) ⭐️ 8.0/10
7. [Hacker News thread compares AI model harness performance](#item-tech-news-7) ⭐️ 7.0/10
8. [Anthropic approved for Nasdaq listing under ticker ANT](#item-tech-news-8) ⭐️ 7.0/10
9. [Telegram Requires Bots and Mini‑Apps to Use Stars for Digital Sales](#item-tech-news-9) ⭐️ 7.0/10
10. [可灵 AI launches Kling Image 4.0 with native 8K generation](#item-tech-news-10) ⭐️ 7.0/10

**Financial News**
1. [Former Nvidia CEO says he would return if board asks](#item-finance-news-1) ⭐️ 8.0/10
2. [MIIT tasks auto association to assess 60‑day payment rule for 17 car makers](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Java4Shell RCE vulnerability in OpenJDK Base64 processing](https://calif.io/java4shell/) ⭐️ 8.0/10

The Java4Shell exploit \(CVE‑2026‑114938, CVSS 9.2\) enables unauthenticated remote code execution by abusing OpenJDK’s Base64 decoder on x86‑64 CPUs that support the AVX‑512 VBMI instruction set. It affects Java 17 \(17.0.6 and later\), Java 21, Java 25, and Java 27 builds, while standard Java 8/11 are generally safe except for the Oracle Java 8 Performance Pack. Only servers with Intel Ice Lake‑era \(or newer\) Xeon and AMD Zen 4‑era \(or newer\) EPYC/Ryzen CPUs are vulnerable; ARM64 systems are not impacted.

hackernews · werrett · Nov 17, 21:11 · [Discussion](https://news.ycombinator.com/item?id=50538240)

**「OpenJDK Base64 decoder and hardware acceleration」** OpenJDK’s Base64 implementation was optimized to use the AVX‑512 VBMI instruction set on recent x86‑64 CPUs, a change introduced in the Java 17 line \(17.0.6 and later\) and carried forward to newer releases such as Java 21, 25 and 27. This hardware‑accelerated path had not previously been associated with security bugs, but the new CVE‑2026‑114938 \(Java4Shell\) shows that a memory‑corruption flaw in that decoder can be exploited for unauthenticated remote code execution. The vulnerability only affects builds running on processors that support AVX‑512 VBMI \(Intel Ice Lake and newer, AMD Zen 4 and newer\), while ARM64 and older Java 8/11 builds are generally unaffected.

**「Impact」** Systems running the affected Java versions on recent Intel or AMD servers can be remotely compromised unless mitigated, prompting administrators to apply vendor patches, disable AVX‑512 via the -XX:UseAVX=2 flag, or upgrade to non‑vulnerable JVM builds.

**「Community discussion」** Commenters noted that Semgrep has released detection scripts for the five key conditions of the exploit, and some suggest a temporary workaround by disabling AVX‑512 with the -XX:UseAVX=2 JVM flag.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/java-17-rce-vulnerability-cve-2026-114938">Java4Shell Java 17 RCE ( CVE - 2026 - 114938 ): Fix &amp; Versions</a></li>
<li><a href="https://orca.security/resources/research/java4shell-critical-openjdk-base64-decoder-flaw-could-allow-unauthenticated-remote-code-execution/">Java4Shell CVE - 2026 - 114938 : Affected Versions &amp; Mitigation</a></li>

</ul>
</details>

**Tags**: `#Java`, `#Security`, `#OpenJDK`, `#RCE`, `#Vulnerability`

---

<a id="item-tech-news-2"></a>
### [ONNX Runtime repository removed from GitHub, breaking pipelines](https://github.com/microsoft/onnxruntime) ⭐️ 8.0/10

On November 17, 2026 the Microsoft ONNX Runtime repository \(https://github.com/microsoft/onnxruntime\) was removed from GitHub without prior notice, causing machine‑learning pipelines that depend on the package to fail and prompting security concerns among users. The deletion affects the widely used runtime, which had about 22 000 stars, and there is no official explanation from Microsoft at the time of reporting.

hackernews · nvader · Nov 17, 23:18 · [Discussion](https://news.ycombinator.com/item?id=50539610)

**「What is ONNX Runtime?」** ONNX Runtime is Microsoft’s open‑source, cross‑platform inference engine that accelerates execution of ONNX‑format machine‑learning models and is widely used in production pipelines. The project is hosted on GitHub, where its source code, documentation and telemetry settings \(e.g., optional trace‑event collection\) are publicly available. Understanding its role clarifies why the sudden removal of the repository impacts many downstream systems.

**「Impact」** Engineers using ONNX Runtime experienced immediate evaluation failures and must either locate an alternative source, such as the Intel‑maintained fork \(github.com/intel/onnxruntime\), or build the runtime from source to restore functionality.

**「Community discussion」** Commenters noted the lack of advance warning \(nvader\) and suggested the Intel fork as a practical workaround \(Heliodex\).

<details><summary>References</summary>
<ul>
<li><a href="https://onnxruntime.ai/docs/">ONNX Runtime is a cross-platform machine-learning model accelerator</a></li>
<li><a href="https://github.com/microsoft/onnxruntime/blob/main/docs/Privacy.md">onnxruntime/docs/Privacy.md at main · microsoft/onnxruntime</a></li>

</ul>
</details>

**Tags**: `#ONNX`, `#MachineLearning`, `#Infrastructure`, `#Security`, `#GitHub`

---

<a id="item-tech-news-3"></a>
### [SolidJS 2.0 adds server‑side RPC, live and broadcast features](https://www.solidjs.com/blog/solid-2-0-the-long-hold/) ⭐️ 8.0/10

Solid 2.0 is a major version release of the SolidJS framework that adds built‑in server‑side RPC, live data streaming, and broadcast capabilities. These features let front‑end developers write reactive UI code that can directly invoke server functions and push updates without extra libraries. The update is positioned as a high‑value enhancement for Solid users, though it does not represent a broader industry paradigm shift.

hackernews · pier25 · Nov 17, 18:56 · [Discussion](https://news.ycombinator.com/item?id=50536387)

**「Prerequisite concepts」** SolidJS is a JavaScript UI library that uses fine‑grained, compile‑time reactivity to update the DOM efficiently. The framework’s initial stable releases \(1.x\) focused on client‑side rendering and did not include built‑in mechanisms for server‑side remote‑procedure calls, live data synchronization, or broadcast messaging. Understanding this prior architecture clarifies why the new Solid 2.0 features—server‑side RPC, live, and broadcast—represent a notable extension of the library’s capabilities.

**「Impact」** Developers can now implement server‑driven interactions and real‑time UI updates using only SolidJS, reducing the need for separate state‑sync or RPC libraries and simplifying the client‑server architecture of web apps.

**「Community Discussion」** A commenter noted that Solid’s server RPC, live, and broadcast features feel more natural to use than alternatives like LiveView or htmx/datastar, praising the seamless integration.

**Tags**: `#frontend`, `#javascript`, `#web frameworks`, `#solidjs`

---

<a id="item-tech-news-4"></a>
### [Nvidia stops reporting Singapore subsidiary revenue as $104 B figure disclosed](https://www.ft.com/content/dbde7a30-548c-4f9d-a4be-7898a0c24dcf) ⭐️ 8.0/10

Nvidia has ceased publishing sales figures for its Singapore subsidiary, Megaspeed, after the subsidiary reported $104 billion in external revenue for 2025. The move follows U.S. investigations into whether Megaspeed was used to route Nvidia GPU chips to China in violation of export sanctions. The company’s decision removes a previously disclosed revenue line, making the scale of Singapore‑based sales opaque to investors and regulators.

hackernews · louiereederson · Nov 17, 17:12 · [Discussion](https://news.ycombinator.com/item?id=50534631)

**「Why Nvidia’s Singapore sales matter」** Nvidia’s Singapore operations are run through the subsidiary Megaspeed, which aggregates orders that are routed through Singapore before reaching OEMs and ODMs worldwide. US authorities have been investigating whether Megaspeed was used to divert Nvidia’s advanced chips to China in violation of export controls, prompting heightened scrutiny of the subsidiary’s revenue reporting. The company’s decision to stop disclosing Singapore‑specific sales follows earlier investor reports that had highlighted the subsidiary’s $104 billion external revenue in 2025.

**「Impact」** Investors and compliance teams now face greater uncertainty about Nvidia’s exposure to sanction‑related supply‑chain risks, prompting heightened due‑diligence and possible reassessment of the company’s regulatory risk profile.

**「Community discussion」** Commenters noted that the $104 billion figure reflects revenue booked through the Singapore entity rather than chips physically sold there, and that most end‑users acquire Nvidia GPUs via OEMs and cloud providers, not directly, questioning the relevance of the alleged smuggling to Chinese developers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ft.com/content/dbde7a30-548c-4f9d-a4be-7898a0c24dcf?syn-25a6b1a6=1">Nvidia stopped disclosing Singapore sales as revenues hit $104bn</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/nvidia-abruptly-changed-reported-revenue-004426232.html?fr=sycsrp_catchall">Nvidia abruptly changed how it reported revenue in Singapore ...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#Semiconductors`, `#AI hardware`, `#Sanctions`

---

<a id="item-tech-news-5"></a>
### [Prime Radiant releases external sandbox servers for AI coding agents](https://simonwillison.net/2026/Nov/17/external-sandboxes-for-coding-agents/) ⭐️ 8.0/10

Prime Radiant has published three open‑source sandbox server implementations that let coding agents run generated code in an isolated environment while the agent itself remains outside the sandbox. The servers—external‑sandbox‑v86 \(Node.js + v86 WebAssembly Linux\), external‑sandbox‑container \(Python + Apple Containers\), and external‑sandbox‑quicksand \(Python + Microsoft Quicksand/QEMU\)—all expose the same localhost API and include an optional HTTP/HTTPS allow‑list proxy with credential substitution. This pattern enables tools such as Pi, Claude Code, or Codex to safely execute code without risking host compromise or prompt‑injection attacks.

rss · Simon Willison · Nov 17, 22:52

**「Sandboxing code for AI agents」** Running code generated by AI agents poses security risks such as accidental destructive actions or prompt‑injection attacks, so the code must be isolated from the host system. An external sandbox pattern separates the agent process from the execution environment: the agent runs outside while a dedicated sandbox server runs the generated code and returns results via a localhost API. This approach builds on traditional sandboxing techniques \(e.g., container‑based or WebAssembly‑based isolation\) but adapts them for on‑demand code execution by language models.

**「Impact」** Developers can point AI coding agents to the sandbox’s localhost endpoint, gaining deterministic isolation and network‑policy control, which reduces the attack surface when experimenting with local LLMs or untrusted code. Integration requires configuring the agent’s execution calls to the sandbox API and optionally setting proxy allow‑lists.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/prime-radiant-inc/external-sandbox-container">GitHub - prime - radiant -inc/ external - sandbox -container: Python...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#sandboxing`, `#coding agents`, `#devtools`

---

<a id="item-tech-news-6"></a>
### [US hyperscale data centers consume about 2% of national electricity](https://arstechnica.com/science/2026/11/hyperscale-data-centers-use-2-of-us-electricity/) ⭐️ 8.0/10

A study of 403 U.S. hyperscale data centers operating between May 2024 and April 2025 estimates they used 68–99 terawatt‑hours of electricity, representing roughly 1.5%–2.2% of total U.S. consumption—about the same as the entire electricity demand of Wisconsin or Indiana. The facilities were identified from a commercial database of 675 candidates and each averages about 40 MW of power capacity. The analysis could not separate AI‑focused workloads from traditional services, but it provides a baseline for future tracking of large‑scale compute energy use.

telegram · zaihuapd · Nov 17, 12:54

**「Background」** Hyperscale data centers are large‑scale facilities—typically 40 MW or more in capacity—operated by cloud providers and other major compute services. Prior reporting has highlighted their growing share of electricity use, but precise national‑level estimates have been limited. The new study, which examined 403 U.S. hyperscale sites between May 2024 and April 2025, provides the first quantified range \(68–99 TWh, about 1.5%–2.2% of U.S. electricity\) for this class of facilities.

**「Impact」** The finding underscores the sizable energy footprint of hyperscale compute infrastructure, prompting data‑center operators and policymakers to prioritize efficiency upgrades and consider regulatory or sustainability initiatives aimed at curbing electricity demand.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/science/2026/11/hyperscale-data-centers-use-2-of-us-electricity/">Hyperscale data centers use 2% of US electricity - Ars Technica</a></li>

</ul>
</details>

**Tags**: `#data centers`, `#energy consumption`, `#computer systems`

---

<a id="item-tech-news-7"></a>
### [Hacker News thread compares AI model harness performance](https://runta.com/blog/introducing-frontierharness-eval-v1-1/) ⭐️ 7.0/10

A Hacker News discussion examined how different prompt harnesses \(agent configurations\) affect the performance of various LLMs on terminal‑bench style tasks, reporting that about 64% of the compute spend was on runs that failed the benchmark verifiers and that the optimal harness varies by model and problem domain. The thread does not announce a new product or formal study, but shares observed variance across harnesses.

hackernews · Edward40 · Nov 17, 14:53 · [Discussion](https://news.ycombinator.com/item?id=50532191)

**「Prerequisite: harnesses and prior evaluation」** In AI agent research a &quot;harness&quot; refers to the prompt‑engineering wrapper that defines system prompts, tool names, context formatting and other conventions used to turn a language model into a coding agent. RUNTA’s earlier FrontierHarness Eval \(v1.0\) benchmarked a single model across several harnesses, establishing a baseline for how these wrappers affect performance. The new v1.1 expands the study to a full harness × model matrix with more harnesses and models, enabling a compatibility matrix that shows which harness works best with which model.

**「Impact」** Developers building AI agents should benchmark multiple harness designs for each target model and task, rather than assuming a single prompt setup will work best, and may need to adjust system prompts, tool naming, and context handling to reduce failure rates.

**「Community Discussion」** Commenters noted that harness differences stem mainly from context‑engineering choices and that standardizing system prompts could shrink performance variance \(krawczstef\), while others argued the best harness is problem‑specific and may become more important than model size as capabilities grow \(xyzzy\_plugh\).

<details><summary>References</summary>
<ul>
<li><a href="https://runta.com/blog/introducing-frontierharness-eval-v1-1/">Introducing FrontierHarness Eval v1.1 — RUNTA</a></li>
<li><a href="https://runta.com/blog/introducing-frontierharness-eval/">Introducing FrontierHarness Eval — RUNTA</a></li>

</ul>
</details>

**Tags**: `#prompt engineering`, `#AI agents`, `#benchmarking`, `#software engineering`

---

<a id="item-tech-news-8"></a>
### [Anthropic approved for Nasdaq listing under ticker ANT](https://mp.weixin.qq.com/s/IkZCf2pJaAAXPJEpXnEBHQ) ⭐️ 7.0/10

Anthropic announced that it has received approval to list its Class A common stock on the Nasdaq Global Select Market under the ticker symbol “ANT”. The approval enables the company to proceed with a public offering on Nasdaq.

telegram · zaihuapd · Nov 17, 13:00

**「Prerequisite filing for Nasdaq listing」** Anthropic’s Nasdaq approval follows its earlier filing of a Form S‑1 registration statement with the U.S. Securities and Exchange Commission, a required step for any company seeking to list its shares on a U.S. exchange such as the Nasdaq Global Select Market.

**「Impact」** Investors will be able to buy and sell Anthropic shares on Nasdaq once the listing is completed, giving the company access to public capital markets.

<details><summary>References</summary>
<ul>
<li><a href="https://ctrlmag.com/blog/anthropic-files-s-1-nasdaq-ticker-ant">Anthropic Files S-1 for Nasdaq Listing Under Ticker ANT</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Business`, `#StockMarket`, `#Anthropic`

---

<a id="item-tech-news-9"></a>
### [Telegram Requires Bots and Mini‑Apps to Use Stars for Digital Sales](https://telegram.me/zaihuapd/45189) ⭐️ 7.0/10

Telegram announced that, effective this week, all digital goods sold inside bots and mini‑apps must be purchased exclusively with Telegram Stars. The rule covers bot subscriptions, paid tools, access to third‑party AI models, and in‑app points or tokens; cryptocurrency transactions are limited to using GRAM. Telegram will begin active enforcement and any developer found violating the policy will be banned without further warning.

telegram · zaihuapd · Nov 17, 14:46

**「Telegram Stars payment requirement」** Telegram Stars is Telegram’s proprietary virtual currency introduced in 2024 for in‑app purchases. To comply with Apple’s App Store and Google Play’s in‑app purchase rules, Telegram now requires that all digital‑goods sales inside bots and mini‑apps—such as subscriptions, paid tools, AI model access, or tokens—be processed exclusively through Telegram Stars \(or GRAM for crypto‑related trades\).

**「Impact」** Developers must integrate the Stars payment flow into their bots or mini‑apps or risk immediate removal from the platform, forcing a redesign of existing monetisation models that relied on external payment processors.

<details><summary>References</summary>
<ul>
<li><a href="https://core.telegram.org/bots/payments-stars">Bot Payments API for Digital Goods and Services - Telegram APIs</a></li>

</ul>
</details>

**Tags**: `#Telegram`, `#Payments`, `#Bots`, `#AI`

---

<a id="item-tech-news-10"></a>
### [可灵 AI launches Kling Image 4.0 with native 8K generation](https://mp.weixin.qq.com/s/p3_DIBRUUgmxShjD5Wp27w) ⭐️ 7.0/10

On November 17, 可灵 AI announced the release of its Kling Image 4.0 model, which is now publicly available via an open API for enterprise customers and developers. The model supports native 8K image generation, accepts up to 15,000 tokens of text input, and can layout a single image with up to 2,000 characters using more than 70 commercial fonts. It can also produce up to 10 stylistically consistent images in a single request and create ultra‑long canvas outputs. This rollout represents a new capability rather than a measured performance claim.

telegram · zaihuapd · Nov 18, 01:05

**「Background on text‑to‑image models」** Text‑to‑image generation models translate natural‑language prompts into visual content, typically using diffusion or transformer‑based architectures. Historically, such models have been limited to resolutions of a few thousand pixels \(e.g., 1024×1024 or 4K\) and modest prompt lengths, which constrains the detail and size of the output images. Kling Image 4.0 builds on this lineage by offering native 8K generation and a much larger token window, extending the capabilities available to developers and enterprise users.

**「Impact」** Developers can immediately integrate the API to generate ultra‑high‑resolution \(8K\) visuals, enabling use cases such as premium marketing assets and detailed design mock‑ups, but must plan for the higher bandwidth and storage requirements of 8K files.

**Tags**: `#image generation`, `#AI model`, `#API`, `#8K resolution`, `#software engineering`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Former Nvidia CEO says he would return if board asks](https://x.com/JensenHuang/status/2122726005219737649) ⭐️ 8.0/10

Jensen Huang said he would be willing to resume the Nvidia CEO role if the board requests it, while the board currently says it is not considering rehiring him.

telegram · zaihuapd · Nov 17, 16:14

**「Context」** Jensen Huang resigned as Nvidia’s CEO last week following a scandal involving extramarital affairs.

<details><summary>References</summary>
<ul>
<li><a href="https://edition.cnn.com/2026/11/17/business/jensen-huang-nvidia-ceo-statement">Jensen Huang says he would be ‘honored’ to be reinstated as Nvidia ...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#Leadership`, `#Corporate Governance`, `#Stock Market`

---

<a id="item-finance-news-2"></a>
### [MIIT tasks auto association to assess 60‑day payment rule for 17 car makers](http://www.caam.org.cn/chn/5/cate_68/con_5237404.html) ⭐️ 7.0/10

The Ministry of Industry and Information Technology has asked the China Association of Automobile Manufacturers to evaluate whether 17 major car manufacturers are complying with a 60‑day supplier payment rule, as part of a push to keep payments to small‑and‑medium enterprises within 60 days.

telegram · zaihuapd · Nov 18, 01:15

**「Background」** The Ministry of Industry and Information Technology \(MIIT\) has been urging a 60‑day maximum payment term for auto‑industry suppliers to ease financing for small and medium‑sized enterprises, and now has asked the China Association of Automobile Manufacturers \(CAAM\) to verify compliance among 17 major carmakers.

<details><summary>References</summary>
<ul>
<li><a href="https://insidechinaauto.com/2025/06/14/chinese-automakers-make-60-day-supplier-payment-pledge-to-strengthen-supply-chain/">Chinese Automakers Make 60 - Day Supplier Payment Pledge To...</a></li>

</ul>
</details>

**Tags**: `#automotive industry`, `#supplier payments`, `#regulatory policy`, `#China`

---