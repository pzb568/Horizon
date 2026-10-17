---
layout: default
title: "Horizon Summary: 2026-10-17 (EN)"
date: 2026-10-17
lang: en
---

> From 40 items, 16 important content pieces were selected

---

**Technology News**
1. [Apple MLX Enables Distributed Inference of Near‑Trillion‑Parameter Models on Mac Studio](#item-tech-news-1) ⭐️ 8.0/10
2. [Anthropic unveils AI‑augmented Claude Code review with minimal human oversight](#item-tech-news-2) ⭐️ 8.0/10
3. [Report: 90% of US Work Hours Unrepresented by Current AI Benchmarks](#item-tech-news-3) ⭐️ 8.0/10
4. [OpenBSD 37-Year-Old Kernel Bug Exploited](#item-tech-news-4) ⭐️ 8.0/10
5. [\[Research\] 2,788 tokens/s on a single RTX 5090 with a diffusion LLM — Introducing ORL \(fully open source\) \[R\]](#item-tech-news-5) ⭐️ 8.0/10
6. [Nvidia denies RTX 5090 discontinuation as US listings drop and prices jump](#item-tech-news-6) ⭐️ 8.0/10
7. [Claude reveals ECDSA curve origins](#item-tech-news-7) ⭐️ 7.0/10
8. [Llama.cpp Enables GGUF Model Inference on Jailbroken PS5](#item-tech-news-8) ⭐️ 7.0/10
9. [Waymo expands autonomous ride‑hailing to Toronto](#item-tech-news-9) ⭐️ 7.0/10
10. [JPEG XL vs AVIF: size and speed trade‑offs for web images](#item-tech-news-10) ⭐️ 7.0/10
11. [I never authorized an integration that scans my secrets](#item-tech-news-11) ⭐️ 7.0/10
12. [Show HN: Gemini 4 Argon plays StarCraft](#item-tech-news-12) ⭐️ 7.0/10
13. [OpenAI launches GPT‑Live‑1.1 with six new voice languages](#item-tech-news-13) ⭐️ 7.0/10
14. [StepFun AI releases 600B‑parameter Step 5 Preview multimodal model](#item-tech-news-14) ⭐️ 7.0/10
15. [Apple iPhone Duo foldable phone sells out in a minute, stock jumps over 2%](#item-tech-news-15) ⭐️ 7.0/10

**Financial News**
1. [Anthropic IPO valuation outlook cut to $1.5 trillion](#item-finance-news-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Apple MLX Enables Distributed Inference of Near‑Trillion‑Parameter Models on Mac Studio](https://machinelearning.apple.com/research/mlx-distributed-inference) ⭐️ 8.0/10

Apple released a new version of its MLX library that adds distributed inference support for very large language models, specifically the near‑trillion‑parameter Muse Spark Open. The library runs on Mac Studio machines equipped with up to 512 GB of unified memory and can scale across a cluster of four Mac Studios, where the authors report generating more than 36 tokens per second for an 8,192‑token context. This capability is presented as a ready‑to‑use tool for developers who want to run frontier‑class models locally on Apple hardware, rather than relying on cloud services.

hackernews · antipaul · Oct 16, 13:43 · [Discussion](https://news.ycombinator.com/item?id=50118320)

**「Prerequisite: Muse Spark Open and Apple MLX」** Muse Spark Open is an open‑weight large language model released by Meta, described as the most capable U.S. open‑weight model to date with roughly 800 billion parameters and targeting Apple silicon such as the M5 Ultra Mac Studio. Apple’s MLX library is a Python‑based machine‑learning framework that provides accelerated inference on Apple GPUs and supports distributed execution across multiple Mac Studios, previously used for smaller models. Together, the model’s size and the library’s distributed inference capabilities enable near‑trillion‑parameter inference on a desktop‑class Mac Studio setup.

**「Impact」** AI engineers can now perform inference of frontier‑scale LLMs on‑premise using Mac Studio, potentially reducing cloud compute expenses, but they must have high‑memory configurations \(up to 512 GB\) or multiple machines to achieve competitive throughput.

**「Community Discussion」** One commenter noted that while Apple’s offering lets users run massive models locally, the implied cost model could involve paying Apple tens of thousands of dollars for access to the hardware, echoing concerns that the service may primarily benefit Apple’s revenue rather than the broader research community.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.meta.ai/models/muse-spark-open">Muse Spark Open | Meta</a></li>
<li><a href="https://research.meta.ai/blog/muse-spark-open">Introducing Muse Spark Open, The Most Capable US Open‑Weight ...</a></li>

</ul>
</details>

**Tags**: `#MLX`, `#distributed inference`, `#Apple hardware`, `#large language models`

---

<a id="item-tech-news-2"></a>
### [Anthropic unveils AI‑augmented Claude Code review with minimal human oversight](https://claude.dev/blog/solving-code-review-at-anthropic/) ⭐️ 8.0/10

Anthropic published a blog describing Claude Code’s AI‑augmented code review system, which automates most of the review workflow and leaves at most one human—often the author—in the loop. The process routes a reviewer’s attention only to changes deemed high‑risk, and the evaluation model is continuously retrained on each incident and code‑review change. The blog claims the system can handle tens of thousands of pull requests per day, dramatically reducing manual review effort.

hackernews · pretext · Oct 16, 19:04 · [Discussion](https://news.ycombinator.com/item?id=50122951)

**「Claude Code and its code‑review system」** Claude Code is Anthropic’s terminal‑native AI coding agent that assists developers with writing, testing, and debugging code. The platform introduced a multi‑agent pull‑request review feature earlier in 2026, and on October 15 2026 made the Code Review system generally available to Claude Team and Enterprise customers, pairing it with a promotional launch. Understanding this prior release clarifies why the blog post’s description of an AI‑augmented review workflow is notable for developers.

**「Impact」** Developers using Claude Code can expect their pull‑request triage time to shrink, as the AI handles the bulk of checks and only escalates risky changes for human attention, potentially freeing engineers to focus on higher‑value work.

**「Community Discussion」** Commenters expressed concern that the minimal‑human approach may clash with compliance standards such as SOC 2, which typically require an independent reviewer, and questioned whether the AI can reliably replace human judgment at the reported scale of 30 k PRs per day.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/resources/articles/code-review-is-now-generally-available">Code Review is now generally available | Claude by Anthropic</a></li>
<li><a href="https://www.unite.ai/anthropic-makes-code-review-for-claude-code-generally-available/">Anthropic Makes Code Review for Claude Code Generally ...</a></li>
<li><a href="https://convly.ai/claude-code-review-2026/">Claude Code Review (2026): The Terminal Agent That Actually</a></li>

</ul>
</details>

**Tags**: `#code review`, `#AI‑assisted development`, `#software engineering`, `#dev tools`, `#Anthropic`

---

<a id="item-tech-news-3"></a>
### [Report: 90% of US Work Hours Unrepresented by Current AI Benchmarks](https://www.mercor.com/research/labor-index/benchmark-map/) ⭐️ 8.0/10

A new Mercor research report finds that roughly 90% of U.S. working hours are spent on tasks that existing AI benchmarks cover poorly or not at all, indicating a large mismatch between benchmark prompts and real‑world work. The analysis notes that benchmark sets are heavily weighted toward high‑wage occupations, leaving most everyday tasks under‑represented.

hackernews · speckx · Oct 16, 17:08 · [Discussion](https://news.ycombinator.com/item?id=50121179)

**「Context on AI Benchmarks and Job Task Mapping」** AI benchmarks are curated sets of tasks \(e.g., MMLU, BIG‑bench\) used to gauge model performance, but they have historically been limited to a narrow slice of real‑world work. Prior analyses have shown that only a small fraction of occupations are directly represented by these benchmarks—Mercor’s earlier mapping found that just 208 of the 923 U.S. occupations appear in existing benchmark suites, leaving most job tasks unmeasured. This background explains why the new report’s claim that roughly 90% of U.S. working hours lack adequate benchmark coverage is significant.

**「Impact」** The gap makes it difficult for developers and enterprises to gauge how well AI models will perform on the majority of workplace tasks, prompting a push for broader, more representative evaluation suites before deploying AI‑assisted automation.

**「Community Discussion」** Commenters argue the benchmark coverage is superficial—for example, labeling a social‑worker category as “well covered” despite only 13 prompts, and warning that such limited representations risk misleading claims about AI’s readiness for most jobs.

<details><summary>References</summary>
<ul>
<li>Mercor Research mapped AI benchmarks to actual US jobs ... - X</li>

</ul>
</details>

**Tags**: `#AI benchmarks`, `#labor market`, `#AI evaluation`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [OpenBSD 37-Year-Old Kernel Bug Exploited](https://calif.io/research/big-fish) ⭐️ 8.0/10

Researchers have demonstrated an exploit against a kernel bug in OpenBSD that has existed for 37 years. The vulnerability, present in the core of the operating system, was uncovered and successfully leveraged despite the codebase’s long history of extensive auditing. This finding highlights that even heavily reviewed kernels can harbor deep, long‑standing flaws that remain undetected.

hackernews · rs\_rs\_rs\_rs\_rs · Oct 16, 14:44 · [Discussion](https://news.ycombinator.com/item?id=50118977)

**「Prerequisite context」** OpenBSD’s kernel has long been praised for rigorous code review and security hardening such as KASLR, SMAP and SMEP, yet the exploit chains a 37‑year‑old integer overflow in a shared‑memory counter with a later out‑of‑bounds write to gain root on OpenBSD 7.9. The underlying flaw originates from the original BSD source code and survived multiple releases before being addressed in an errata after the proof‑of‑concept was published.

**「Impact」** OpenBSD maintainers will need to issue a security patch to remediate the bug, and administrators should apply the update promptly to protect systems from potential attacks.

**「Community Discussion」** Commenters noted that the same code had been unintentionally fixed in NetBSD in 1999, and they debated whether fuzzing or static analysis could have discovered such a long‑lived kernel flaw, suggesting that human insight was crucial in this case.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/10/researchers-demonstrate-openbsd-root.html">Researchers Demonstrate OpenBSD Root Exploit Chaining 37-Year ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#openbsd`, `#kernel`, `#vulnerability`

---

<a id="item-tech-news-5"></a>
### [\[Research\] 2,788 tokens/s on a single RTX 5090 with a diffusion LLM — Introducing ORL \(fully open source\) \[R\]](https://www.reddit.com/r/MachineLearning/comments/1x7qgr0/research_2788_tokenss_on_a_single_rtx_5090_with_a/) ⭐️ 8.0/10

ORL introduces a fast, open‑source approach to diffusion LLM inference, delivering multi‑fold token‑throughput gains on modern GPUs.

reddit · r/MachineLearning · /u/arty\_photography · Oct 16, 20:03

**Tags**: `#diffusion-LLM`, `#inference-optimization`, `#open-source`, `#hardware-acceleration`

---

<a id="item-tech-news-6"></a>
### [Nvidia denies RTX 5090 discontinuation as US listings drop and prices jump](https://www.techpowerup.com/353578/nvidia-reportedly-ending-the-rtx-5090-reserves-gb202-silicon-for-workstation-gpus) ⭐️ 8.0/10

Rumors that Nvidia has halted production of the RTX 5090/V2 and stopped supplying GB202 silicon to the GeForce line were publicly denied by senior VP Jeff Fisher, who called the claim &quot;not factual&quot; but admitted supply constraints. Despite the denial, the official US store removed the RTX 5090 page and retailers such as Micro Center marked it &quot;no longer sold,&quot; while the 32 GB model’s price in China rose from about ¥35,000 in early September to roughly ¥54,000 by mid‑October. The alleged shift would redirect GB202 capacity to the higher‑margin RTX PRO line, and the consumer flagship is now the RTX 5080 24 GB, built on a smaller GB203 die yet priced at flagship levels.

telegram · zaihuapd · Oct 17, 00:02

**「Prerequisite context」** The RTX 5090 is Nvidia’s top‑end consumer graphics card built on the GB202 Ada Lovelace silicon, positioned above the RTX 5080 and traditionally sold to gamers and creators. Nvidia also offers a separate RTX PRO line of workstation GPUs that use the same silicon family for higher‑margin professional workloads, which the company can prioritize if it reallocates production capacity.

**「Impact」** AI/ML developers and researchers who rely on the RTX 5090 for high‑end workloads may face reduced availability and sharply higher costs, prompting them to consider the less powerful RTX 5080 or alternative GPU vendors to stay within budget.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/products/workstations/professional-desktop-gpus/">RTX PRO in Desktops | Built For Professionals | NVIDIA</a></li>

</ul>
</details>

**Tags**: `#GPU`, `#Nvidia`, `#AI/ML`, `#Hardware`, `#TechIndustry`

---

<a id="item-tech-news-7"></a>
### [Claude reveals ECDSA curve origins](https://www.anthropic.com/research/ecdsa-curve-origins) ⭐️ 7.0/10

Anthropic&\#x27;s Claude uncovered that NIST elliptic curve seeds were generated using a simple timestamp‑seeded RNG, raising security concerns for many systems.

hackernews · ahlCVA · Oct 16, 18:55 · [Discussion](https://news.ycombinator.com/item?id=50122800)

**Tags**: `#cryptography`, `#security`, `#software engineering`, `#industry`

---

<a id="item-tech-news-8"></a>
### [Llama.cpp Enables GGUF Model Inference on Jailbroken PS5](https://github.com/cobanov/PS5LM) ⭐️ 7.0/10

A GitHub project \(cobanov/PS5LM\) demonstrates that a jailbroken PlayStation 5 can run llama.cpp and load any GGUF‑format LLM, exemplified by the 27‑billion‑parameter Qwen 3.8 model quantised to 2 bits. The hack repurposes the console’s custom AMD Zen 2‑based CPU and GPU as a low‑cost edge inference device, consuming roughly $0.70 per day in electricity for about 2 million output tokens. This capability is limited to hobbyist users with modified hardware and is not supported by Sony, so it remains a niche, unofficial solution rather than a commercial offering.

hackernews · Anon84 · Oct 16, 18:32 · [Discussion](https://news.ycombinator.com/item?id=50122431)

**「Prerequisites: llama.cpp, GGUF, and PS5 homebrew」** llama.cpp is a C/C++ inference engine that runs Llama‑compatible models packaged in the GGUF file format, allowing local execution on CPUs without GPU acceleration. The GGUF format is produced by converting HuggingFace checkpoints with the llama.cpp conversion script, which prepares models for efficient on‑device inference. A jailbroken PlayStation 5 can run unsigned code, turning the console into a general‑purpose Linux‑like environment where homebrew applications such as llama.cpp can be compiled and executed.

**「Low‑cost edge inference on a jailbroken PS5」** A jailbroken PlayStation 5 can now act as a private AI inference node, running the 27‑billion‑parameter Qwen‑3.8‑27B GGUF model at roughly 20 tokens per second and smaller models up to about 124 tokens per second, while drawing only ~70 cents of electricity per day. This provides hobbyists with a sub‑dollar‑per‑day edge‑compute option, but it requires a modified console and is not suitable for production‑grade workloads.

**「Community Discussion」** Commenters note the practical appeal of turning a PS5 into a cheap compute node—jjcm cites power‑cost efficiency and potential tasks like server monitoring—while Rabbit504030201 warns that hosting the project on GitHub risks takedown by Sony, suggesting a more independent domain would be safer.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/docs/inference-endpoints/engines/llama_cpp">llama.cpp · Hugging Face</a></li>
<li><a href="https://huggingface.co/docs/hub/gguf-llamacpp">GGUF usage with llama.cpp · Hugging Face</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/discussions/2948">Tutorial: How to convert HuggingFace model to GGUF format</a></li>
<li><a href="https://www.analyticsinsight.net/news/jailbroken-ps5-turns-into-a-local-ai-machine-with-speeds-above-100-tokens-per-second">Jailbroken PS5 Turns into a Local AI Machine with Speeds ...</a></li>
<li><a href="https://wccftech.com/jailbroken-ps5-local-ai-server-27b-llm/">A Jailbroken PS5 Got Turned Into a Local AI Server That Can ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#Edge Computing`, `#Hardware Hacking`, `#Open Source`

---

<a id="item-tech-news-9"></a>
### [Waymo expands autonomous ride‑hailing to Toronto](https://waymo.com/blog/2026/10/waymo-in-toronto/) ⭐️ 7.0/10

Waymo announced it will launch its autonomous ride‑hailing service in Toronto, extending its commercial operations beyond the United States. The rollout is slated for later this year and will initially cover a limited service area while creating local jobs, as noted in the company blog. The expansion follows Waymo’s existing deployments in Phoenix, Austin and San Francisco, marking its first full‑scale service in Canada.

hackernews · ChrisArchitect · Oct 16, 14:44 · [Discussion](https://news.ycombinator.com/item?id=50118981)

**「Waymo’s existing service footprint and prior Toronto speculation」** Waymo’s driverless ride‑hailing service is currently available in Los Angeles, the San Francisco Bay Area, Phoenix, Austin and Atlanta, and earlier reports noted Toronto as a potential expansion market. Those reports from late 2025 described Toronto’s interest in allowing Waymo taxis and highlighted the city’s consideration of the service. This context explains why the October 2026 announcement of an actual launch in Toronto is notable.

**「Impact」** Toronto residents will be able to request driverless rides through the Waymo app, and the company will need to secure approval from Transport Canada and local authorities, potentially shaping Canadian autonomous‑vehicle regulations.

**「Community Discussion」** Comments on the announcement show mixed experiences: some users praise Waymo rides in San Francisco, while others report long delays and navigation problems in Austin, indicating reliability can vary across cities.

<details><summary>References</summary>
<ul>
<li><a href="https://mobilesyrup.com/2025/12/02/toronto-waymo-self-driving-taxis/">Toronto looking into allowing Waymo self-driving taxis</a></li>
<li><a href="https://www.blogto.com/tech/2025/12/waymo-toronto/">Waymo self-driving taxis could be coming to Toronto</a></li>

</ul>
</details>

**Tags**: `#autonomous-vehicles`, `#Waymo`, `#self-driving`, `#AI`, `#transportation`

---

<a id="item-tech-news-10"></a>
### [JPEG XL vs AVIF: size and speed trade‑offs for web images](https://jakearchibald.com/2026/jpeg-xl-vs-avif/) ⭐️ 7.0/10

The article by farlight on jakearchibald.com presents a detailed comparison of JPEG XL and AVIF for typical web‑image scenarios, measuring file size reductions and encoding/decoding speeds across photos, screenshots, and illustrations. It shows that JPEG XL can achieve 2–7 % smaller files for photos and up to ~25 % for screenshots/illustrations when using its highest‑effort settings, but those settings are dramatically slower \(up to 180× longer\) than AVIF’s default encoder. Conversely, AVIF generally encodes faster while still delivering competitive compression, making the choice dependent on the developer’s priority between size and performance.

hackernews · farlight · Oct 16, 16:12 · [Discussion](https://news.ycombinator.com/item?id=50120224)

**「Background on JPEG XL and AVIF」** JPEG XL and AVIF are modern image codecs introduced as successors to JPEG and WebP, offering higher compression efficiency, HDR and lossless support, and progressive decoding for web delivery. Both formats are now supported in major browsers—AVIF in roughly 93% of browsers while JPEG XL has more limited adoption—and have been the focus of several 2026 benchmark studies that measured file size, visual quality, and encoding speed on high‑resolution images. Those prior comparisons provide the technical context for the article’s detailed trade‑off analysis.

**「Impact」** Web developers can use the benchmark results to decide which format and encoder settings best fit their delivery pipeline—opting for AVIF when encoding speed is critical, or selecting high‑effort JPEG XL when marginal size savings outweigh longer processing times.

**「Community discussion」** Commenter yhjc2692 notes that libjxl’s maximum‑effort mode, while yielding 2–7 % smaller photos and ~25 % smaller screenshots/illustrations, requires 9–46 seconds per image—50–180× slower than the default—making it impractical for many production workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://lpic.cc/en/blog/webp-avif-jpegxl-format-comparison">WebP vs AVIF vs JPEG XL 2026: Complete Format Comparison ...</a></li>
<li><a href="https://cleanor.app/blog/next-gen-image-formats-2026-avif-webp-jpeg-xl-benchmark">AVIF vs WebP vs JPEG XL: Best Web Image Format 2026</a></li>
<li><a href="https://fileza.io/articles/avif-vs-jpeg-xl-2026-comparison">AVIF vs JPEG XL in 2026: The Definitive Format Comparison for ...</a></li>

</ul>
</details>

**Tags**: `#image formats`, `#web performance`, `#compression`

---

<a id="item-tech-news-11"></a>
### [I never authorized an integration that scans my secrets](https://github.com/home-assistant/home-assistant.io/issues/49314) ⭐️ 7.0/10

A Home Assistant security feature that checks passwords against breach databases can be turned off, raising privacy concerns for users and developers.

hackernews · trvrprkr · Oct 16, 20:33 · [Discussion](https://news.ycombinator.com/item?id=50124251)

**Tags**: `#security`, `#privacy`, `#home-assistant`, `#open-source`, `#software-engineering`

---

<a id="item-tech-news-12"></a>
### [Show HN: Gemini 4 Argon plays StarCraft](https://starskirmish.com/bench/v0-2/) ⭐️ 7.0/10

A new benchmark shows how top LLMs perform when writing code to play StarCraft, highlighting comparative strengths and research directions.

hackernews · \_\_cayenne\_\_ · Oct 16, 14:18 · [Discussion](https://news.ycombinator.com/item?id=50118688)

**Tags**: `#LLM benchmarking`, `#Game AI`, `#Code generation`, `#AI research`

---

<a id="item-tech-news-13"></a>
### [OpenAI launches GPT‑Live‑1.1 with six new voice languages](https://x.com/OpenAI/status/2110797830361436604) ⭐️ 7.0/10

OpenAI released GPT‑Live‑1.1, updating its voice model for ChatGPT, Codex and the “点点” service. The new version adds support for six additional languages—French, German, Hindi, Mexican Spanish, Korean and Japanese—improves accent rendering and reduces the “checking…” latency. API access to the model is announced to roll out soon.

telegram · zaihuapd · Oct 16, 04:50

**「Background on GPT‑Live voice model」** GPT‑Live is OpenAI’s real‑time speech model that powers voice interaction in products such as ChatGPT and Codex. The initial release \(GPT‑Live 1.0\) provided English‑only voice output, enabling developers to add spoken responses to applications via the platform’s API. The new GPT‑Live‑1.1 update builds on that foundation by adding six additional languages and improving latency, which is why the language expansion is notable for developers using the existing voice capabilities.

**「Impact」** Developers can now integrate higher‑quality, lower‑latency speech in the newly supported languages, expanding multilingual voice‑enabled applications without waiting for a separate model release.

**Tags**: `#OpenAI`, `#speech AI`, `#multilingual support`, `#API update`

---

<a id="item-tech-news-14"></a>
### [StepFun AI releases 600B‑parameter Step 5 Preview multimodal model](https://huggingface.co/stepfun-ai/Step-5-Preview) ⭐️ 7.0/10

StepFun AI has released the Step 5 Preview model on Hugging Face, a 600‑billion‑parameter mixture‑of‑experts \(MoE\) model with 270 billion active parameters. It supports up to 1 million token context and accepts text, image, and video inputs. The model can be accessed via an OpenAI‑compatible API using vLLM or SGLang and is distributed under the StepFun Model License 1.0. Performance claims for software‑engineering, long‑running agents, and finance tasks are unverified and come from an informal announcement.

telegram · zaihuapd · Oct 16, 06:36

**「Background」** Mixture‑of‑Experts \(MoE\) models activate only a fraction of their total parameters for each token, enabling total parameter counts in the hundreds of billions while keeping inference costs similar to smaller dense models. Recent multimodal MoE systems such as DeepSeek‑V 4.1‑Flash have shown that this architecture can process text and image inputs and support context windows up to one million tokens, a capability that StepFun’s new Step 5 Preview extends for software‑engineering and agent workloads. The model can be accessed through OpenAI‑compatible APIs and deployed with runtimes like vLLM or SGLang, which are now standard for serving large generative models.

**「Impact」** Developers can now experiment with a very large multimodal model that handles extremely long contexts, enabling more capable AI agents and software‑engineering tools, but deploying it will require substantial GPU memory and compute resources.

<details><summary>References</summary>
<ul>
<li><a href="https://build.nvidia.com/stepfun-ai/step-5-preview">Step 5 Preview Model by Stepfun-ai | NVIDIA NIM</a></li>
<li><a href="https://www.i-scoop.eu/stepfun-step-5-preview/">StepFun Step 5 Preview uit Shanghai | i-SCOOP</a></li>

</ul>
</details>

**Tags**: `#large-language-model`, `#multimodal`, `#AI-agents`, `#software-engineering`, `#long-context`

---

<a id="item-tech-news-15"></a>
### [Apple iPhone Duo foldable phone sells out in a minute, stock jumps over 2%](https://api3.cls.cn/share/article/2507193?os=android&amp;amp;sv=8.8.4&amp;amp;app=cailianpress) ⭐️ 7.0/10

Apple launched its first foldable smartphone, the iPhone Duo, and reported that all units across every model were sold out within one minute of opening sales. The rapid sell‑out coincided with a pre‑market rise of more than 2% in Apple’s U.S. stock price, pushing the opening price to a historic high. The report reflects a vendor claim of immediate market demand rather than an independently measured sales figure.

telegram · zaihuapd · Oct 16, 12:45

**「Prerequisite: Apple’s first foldable iPhone announcement」** Apple announced its first foldable iPhone, the iPhone Duo, in September 2026, highlighting a 7.6‑inch inner display and a nano‑texture finish, and opened pre‑orders for the device on October 16 2026 at 5 a.m. PT. The Duo marks Apple’s entry into the foldable‑screen market, a segment previously led by Android manufacturers.

**「Impact」** Investors responded to the sell‑out news with a short‑term boost in Apple’s share price, as evidenced by the &gt;2% pre‑market increase, suggesting heightened market optimism around Apple’s entry into the foldable‑phone segment.

<details><summary>References</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/10/open-up-to-new-possibilities-with-iphone-duo/">Open up to new possibilities with iPhone Duo - Apple</a></li>
<li><a href="https://www.apple.com/newsroom/2026/09/apple-unveils-iphone-duo/">Apple unveils iPhone Duo</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#mobile`, `#market`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Anthropic IPO valuation outlook cut to $1.5 trillion](https://www.reuters.com/business/finance/investors-temper-anthropic-ipo-valuation-expectations-over-revenue-growth-2026-10-15/) ⭐️ 7.0/10

Investors reduced Anthropic&\#x27;s expected IPO valuation from $2 trillion to about $1.5 trillion, citing slower revenue growth, intensified model‑price competition and higher compute‑cost pressures.

telegram · zaihuapd · Oct 16, 15:46

**「Prior valuation expectations」** Earlier, investors had expected Anthropic’s IPO valuation to be about $2 trillion, reflecting its fast‑growing Q3 2026 revenue and a planned $518 billion cloud‑spending commitment over the next decade.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tipranks.com/news/anthropic-ipo-why-investors-are-rethinking-its-2-trillion-valuation">Anthropic IPO: Why Investors Are Rethinking Its $2 Trillion ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#IPO`, `#Valuation`, `#Anthropic`, `#TechSector`

---