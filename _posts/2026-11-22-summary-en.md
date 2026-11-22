---
layout: default
title: "Horizon Summary: 2026-11-22 (EN)"
date: 2026-11-22
lang: en
---

> From 24 items, 5 important content pieces were selected

---

**Technology News**
1. [GPGME double‑free vulnerability affecting versions before 2.3.0](#item-tech-news-1) ⭐️ 8.0/10
2. [Tesla begins rolling out FSD v15 with safety boost and visual overlay](#item-tech-news-2) ⭐️ 8.0/10
3. [OpenRouter warns MiniMax prompts may have been read by third parties](#item-tech-news-3) ⭐️ 7.0/10
4. [Google Gemini adds separate control to disable training data retention](#item-tech-news-4) ⭐️ 7.0/10

**Technology Blog**
1. [Avoiding Catastrophic Mistakes in Large Codebases](#item-tech-blog-1) ⭐️ 4.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [GPGME double‑free vulnerability affecting versions before 2.3.0](https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html) ⭐️ 8.0/10

A double‑free bug in the GPGME library \(versions &lt; 2.3.0\) has been disclosed, which could be chained into remote code execution. The flaw impacts any software that links against the vulnerable GPGME, including GitLab, Gpg4win, GnuPG Desktop, many mail and XMPP clients, and Samba. Patches are already available from Red Hat and GitLab, but upstream GPGME has not yet released an official fix.

hackernews · gdgghhhhh · Nov 21, 08:32 · [Discussion](https://news.ycombinator.com/item?id=50587208)

**「What is GPGME and the double‑free flaw」** GPGME \(GnuPG Made Easy\) is the official library that applications use to interact with GnuPG for OpenPGP operations such as signature verification and encryption. The disclosed vulnerability is a double‑free memory error that can be triggered by an OpenPGP key containing an unusually long user ID, potentially allowing data exfiltration or remote‑code execution when the malformed key is processed. This flaw affects any software that links against GPGME versions prior to 2.3.0, including Gpg4win, GnuPG Desktop, mail and XMPP clients, Samba, and others.

**「Impact」** Projects that embed GPGME must upgrade to version 2.3.0 or apply the vendor patches \(e.g., Red Hat’s backport, GitLab’s Omnibus update\) to avoid potential code execution attacks.

**「Community discussion」** Commenters note that the issue is a double‑free rather than a direct RCE chain, suggesting the severity may be overstated, while others point out that Red Hat patched the bug five years ago but upstream missed it. A list of affected applications was also provided, confirming the wide reach of the vulnerability.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/11/gnupg-warns-critical-gpgme-flaw-could.html">GnuPG Warns Critical GPGME Flaw Could Expose App Data via...</a></li>
<li><a href="https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html">[Announce] GnuPG Security Advisory for GPGME ...</a></li>
<li><a href="https://www.openwall.com/lists/oss-security/2026/11/20/13">oss-security - Fwd: GnuPG Security Advisory for GPGME ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#open-source`, `#devops`, `#cryptography`

---

<a id="item-tech-news-2"></a>
### [Tesla begins rolling out FSD v15 with safety boost and visual overlay](https://x.com/Tesla/status/2124222447855743019) ⭐️ 8.0/10

Tesla started an over‑the‑air rollout of Full Self‑Driving version 15 \(FSD v15\) to overseas vehicles. The update claims a 25‑fold increase in handling of safety‑critical scenarios and introduces a new &quot;Tesla Reality View&quot; visual overlay that can display camera feed and planned path on the infotainment screen in full‑screen, map or split‑view modes, with a quiet mode option. Navigation now layers turn‑by‑turn cues on the overlay, turn‑signal sounds are softened and fade, and the software adds optimizations for potholes, debris, school zones and speed control in adverse weather.

telegram · zaihuapd · Nov 22, 00:03

**「What is Tesla Full Self-Driving \(FSD\)」** Tesla’s Full Self‑Driving \(FSD\) suite is the company’s beta‑level driver‑assist system that runs on an on‑board neural‑network stack and has been released in incremental versions, most recently v14, which provided basic lane‑keeping, navigation‑on‑autopilot and limited city‑street capabilities. Each version expands the end‑to‑end perception and planning models, and prior rollouts have been used to gather fleet data for safety improvements.

**「Impact」** Owners whose cars receive the OTA update will gain the enhanced safety handling and the new UI, potentially improving driver awareness and reducing incidents in challenging conditions. Users should ensure their vehicle firmware is updated to v15 to access these features.

<details><summary>References</summary>
<ul>
<li><a href="https://electrek.co/2026/11/21/tesla-fsd-v15-rollout-25x-safety-reality-view/">Tesla launches FSD v15, targets its biggest weaknesses, from ...</a></li>

</ul>
</details>

**Tags**: `#autonomous driving`, `#AI`, `#software engineering`, `#Tesla`

---

<a id="item-tech-news-3"></a>
### [OpenRouter warns MiniMax prompts may have been read by third parties](https://news.ycombinator.com/item?id=50585962) ⭐️ 7.0/10

OpenRouter has warned that prompts sent to MiniMax models between July and October 2026 may have been accessed by an unauthorised third party. Security researchers observed that URLs embedded in test prompts were visited 40 to 130 hours after submission, indicating the data was read downstream. OpenRouter attributes the issue to MiniMax and its forwarding partners AtlasCloud, Novita, and StreamLake, and has removed the &quot;zero data retention&quot; label from the affected endpoints. Users with sensitive credentials are advised to rotate API keys and passwords immediately.

telegram · zaihuapd · Nov 21, 06:53

**「Background」** OpenRouter is a routing platform that forwards API calls to various large‑language‑model providers, including MiniMax, a Chinese‑based LLM service. MiniMax endpoints were advertised with a “Zero Data Retention” \(ZDR\) label, meaning OpenRouter claimed that prompts would not be stored or logged. The incident arose because a security researcher embedded unique test URLs in prompts sent to MiniMax between July and October 2026; a third party later accessed those URLs 40–130 hours after the requests, indicating the prompts were readable downstream. This exposure prompted OpenRouter to remove the ZDR badge from the affected endpoints and advise users to rotate API keys and passwords.

**「Impact」** Developers using MiniMax via OpenRouter should replace any exposed API keys or passwords and review their data‑handling practices to mitigate potential credential leakage.

<details><summary>References</summary>
<ul>
<li><a href="https://explainx.ai/blog/openrouter-minimax-prompts-may-have-been-read-customer-email-november-2026">OpenRouter MiniMax Leak Email: What to Do (Nov 2026 ...</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#LLM APIs`, `#data privacy`

---

<a id="item-tech-news-4"></a>
### [Google Gemini adds separate control to disable training data retention](https://blog.google/innovation-and-ai/products/gemini-app/updated-controls/) ⭐️ 7.0/10

Google Gemini will introduce two new settings in the coming weeks that replace the existing &quot;retain activity history&quot; toggle. One setting lets users choose how long their conversation history is kept, and the other lets them disable the use of dialogue content—including text and attachments—for training generative AI models while still preserving the history. When history is turned off, conversations are kept for about two months for moderation, feedback, and safety purposes, and audio recordings remain excluded from model improvement.

telegram · zaihuapd · Nov 22, 01:24

**「Prerequisite: Gemini’s prior data‑retention model」** Google Gemini is Google’s consumer‑facing generative AI service that stores user conversations in a &quot;retain activity history&quot; setting, which historically controlled both how long chat logs were kept and whether the content could be used to train future model versions. The new controls replace that single toggle with separate options, allowing users to keep their chat history while opting out of training‑data collection.

**「Impact」** Users can now opt out of having their Gemini interactions used to train future models without losing access to their saved conversation history, giving them finer privacy control and reducing the amount of personal data that contributes to model updates.

**Tags**: `#Google Gemini`, `#AI privacy`, `#model training data`, `#product update`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Avoiding Catastrophic Mistakes in Large Codebases](https://seangoedecke.com/to-code-well-avoid-blunders/) ⭐️ 4.0/10

rss · Sean Goedecke · Nov 22, 00:00

**「Background」** The author argues that in large commercial codebases a single inconsistency or unnecessary requirement can degrade an otherwise clean system, making blunders the primary source of technical debt.

**「Solution」** To mitigate this risk, the article advises developers to treat consistency and requirement minimalism as the core objectives of every change. It recommends spotting where a new task naturally belongs in the existing architecture, then stripping it down to the smallest viable set of requirements before implementation. The author warns against introducing parallel implementations, duplicate sources of truth, or converting safe synchronous operations into fragile asynchronous ones, as these create hidden failure points. By keeping the focus on “not blundering” rather than on clever patterns or extra features, engineers can preserve trust in the codebase and avoid the combinatorial explosion of inter‑dependent requirements. Although the piece offers concrete examples of typical blunders, it stops short of providing detailed processes or tooling guidance, positioning the advice as a high‑level mindset shift for teams working on big, shared codebases.

**「Takeaway」** The article’s central claim is that reliable software stems more from rigorously avoiding consistency errors and superfluous requirements than from pursuing clever abstractions.

**Tags**: `#software engineering`, `#code quality`, `#technical debt`

---