---
layout: default
title: "Horizon Summary: 2026-11-08 (EN)"
date: 2026-11-08
lang: en
---

> From 39 items, 15 important content pieces were selected

---

**Technology News**
1. [Claude Code&\#x27;s &quot;Don&\#x27;t Ask Again&quot; exposes passwords in 1,122 public GitHub files](#item-tech-news-1) ⭐️ 8.0/10
2. [MaxxBench – &quot;Nice DeepSWE score. But is it true?&quot;](#item-tech-news-2) ⭐️ 8.0/10
3. [GitHub Rubicon architecture enables 7200 pushes per second](#item-tech-news-3) ⭐️ 8.0/10
4. [The end of Microsoft Research&\#x27;s AI Frontiers group](#item-tech-news-4) ⭐️ 7.0/10
5. [Discord highlights Electron’s RAM bloat on Windows 11](#item-tech-news-5) ⭐️ 7.0/10
6. [Fedora Asahi Remix 45 ships same day as Fedora 45, Asahi Linux 7.3 still lacks USB‑C display support](#item-tech-news-6) ⭐️ 7.0/10
7. [We Visited China’s Stargate in Inner Mongolia](#item-tech-news-7) ⭐️ 7.0/10
8. [Microsoft winds down Oracle AI compute rental agreement](#item-tech-news-8) ⭐️ 7.0/10
9. [🍏 苹果称 iPhone Duo 适配应用已超 10 万个](#item-tech-news-9) ⭐️ 7.0/10
10. [Tesla Optimus robot may be offered only for rent](#item-tech-news-10) ⭐️ 7.0/10
11. [Claude Code web search may leak user email addresses](#item-tech-news-11) ⭐️ 7.0/10
12. [🤖 Claude Max 用量宣传被诉，Anthropic 被判决须应诉](#item-tech-news-12) ⭐️ 7.0/10
13. [Apple unveils HALO humanoid robot system using two Qwen models](#item-tech-news-13) ⭐️ 7.0/10
14. [Democratic Lawmaker Calls for Ban on AI Recursive Self‑Improvement](#item-tech-news-14) ⭐️ 7.0/10

**Financial News**
1. [SoftBank, ABB consider carving out China robotics unit to rescue $5.4 billion deal](#item-finance-news-1) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Claude Code&\#x27;s &quot;Don&\#x27;t Ask Again&quot; exposes passwords in 1,122 public GitHub files](https://apiiro.com/blog/coding-agents-leaking-secrets-github-dont-ask-again) ⭐️ 8.0/10

Claude Code’s “Don’t Ask Again” feature can expose secrets if local settings are committed, underscoring AI‑assistant security concerns.

hackernews · shmulc · Nov 7, 20:45 · [Discussion](https://news.ycombinator.com/item?id=50407882)

**Tags**: `#AI coding assistants`, `#secret leakage`, `#software security`, `#GitHub`, `#developer tooling`

---

<a id="item-tech-news-2"></a>
### [MaxxBench – &quot;Nice DeepSWE score. But is it true?&quot;](https://maxxbench.unlap.ai/research/why-maxxbench/) ⭐️ 8.0/10

A Hacker News debate examines the validity of MaxxBench&\#x27;s DeepSWE scores, raising broader questions about LLM benchmark trustworthiness.

hackernews · antiuniverse · Nov 7, 17:19 · [Discussion](https://news.ycombinator.com/item?id=50406222)

**Tags**: `#benchmarks`, `#LLM evaluation`, `#AI research`

---

<a id="item-tech-news-3"></a>
### [GitHub Rubicon architecture enables 7200 pushes per second](https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/) ⭐️ 8.0/10

GitHub has introduced a new Git storage system called Rubicon that stores objects in Azure Blob Storage and manages references with a Ref‑CAS layer. In internal tests the architecture handled 5,000 concurrent AI agents working on a single repository, processing up to 7,200 push operations per second while keeping read latency low. The system uses virtual replicas for read/write handling and background nodes for data‑packet compression. Rubicon is currently available only in a limited private preview and will be rolled out more broadly over time.

telegram · zaihuapd · Nov 7, 14:12

**「Prerequisite concepts」** Git repositories store objects \(packs and auxiliary data\) and reference metadata that historically reside on tightly coupled storage systems. Rubicon separates these layers by placing Git objects in Azure Blob Storage while managing references and pack manifests in a dedicated Ref‑CAS log service, reducing coordination overhead and enabling higher concurrency for AI‑driven workflows.

**「Impact」** Teams that rely on AI‑driven tooling or need to support many simultaneous contributors can request access to the preview to benefit from dramatically higher push throughput, but must adapt their workflows to the new storage backend and reference model.

<details><summary>References</summary>
<ul>
<li><a href="https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/">Inside GitHub’s new Git storage architecture - The GitHub Blog</a></li>

</ul>
</details>

**Tags**: `#GitHub`, `#Infrastructure`, `#AI tooling`

---

<a id="item-tech-news-4"></a>
### [The end of Microsoft Research&\#x27;s AI Frontiers group](https://hunch.net/?p=13764006) ⭐️ 7.0/10

Microsoft Research is ending its AI Frontiers group, signaling a strategic move toward transformer‑centric scaling over exploratory AI research.

hackernews · srean · Nov 7, 18:02 · [Discussion](https://news.ycombinator.com/item?id=50406563)

**Tags**: `#Microsoft Research`, `#AI research strategy`, `#industry trends`

---

<a id="item-tech-news-5"></a>
### [Discord highlights Electron’s RAM bloat on Windows 11](https://www.windowslatest.com/2026/11/06/every-windows-11-app-should-kill-electron-and-discord-just-showed-why-no-starting-screen-and-70-less-ram-even-with-two-accounts-signed-in/) ⭐️ 7.0/10

The article demonstrates that Discord’s Electron‑based Windows 11 client consumes a large amount of memory—up to 70 % more RAM and shows a sluggish start‑up screen—even with only two accounts signed in, and contrasts this with a newer native client that starts instantly and uses far less RAM. It concludes that Windows 11 developers should stop using Electron for new apps and adopt lighter‑weight native frameworks.

hackernews · thunderbong · Nov 7, 11:11 · [Discussion](https://news.ycombinator.com/item?id=50403507)

**「What is Electron and why Discord’s Rust client matters」** Electron is a framework that lets developers create cross‑platform desktop applications with web technologies by bundling a Chromium engine, which typically results in multi‑gigabyte RAM usage on Windows 11. Discord has historically used Electron, but it recently released a Rust‑based client \(named Phoenix\) that launches before the Electron version finishes loading and consumes roughly 290 MB of RAM when two accounts are signed in, illustrating a lower‑memory alternative to the usual Electron approach.

**「Impact」** Developers building desktop applications for Windows 11 may need to reconsider Electron and evaluate alternatives such as WinUI, Rust GUI toolkits, or Kotlin Multiplatform to avoid the high memory overhead that can degrade user experience on low‑RAM systems.

**「Community discussion」** Commenters note that Electron’s RAM usage has been a long‑standing complaint \(e.g., VS Code\) and praise its accessibility support, but many agree the memory cost is increasingly unacceptable given today’s RAM prices, urging a shift toward more efficient native solutions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.windowslatest.com/2026/11/06/every-windows-11-app-should-kill-electron-and-discord-just-showed-why-no-starting-screen-and-70-less-ram-even-with-two-accounts-signed-in/">Every Windows 11 app should kill Electron, and Discord just ...</a></li>
<li><a href="https://todayforai.com/en/items/art-5eb62195-e80">Discord Rewrites Client in Rust, Beating Electron on Cold ...</a></li>

</ul>
</details>

**Tags**: `#electron`, `#windows-11`, `#desktop-app-development`, `#performance`

---

<a id="item-tech-news-6"></a>
### [Fedora Asahi Remix 45 ships same day as Fedora 45, Asahi Linux 7.3 still lacks USB‑C display support](https://asahilinux.org/2026/11/progress-report-7-3/) ⭐️ 7.0/10

The Asahi Linux 7.3 progress report notes that Fedora Asahi Remix 45 was released on 3 November, the same day as upstream Fedora 45, marking the first time a new Fedora Asahi Remix version has coincided with the upstream release. The report also highlights ongoing hardware support gaps for Apple Silicon, most notably the lack of USB‑C external‑display support, which remains a blocker for many users.

hackernews · ackyshake · Nov 7, 05:20 · [Discussion](https://news.ycombinator.com/item?id=50401867)

**「Prerequisite: Asahi Linux on Apple Silicon」** Asahi Linux is the community project that ports the mainline Linux kernel to run on Apple Silicon Macs, contributing upstream patches such as the macaudio and avd drivers for the Linux 7.3 kernel. Fedora Asahi Remix is a downstream Fedora spin that packages Asahi‑enabled kernels for Apple Silicon, and its version 45 was released in sync with Fedora 45 on 3 November 2026. The progress report builds on these upstream and downstream efforts to improve hardware support for newer M‑series chips.

**「Impact」** Developers and users can now obtain the latest Fedora Asahi Remix immediately after Fedora 45’s release, simplifying testing and deployment on Apple Silicon, but the missing USB‑C display support may still deter users who need external monitors, requiring them to wait for future Asahi Linux updates.

**「Community Discussion」** One commenter pointed out that the absence of USB‑C display support is the only remaining obstacle for them to adopt Asahi Linux, indicating that hardware‑feature priorities are a source of frustration among potential users.

<details><summary>References</summary>
<ul>
<li><a href="https://asahilinux.org/2026/11/progress-report-7-3/">Progress Report: Linux 7.3 - Asahi Linux</a></li>
<li><a href="https://asahilinux.org/2026/11/progress-report-7-3/">Progress Report: Linux 7.3 - Asahi Linux</a></li>

</ul>
</details>

**Tags**: `#Linux`, `#Apple Silicon`, `#Open Source`, `#Operating Systems`

---

<a id="item-tech-news-7"></a>
### [We Visited China’s Stargate in Inner Mongolia](https://newsletter.semianalysis.com/p/we-visited-chinas-stargate-in-inner) ⭐️ 7.0/10

The piece reports on a massive Chinese AI datacenter, highlighting its scale, cost efficiency, and strategic significance.

rss · Semianalysis · Nov 7, 19:01

**Tags**: `#AI infrastructure`, `#datacenters`, `#China`, `#compute scaling`

---

<a id="item-tech-news-8"></a>
### [Microsoft winds down Oracle AI compute rental agreement](https://www.bloomberg.com/news/articles/2026-11-06/microsoft-is-winding-down-oracle-deal-to-rent-ai-cloud-capacity) ⭐️ 7.0/10

Microsoft is gradually ending its AI compute rental agreement with Oracle, having not renewed the contract in recent months. The Oracle hardware relies on older-generation Nvidia chips that no longer meet Microsoft&\#x27;s requirements. The deal, announced in 2023 to support the AI‑powered version of Bing, is being phased out as Microsoft shifts its AI infrastructure strategy.

telegram · zaihuapd · Nov 7, 02:00

**「2023 Microsoft‑Oracle AI rental deal」** In 2023 Microsoft announced a deal to rent GPU capacity from Oracle to power the AI‑enhanced version of Bing, a rare cross‑cloud partnership that relied on Oracle’s servers equipped with older‑generation NVIDIA chips. The agreement let Microsoft supplement its own Azure compute while Oracle marketed its AI infrastructure as strong demand, later renewing a four‑year‑old GPU contract at a premium. This prior arrangement provides the context for Microsoft’s current decision to wind down the rental agreement.

**「Impact」** Microsoft will need to source the required AI compute from its own Azure cloud or other providers, reducing Oracle&\#x27;s AI‑related revenue and signaling a broader move away from third‑party GPU rentals for large‑scale AI workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://www.zerohedge.com/markets/microsoft-pulls-plug-oracle-ai-rental-post-election-data-center-fallout-spreads">Microsoft Pulls The Plug On Oracle AI Rental As... | ZeroHedge</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#Oracle`, `#AI compute`, `#Cloud infrastructure`, `#Hardware`

---

<a id="item-tech-news-9"></a>
### [🍏 苹果称 iPhone Duo 适配应用已超 10 万个](https://9to5mac.com/2026/11/06/apple-says-there-are-already-over-100000-apps-built-for-iphone-duo/) ⭐️ 7.0/10

Apple reports over 100,000 apps adapted for the iPhone Duo, indicating rapid developer adoption.

telegram · zaihuapd · Nov 7, 02:30

**Tags**: `#iPhone Duo`, `#App Store`, `#Mobile Development`

---

<a id="item-tech-news-10"></a>
### [Tesla Optimus robot may be offered only for rent](https://www.ithome.com/1/023/675.htm) ⭐️ 7.0/10

Elon Musk said at the 33rd Barron&\#x27;s Investor Conference that Tesla’s Optimus humanoid robot will likely be available only through a rental model, with no purchase option disclosed. Early production began in October at the Fremont factory, targeting a capacity of one million units per year, but full‑scale production is expected to take another year, with external deliveries planned for around the end of 2027.

telegram · zaihuapd · Nov 7, 06:33

**「Earlier Optimus developments」** Tesla first unveiled the humanoid Optimus robot in 2021 and has since shown prototype demonstrations, with a 2024 announcement that early production would begin at its Fremont factory. Recent reports indicated the start of limited‑volume manufacturing and a target of scaling to tens of thousands of units per week by 2027, providing context for Musk’s latest comment about offering the robot only on a rental basis.

**「Impact」** Enterprises that want to use Optimus will need to budget for ongoing lease fees rather than a one‑time purchase, shifting capital expenditures to operating expenses and potentially limiting adoption to firms comfortable with subscription‑style hardware costs.

<details><summary>References</summary>
<ul>
<li><a href="https://interestingengineering.com/ai-robotics/tesla-optimus-robot-enters-production">Tesla Optimus production starts as Musk targets 20,000 robots weekly</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#AI`, `#hardware`, `#industry-news`

---

<a id="item-tech-news-11"></a>
### [Claude Code web search may leak user email addresses](https://github.com/anthropics/claude-code/issues/107757) ⭐️ 7.0/10

Developers reported that Claude Code inserts the logged‑in user&\#x27;s email address into outbound web‑search requests, causing the address to be sent to sites such as Wikipedia and the U.S. Securities and Exchange Commission. The issue originated from a fix that added the email to the model context to stop Claude from inserting author names. Version 2.1.317 introduced a filter that blocks the email, but it can be bypassed with a Python script, and Anthropic plans to remove the email from the context entirely in the next release.

telegram · zaihuapd · Nov 7, 08:09

**「Claude Code’s web‑search behavior」** Claude Code is Anthropic’s AI‑assisted coding tool that can issue web requests on behalf of the user. To stop the model from inserting incorrect author names, engineers previously placed the logged‑in user’s email address into the model’s context, which caused the email to be automatically included in outbound HTTP headers when Claude performed searches. This design flaw, first reported in July 2026, led to the address being sent to sites such as Wikipedia and the U.S. Securities and Exchange Commission, prompting the current security fix.

**「Impact」** Affected developers may receive large volumes of phishing or scam emails, and should monitor for the upcoming version that removes the email from the model context or apply temporary mitigations such as disabling web‑search features.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gate.com/news/detail/claude-code-automatically-leaks-user-email-to-wikipedia-sec-anthropic-25467614">Claude Code Automatically Leaks User Email to Wikipedia, SEC ...</a></li>
<li><a href="https://explainx.ai/blog/claude-code-leaks-your-email-user-agent-header-how-to-stop-it-2026">Claude Code Leaks Your Email in Headers: 5-Min Fix - explainx.ai</a></li>
<li><a href="https://cellcog.ai/blog/claude-code-email-leak/">Claude Code Sent User Emails to Websites: What Happened</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#privacy`, `#Claude Code`, `#software engineering`

---

<a id="item-tech-news-12"></a>
### [🤖 Claude Max 用量宣传被诉，Anthropic 被判决须应诉](https://thenextweb.com/news/anthropic-claude-max-lawsuit-ruling-usage-claims) ⭐️ 7.0/10

Anthropic must respond to claims that its Claude Max pricing was misleading, a notable legal development for the AI industry.

telegram · zaihuapd · Nov 7, 12:44

**Tags**: `#AI`, `#Legal`, `#Anthropic`, `#Pricing`

---

<a id="item-tech-news-13"></a>
### [Apple unveils HALO humanoid robot system using two Qwen models](https://weibo.com/1642634100/RqjjGllvw) ⭐️ 7.0/10

Apple&\#x27;s research team posted a preprint on arXiv on November 4 describing HALO, a three‑layer autonomous control system for a humanoid robot. The top layer uses the Qwen3.6‑35B‑A3B model to plan tasks, the middle layer employs Qwen3.5‑2B to generate motion commands, and the bottom layer is a reinforcement‑learning‑trained motion tracker. The system was validated on the Yu‑Shu G1 robot, successfully transferring actions learned in simulation to a previously unseen real‑world room, and the data, training pipelines, and deployment code have been released publicly.

telegram · zaihuapd · Nov 7, 13:35

**「Background」** HALO builds on recent research that trains robot control policies entirely in simulation and then deploys them onboard physical humanoids, avoiding costly real‑world data collection. The HALO preprint \(arXiv 2611.06908\) details a three‑tier architecture—an upper‑level Qwen 3.6‑35B‑A3B model for task planning, a mid‑level Qwen 3.5‑2B model for motion generation, and a reinforcement‑learning‑trained low‑level controller for motion tracking—and the associated code has been released on GitHub.

**「Impact」** The open‑source release gives robotics researchers a concrete, reproducible stack that combines large language models with RL‑based low‑level control, potentially speeding up development of AI‑driven humanoid robots and signalling Apple&\#x27;s entry into this research area.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/apple-aiml-research/ml-halo">GitHub - apple-aiml-research/ml-halo: HALO: Perceptive ...</a></li>
<li><a href="https://arxiv.org/html/2611.06908">Perceptive Humanoid Motion from Simulation - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#large-language-models`, `#reinforcement-learning`, `#Apple`

---

<a id="item-tech-news-14"></a>
### [Democratic Lawmaker Calls for Ban on AI Recursive Self‑Improvement](https://x.com/AlexBores/status/2118494668769878037) ⭐️ 7.0/10

U.S. Democratic Representative Alex Bores urged Congress to pass legislation this year prohibiting AI recursive self‑improvement \(RSI\), where AI systems autonomously create next‑generation AI. He cited accelerating AI research—OpenAI’s plan for an automated AI researcher by March 2028 and Anthropic’s forecast that AI could handle about 80% of frontier model development by the end of 2027—as evidence that the risk of error or alignment drift could compound across generations, prompting an immediate ban request.

telegram · zaihuapd · Nov 8, 01:30

**「Prerequisite: AI automation milestones」** Recursive self‑improvement \(RSI\) is the notion that an AI system can autonomously design and build a more capable successor, potentially accelerating its own capabilities across generations. OpenAI has publicly pledged to deploy an “automated AI researcher” that can conduct research alongside humans by March 2028, and Anthropic projects that its Claude system will perform roughly 80 % of frontier model development by the end of 2027. These industry timelines indicate that the technical conditions for RSI are expected to emerge soon, giving context to the congressional call for a ban.

**「Impact」** If such a ban were enacted, AI developers would need to halt or redesign projects that enable AI systems to independently generate or improve subsequent AI models, potentially limiting research on automated model‑generation tools and requiring compliance checks for RSI capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/built-to-benefit-everyone-our-plan/">Built to benefit everyone: our plan - OpenAI</a></li>
<li><a href="https://cryptobriefing.com/anthropic-claude-lead-frontier-model-training-2027/">Anthropic projects Claude will lead 80-90% of frontier model ...</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#AI safety`, `#Legislation`, `#Recursive self‑improvement`

---

## Financial News

<a id="item-finance-news-1"></a>
### [SoftBank, ABB consider carving out China robotics unit to rescue $5.4 billion deal](https://www.bloomberg.com/news/articles/2026-11-07/softbank-abb-weigh-china-carve-out-to-salvage-robotics-deal) ⭐️ 8.0/10

SoftBank and ABB are weighing a carve‑out of ABB’s China robotics business to revive a $5.4 billion acquisition that Chinese regulators halted.

telegram · zaihuapd · Nov 7, 11:24

**「Background」** Earlier this week, Chinese regulators halted SoftBank’s $5.4 billion plan to acquire ABB’s robotics division, citing a foreign‑investment security review.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/business/media-telecom/softbank-abb-explore-china-carve-out-salvage-robotics-deal-bloomberg-news-2026-11-07/">SoftBank, ABB explore China carve-out to salvage robotics ...</a></li>

</ul>
</details>

**Tags**: `#Mergers &amp; Acquisitions`, `#Robotics`, `#China Policy`, `#SoftBank`, `#ABB`

---