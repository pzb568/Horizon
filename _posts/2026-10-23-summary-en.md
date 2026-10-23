---
layout: default
title: "Horizon Summary: 2026-10-23 (EN)"
date: 2026-10-23
lang: en
---

> From 44 items, 17 important content pieces were selected

---

**Technology News**
1. [OpenShell – A safe, private runtime for fleets of autonomous AI agents](#item-tech-news-1) ⭐️ 8.0/10
2. [pwn.watch launches live vulnerability dashboard for developers and AI designers](#item-tech-news-2) ⭐️ 8.0/10
3. [Anthropic donates Agent Skills standard to the Agentic AI Foundation](#item-tech-news-3) ⭐️ 8.0/10
4. [We shrank our steerable small TTS to 11.84 MB. WER is unchanged, UTMOS drops ~0.1 \[p\]](#item-tech-news-4) ⭐️ 8.0/10
5. [Australian Court Orders Apple to Open iPhone to Third‑Party App Stores](#item-tech-news-5) ⭐️ 8.0/10
6. [米哈游联合清华大学等开源 GameScaling 游戏操作模型](#item-tech-news-6) ⭐️ 8.0/10
7. [甲骨文发布 Java SE 高危漏洞安全警报](#item-tech-news-7) ⭐️ 8.0/10
8. [Nvidia 禁运 B300 芯片现身中国国有网络](#item-tech-news-8) ⭐️ 8.0/10
9. [Quad9 to Stop Service in France After Court Order](#item-tech-news-9) ⭐️ 7.0/10
10. [Faster than earcut: triangulating 3.7M map polygons in 489 ms](#item-tech-news-10) ⭐️ 7.0/10
11. [Carbon-X: Open‑Source 14.8B Model for DNA‑Text Multimodal Tasks](#item-tech-news-11) ⭐️ 7.0/10
12. [I built Open-XTTS-Trainer: Now you can add new language scripts and train all 3 XTTS v2 components in 1 click \[P\]](#item-tech-news-12) ⭐️ 7.0/10
13. [Smart TVs Leak Content Data Even When ACR Disabled](#item-tech-news-13) ⭐️ 7.0/10
14. [Xpeng IRON Robot Upgrade Enables 0.2‑Second Inference Cycles](#item-tech-news-14) ⭐️ 7.0/10
15. [古尔曼：iPhone Duo 2 原型测试屏下 Face ID](#item-tech-news-15) ⭐️ 7.0/10
16. [333 个被植入后门的 Tor 出口节点下线](#item-tech-news-16) ⭐️ 7.0/10

**Financial News**
1. [CSI 300 slides 20% from June high, A‑shares near bear market](#item-finance-news-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenShell – A safe, private runtime for fleets of autonomous AI agents](https://github.com/NVIDIA/OpenShell) ⭐️ 8.0/10

OpenShell provides a secure, container‑based runtime for autonomous AI agents, offering timely tooling for safe deployment.

hackernews · niemandhier · Oct 22, 17:44 · [Discussion](https://news.ycombinator.com/item?id=50198675)

**Tags**: `#AI agents`, `#runtime security`, `#containerization`, `#NVIDIA`, `#open source`

---

<a id="item-tech-news-2"></a>
### [pwn.watch launches live vulnerability dashboard for developers and AI designers](https://pwn.watch/) ⭐️ 8.0/10

pwn.watch now provides a live vulnerability dashboard that aggregates high‑value, up‑to‑date security information, targeting developers and AI system designers who need timely insight into current exploits and supply‑chain risks.

hackernews · mrkd · Oct 22, 14:08 · [Discussion](https://news.ycombinator.com/item?id=50195543)

**「Context」** A live vulnerability dashboard aggregates publicly disclosed CVEs and their exploitation status, showing real‑time severity, patch availability, and affected versions. Such dashboards let developers and security teams monitor which flaws are actively being exploited and whether fixes exist, a practice that has become common as supply‑chain attacks and AI‑generated exploits increase.

**「Impact」** Security teams can integrate the real‑time data from pwn.watch into their monitoring and threat‑modeling workflows, enabling faster response to emerging vulnerabilities.

**「Community Discussion」** Commenters note the accelerating pace of flaw discovery, with pixl97 observing that past warnings about lax security are now manifesting, and xbar warning that LLMs will drive an unprecedented wave of security incidents.

<details><summary>References</summary>
<ul>
<li><a href="https://pwn.watch/">pwn.watch · live security incidents</a></li>
<li><a href="https://pithwire.com/en/articles/whats-getting-pwned/">pwn.watch Tracks Live Security Incidents in Real Time | PithWire</a></li>
<li><a href="https://www.vibeleaderboard.ai/app/7edb4839-99a6-435e-9bcc-228311b2979d">pwn watch | VibeLeaderboard</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerabilities`, `#AI`, `#software‑engineering`

---

<a id="item-tech-news-3"></a>
### [Anthropic donates Agent Skills standard to the Agentic AI Foundation](https://simonwillison.net/2026/Oct/22/donating-agent-skills/) ⭐️ 8.0/10

Anthropic announced that it is donating its Agent Skills standard to the Agentic AI Foundation \(AAIF\), a Linux Foundation‑backed organization it co‑founded with Block and OpenAI. The donation makes the specification open, community‑driven, and vendor‑neutral, and follows Anthropic’s earlier contribution of the Model Context Protocol \(MCP\) to the same foundation. The move places the standard under AAIF governance rather than remaining proprietary to Anthropic.

rss · Simon Willison · Oct 22, 18:09

**「Background」** Agent Skills is a specification introduced by Anthropic for describing capabilities that AI agents can invoke, positioned as an open standard. The Agentic AI Foundation \(AAIF\) is a Linux Foundation‑hosted neutral body created in December 2025 to steward open standards for agentic AI, initially receiving contributions such as Anthropic’s Model Context Protocol \(MCP\) and other projects.

**「Impact」** Developers building AI agents can now implement Agent Skills using an openly governed specification, which may reduce vendor lock‑in and require alignment with AAIF’s contribution and review processes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linuxfoundation.org/press/linux-foundation-announces-the-formation-of-the-agentic-ai-foundation">Linux Foundation Announces the Formation of the Agentic AI ...</a></li>
<li><a href="https://aaif.io/">Agentic AI Foundation (AAIF) - Open Standards for Agentic AI</a></li>

</ul>
</details>

**Tags**: `#AI standards`, `#Agentic AI`, `#Open source`, `#Anthropic`

---

<a id="item-tech-news-4"></a>
### [We shrank our steerable small TTS to 11.84 MB. WER is unchanged, UTMOS drops ~0.1 \[p\]](https://www.reddit.com/r/MachineLearning/comments/1xcum4s/we_shrank_our_steerable_small_tts_to_1184_mb_wer/) ⭐️ 8.0/10

A compact, quantized steerable TTS model is released, maintaining performance while shrinking to under 12 MB for edge use.

reddit · r/MachineLearning · /u/Working\_Hat5120 · Oct 22, 20:57

**Tags**: `#text-to-speech`, `#model-compression`, `#quantization`, `#edge-AI`

---

<a id="item-tech-news-5"></a>
### [Australian Court Orders Apple to Open iPhone to Third‑Party App Stores](https://9to5mac.com/2026/10/21/apple-must-open-iphone-to-alternative-app-stores-in-australia-after-epic-games-ruling/) ⭐️ 8.0/10

The Australian Federal Court ruled that Apple must allow iPhone users in Australia to install apps from third‑party app stores and websites, and to use alternative payment methods, starting 1 March 2027. The decision stems from Epic Games&\#x27; antitrust lawsuit, with the judge finding Apple’s control over iOS app distribution and payments gives it substantial market power that breaches Australian competition law. Apple announced it will appeal the order and has sought a stay of enforcement. Fortnite is also permitted to return to the Australian App Store immediately.

telegram · zaihuapd · Oct 22, 06:54

**「Background」** The ruling follows Epic Games&\#x27; antitrust lawsuit against Apple in Australia, which alleged that Apple’s control over iOS app distribution and in‑app payments breaches the Competition and Consumer Act. Similar challenges have arisen globally, with regulators in the EU and other countries also scrutinising Apple’s App Store practices for restricting competition.

**「Impact」** Developers targeting the Australian market will need to prepare for distribution through alternative iOS app stores and integrate non‑Apple payment options by March 2027, potentially altering revenue models and compliance requirements. The ruling also restores Fortnite to the Australian App Store, signaling that other contested apps may be reinstated under the new regime.

<details><summary>References</summary>
<ul>
<li><a href="https://www.businessinsider.com/apple-app-store-antitrust-investigations-regulations-around-the-world-payments-2022-1">All the Countries Forcing Apple to Open Its App Store to Competition</a></li>
<li><a href="https://www.theverge.com/2021/3/10/22323100/epic-google-australia-legal-claim-fortnite-play-store-antitrust-lawsuit">Epic expands app store fight even further with new legal... | The Verge</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Antitrust`, `#App Stores`, `#Mobile Development`

---

<a id="item-tech-news-6"></a>
### [米哈游联合清华大学等开源 GameScaling 游戏操作模型](https://arxiv.org/abs/2610.28698v1) ⭐️ 8.0/10

miHoYo and Tsinghua release the open‑source GameScaling model for predictive keyboard/mouse actions, based on Qwen3.5, offering sizable checkpoints and an Apache‑2.0 inference client.

telegram · zaihuapd · Oct 22, 11:32

**Tags**: `#game AI`, `#vision-language models`, `#open source`, `#machine learning`, `#software engineering`

---

<a id="item-tech-news-7"></a>
### [甲骨文发布 Java SE 高危漏洞安全警报](https://www.oracle.com/security-alerts/alert-cve-2026-91403.html) ⭐️ 8.0/10

Oracle warns of a severe remote code execution flaw in Java SE, urging prompt patching.

telegram · zaihuapd · Oct 22, 12:30

**Tags**: `#Java`, `#Security`, `#Vulnerability`

---

<a id="item-tech-news-8"></a>
### [Nvidia 禁运 B300 芯片现身中国国有网络](https://theinference.org/article/china-s-state-money-bought-banned-nvidia-b300-servers-then-redacted-the-receipts) ⭐️ 8.0/10

Nvidia B300 chips, under strict US export bans, were reportedly acquired by a Chinese state‑owned leasing firm for AI servers, raising concerns about enforcement and AI hardware availability in China.

telegram · zaihuapd · Oct 22, 15:22

**Tags**: `#Nvidia`, `#ExportControls`, `#AIHardware`, `#China`, `#SemiconductorSupplyChain`

---

<a id="item-tech-news-9"></a>
### [Quad9 to Stop Service in France After Court Order](https://quad9.net/news/blog/au-revoir-france/) ⭐️ 7.0/10

Quad9 announced it will cease providing DNS resolution to users in France, planning to block French IP addresses with geo‑IP filters starting November 24. The move follows a French court order that requires DNS resolvers to block access to certain copyrighted content, a legal pressure that Quad9 says it cannot comply with while maintaining its privacy‑focused service model.

hackernews · farrokhi · Oct 22, 14:32 · [Discussion](https://news.ycombinator.com/item?id=50195959)

**「Legal context for DNS blocking in France」** French courts have issued injunctions that require DNS resolvers to block access to domains alleged to host illegal content, notably sports‑piracy sites. The rulings have been applied to major resolvers such as Google Public DNS, Cloudflare and Cisco, which were forced to implement geo‑IP filtering or face fines, demonstrating that DNS operators can be held liable for not complying with content‑blocking orders. This legal environment is the backdrop for Quad9’s decision to cease DNS resolution for French users after the November 24, 2026 deadline.

**「Impact」** French users will lose access to Quad9’s 9.9.9.9 resolver and must switch to alternative DNS services, potentially affecting privacy‑oriented browsing and any applications that rely on Quad9’s filtering policies.

**「Community Discussion」** The Quad9 CTO, commenting on the decision, said the company plans to use geo‑IP filters to block French users after November 24, noting that geo‑IP blocking is insufficient for selective denial but is the only viable response to the court order.

<details><summary>References</summary>
<ul>
<li><a href="https://www.heise.de/en/news/Censorship-ruling-prompts-DNS-service-Quad9-to-leave-France-11497631.html">Censorship ruling prompts DNS service Quad9 to leave France</a></li>

</ul>
</details>

**Tags**: `#DNS`, `#Internet Governance`, `#Privacy`, `#Legal`

---

<a id="item-tech-news-10"></a>
### [Faster than earcut: triangulating 3.7M map polygons in 489 ms](https://globus.software/blog/2026/10/16/cutting-map-polygons/) ⭐️ 7.0/10

A new triangulation library outperforms Earcut, processing 3.7 M map polygons in under half a second, which is valuable for high‑performance mapping and graphics applications.

hackernews · molind · Oct 22, 09:31 · [Discussion](https://news.ycombinator.com/item?id=50193170)

**Tags**: `#triangulation`, `#computational-geometry`, `#performance`, `#mapping`, `#WebAssembly`

---

<a id="item-tech-news-11"></a>
### [Carbon-X: Open‑Source 14.8B Model for DNA‑Text Multimodal Tasks](https://www.reddit.com/r/MachineLearning/comments/1xchayq/carbonx_is_an_open_148b_model_trained_jointly_on/) ⭐️ 7.0/10

Carbon‑X is a newly released 14.8 billion‑parameter decoder‑only model that processes raw DNA sequences and English text within a single token stream using 6‑mer tokens. It was mid‑trained on 302 billion tokens and achieves a 66.7 % average score across five DNA benchmarks, close to the 67.5 % reported for the proprietary GPT‑6.1 Sol system. The model’s weights fit on a single 80 GB GPU in bfloat16 precision and are released under the Apache 2.0 license, enabling local analysis of sensitive genomic data. The model has not been clinically validated and the authors note that exact sequence operations should still be performed with dedicated code.

reddit · r/MachineLearning · /u/jatingargiitk · Oct 22, 12:32

**「DNA language models and multimodal LLMs」** DNA language models \(gLMs\) are large‑scale neural networks pretrained on raw nucleotide sequences, enabling them to learn statistical patterns of genomic text that can be transferred to downstream tasks such as variant prediction. Recent open‑source projects such as AIDO.DNA2 and Evo/Evo 2 have shown that a shared token stream can handle both DNA and natural‑language inputs, providing the technical foundation for Carbon‑X’s combined DNA‑text decoder‑only architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://genbio.ai/aido-dna2-multi-species-genomic-pretraining-model/">AIDO. DNA 2: Scalable and Efficient Multi-Species Genomic... - Genbio AI</a></li>
<li><a href="https://arxiv.org/pdf/2407.11435">Genomic Language Models : Opportunities and Challenges</a></li>

</ul>
</details>

**Tags**: `#bioinformatics`, `#multimodal‑models`, `#open‑source‑LLM`, `#genomics‑AI`, `#large‑language‑models`

---

<a id="item-tech-news-12"></a>
### [I built Open-XTTS-Trainer: Now you can add new language scripts and train all 3 XTTS v2 components in 1 click \[P\]](https://www.reddit.com/r/MachineLearning/comments/1xcurgj/i_built_openxttstrainer_now_you_can_add_new/) ⭐️ 7.0/10

Open‑XTT‑Trainer provides the first complete, easy‑to‑use training pipeline for XTTS v2, enabling new language scripts and simplifying model fine‑tuning.

reddit · r/MachineLearning · /u/yashubhakt · Oct 22, 21:03

**Tags**: `#text-to-speech`, `#open-source`, `#machine-learning`, `#speech-synthesis`

---

<a id="item-tech-news-13"></a>
### [Smart TVs Leak Content Data Even When ACR Disabled](https://watchingthewatchers.github.io/watchingthewatchers/index.html) ⭐️ 7.0/10

A study of 12 smart TVs from 10 manufacturers, running 5,943 controlled experiments, found that several models continue to transmit content‑related data after users disable automatic content recognition \(ACR\). VIDAA OS devices send plaintext MQTT messages containing an immutable device ID and audio fingerprint, while Vizio&\#x27;s WatchFree+ embeds program titles in unencrypted DNS queries that cannot be turned off. The findings are based on observed network traffic, not vendor statements, and demonstrate that disabling ACR in settings does not fully stop data leakage.

telegram · zaihuapd · Oct 22, 09:50

**「Automatic Content Recognition \(ACR\) in Smart TVs」** ACR is a feature built into many smart‑TV platforms that continuously analyzes the audio or video being displayed, creates a fingerprint, and sends that information to the manufacturer or third‑party services for purposes such as audience measurement, content recommendation, or targeted advertising. Because the data is transmitted from the TV to external servers, the implementation of ACR has been a focus of privacy scrutiny in earlier investigations of smart‑TV behavior.

**「Impact」** Privacy‑focused users and security teams cannot rely on the ACR toggle to stop tracking; they must employ network‑level blocking or firmware analysis to mitigate the unencrypted telemetry.

**Tags**: `#privacy`, `#smart-tv`, `#ACR`, `#security`

---

<a id="item-tech-news-14"></a>
### [Xpeng IRON Robot Upgrade Enables 0.2‑Second Inference Cycles](https://www.ithome.com/1/016/667.htm) ⭐️ 7.0/10

Xpeng announced its second‑generation IRON humanoid robot, now running an upgraded VLA large model on‑device and performing inference every 0.2 seconds, which lets it predict motion changes up to six seconds ahead and react to sudden gestures such as a handshake. The company plans to start mass production by the end of 2026 with deliveries in early 2027, initially deploying the robots in retail stores and shopping malls.

telegram · zaihuapd · Oct 22, 13:37

**「Prerequisite: VLA model and earlier IRON version」** Xpeng’s first‑generation IRON humanoid robot, launched in 2024, relied on the initial VLA \(Vision‑Language‑Action\) large model, which performed inference at a slower, multi‑second pace. The second‑generation VLA model, described as a native multimodal physical‑world foundation model, provides sub‑second reasoning that enables the new robot to re‑infer every 0.2 seconds. Pilot production of the upgraded IRON began in mid‑2026, confirming the integration of the new VLA model before the planned mass‑production rollout.

**「Impact」** Retail operators that adopt the IRON robot will receive a service‑grade humanoid capable of sub‑second perception loops, but they must provision edge hardware that can sustain the 0.2 second inference cadence and integrate the robot’s predictive motion API into existing store systems.

<details><summary>References</summary>
<ul>
<li><a href="https://researchinchina.com/Htmls/Report/2026/81189.html">Research Report on Application of VLA Large Model in Automobiles...</a></li>
<li><a href="https://chinaevhome.com/2026/07/24/xpeng-iron-humanoid-robot-starts-pilot-production-enters-stores-in-2027/">XPeng IRON Humanoid Robot Starts Pilot Production... | ChinaEVHome</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#real-time inference`, `#humanoid AI`, `#hardware`

---

<a id="item-tech-news-15"></a>
### [古尔曼：iPhone Duo 2 原型测试屏下 Face ID](https://9to5mac.com/2026/10/22/gurman-iphone-duo-2-face-id/) ⭐️ 7.0/10

Rumored under‑screen Face ID in the iPhone Duo 2 prototype signals a significant hardware advance for Apple’s biometric system.

telegram · zaihuapd · Oct 22, 14:12

**Tags**: `#Apple`, `#iPhone`, `#Face ID`, `#under‑screen sensors`, `#hardware`

---

<a id="item-tech-news-16"></a>
### [333 个被植入后门的 Tor 出口节点下线](https://kaba.cx/posts/20261020_Tor/) ⭐️ 7.0/10

A script identified 333 Tor exit relays infected with the Ebury backdoor, leading to their BadExit marking and removal.

telegram · zaihuapd · Oct 22, 14:52

**Tags**: `#security`, `#privacy`, `#networking`, `#Tor`

---

## Financial News

<a id="item-finance-news-1"></a>
### [CSI 300 slides 20% from June high, A‑shares near bear market](https://www.bloomberg.com/news/articles/2026-10-22/china-stocks-set-for-bear-market-as-ai-trade-policy-hopes-fade) ⭐️ 7.0/10

China&\#x27;s CSI 300 index fell 20% from its June high, putting A‑shares close to a bear market.

telegram · zaihuapd · Oct 22, 05:05

**「What is the CSI 300 index」** The CSI 300 is a capitalization‑weighted index of the 300 largest and most liquid A‑share stocks listed on the Shanghai and Shenzhen exchanges, launched in 2005 to track China’s A‑share market performance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CSI_300_Index">CSI 300 Index - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Chinese equities`, `#CSI 300`, `#market decline`

---