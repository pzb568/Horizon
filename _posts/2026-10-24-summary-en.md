---
layout: default
title: "Horizon Summary: 2026-10-24 (EN)"
date: 2026-10-24
lang: en
---

> From 33 items, 8 important content pieces were selected

---

**Technology News**
1. [Amazon’s Trainium Takes a Strike at the Training King](#item-tech-news-1) ⭐️ 8.0/10
2. [微软悄悄测试 Win11 不同于 Recall 的 AI 记忆应用 Pantheon](#item-tech-news-2) ⭐️ 8.0/10
3. [PHP Foundation Recommends Disabling Upload Progress Feature](#item-tech-news-3) ⭐️ 8.0/10
4. [🤖 KIMI K3.1-Pro 模型正式发布](#item-tech-news-4) ⭐️ 8.0/10
5. [New iPhone Hack Demonstrated, Details Sparse](#item-tech-news-5) ⭐️ 7.0/10
6. [Dessa: the most authentic full-duplex speech model ever built](#item-tech-news-6) ⭐️ 7.0/10
7. [Swedish Government Office Bans ChatGPT and Claude, Requires Approved AI Tools](#item-tech-news-7) ⭐️ 7.0/10

**Financial News**
1. [EU lifts 84.2% tariff on Chinese solar glass](#item-finance-news-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Amazon’s Trainium Takes a Strike at the Training King](https://newsletter.semianalysis.com/p/amazons-trainium-takes-a-strike-at) ⭐️ 8.0/10

Amazon enhances Trainium with native PyTorch training, improving its appeal for ML research and production.

rss · Semianalysis · Oct 23, 19:06

**Tags**: `#AWS Trainium`, `#Machine Learning Hardware`, `#PyTorch`, `#AI Infrastructure`

---

<a id="item-tech-news-2"></a>
### [微软悄悄测试 Win11 不同于 Recall 的 AI 记忆应用 Pantheon](https://www.windowslatest.com/2026/10/23/microsoft-is-quietly-testing-another-recall-for-windows-11-but-this-one-doesnt-record-your-screen/) ⭐️ 8.0/10

Microsoft is testing Project Pantheon, an AI memory app for Windows 11 that stores selected user content for AI queries.

telegram · zaihuapd · Oct 23, 07:42

**Tags**: `#Windows`, `#AI`, `#Productivity`, `#Operating Systems`, `#Microsoft`

---

<a id="item-tech-news-3"></a>
### [PHP Foundation Recommends Disabling Upload Progress Feature](https://x.com/ThePHPF/status/2113580383875019242) ⭐️ 8.0/10

The PHP Foundation advises users to set session.upload\_progress.enabled=0 before the next PHP release to mitigate a critical remote code execution vulnerability identified as CVE‑2026‑115560. The advisory notes that only applications that switch the serialize\_handler to &quot;php&quot; at runtime are potentially affected. The foundation previously recommended keeping this feature disabled for the earlier CVE‑2026‑109619 issue.

telegram · zaihuapd · Oct 23, 13:46

**「Prerequisite: PHP upload‑progress mechanism」** PHP’s upload‑progress feature records file‑upload status in the session using the session.upload\_progress.enabled setting and a serialize\_handler that must be set to the default “php”. A mismatch in the serialize\_handler can allow crafted data to be deserialized, leading to remote code execution, which is the basis of CVE‑2026‑115560. The PHP Foundation has previously issued a similar advisory for CVE‑2026‑109619, also recommending the feature be disabled until a fix is released.

**「Impact」** Web administrators should update their php.ini or equivalent configuration to disable upload‑progress tracking immediately, reducing the attack surface for the RCE flaw until a patched PHP version is released.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/php-shares-mitigation-for-new-and-unpatched-rce-vulnerability/">PHP shares mitigation for new RCE vulnerability with no patch</a></li>
<li><a href="https://help.nextcloud.com/t/new-php-vulnerability-cve-2026-115560-in-community-docker-image/251425">New PHP vulnerability CVE - 2026 - 115560 in community docker image</a></li>

</ul>
</details>

**Tags**: `#php`, `#security`, `#vulnerability`

---

<a id="item-tech-news-4"></a>
### [🤖 KIMI K3.1-Pro 模型正式发布](https://www.kimi.ai/blog/kimi-k3-1-pro) ⭐️ 8.0/10

KIMI releases its 30‑trillion‑parameter K3.1‑Pro model, promising stronger coding, 3D, and finance capabilities with extended context length.

telegram · zaihuapd · Oct 23, 17:14

**Tags**: `#large-language-model`, `#software-engineering`, `#AI-tools`, `#3D-generation`

---

<a id="item-tech-news-5"></a>
### [New iPhone Hack Demonstrated, Details Sparse](https://blog.calif.io/p/iphone) ⭐️ 7.0/10

A blog post published on October 23, 2026 describes a newly demonstrated hack that grants privileged access to current iPhone models, effectively bypassing Apple’s security mechanisms. The write‑up provides security‑focused engineers with practical insights but does not disclose enough technical specifics to determine whether the exploit represents a fundamentally new attack vector or a variation of existing jailbreak techniques.

hackernews · pavel\_lishin · Oct 23, 16:21 · [Discussion](https://news.ycombinator.com/item?id=50211474)

**「Prerequisite context」** The hack builds on Calif’s earlier public demos of iOS exploits, notably the untethered jailbreak for iOS 27.0.1 shown at Hexacon in Paris on Oct 16 2026 and a prior zero‑click worm that spread via WeChat calls across iOS and Android \(Sept 11 2026\). These prior demonstrations established that Calif can achieve kernel‑level code execution without user interaction, setting the stage for the new iPhone exploit.

**「Community Discussion」** Commenters expressed concern that such jailbreaks can be detected by Apple, potentially locking users out of iCloud and iMessage services, and asked whether iOS Lockdown mode offers any real protection against the demonstrated exploits.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.calif.io/p/iphone">iPhone - Calif Newsletter</a></li>
<li><a href="https://blog.calif.io/archive">Archive - Calif Newsletter</a></li>
<li><a href="https://github.com/iMaxTomas/ios27-jb-tracker">GitHub - iMaxTomas/ios27-jb-tracker: iOS 27.0.1 越狱事件（Calif ....</a></li>

</ul>
</details>

**Tags**: `#security`, `#iOS`, `#jailbreak`, `#hardware`

---

<a id="item-tech-news-6"></a>
### [Dessa: the most authentic full-duplex speech model ever built](https://block.xyz/dessa) ⭐️ 7.0/10

Dessa introduces an impressive low‑data, locally‑run full‑duplex speech model, offering high‑value insight for AI and software engineers.

hackernews · dsr12 · Oct 23, 19:09 · [Discussion](https://news.ycombinator.com/item?id=50213925)

**Tags**: `#speech-synthesis`, `#full-duplex`, `#local-inference`, `#low-data-training`

---

<a id="item-tech-news-7"></a>
### [Swedish Government Office Bans ChatGPT and Claude, Requires Approved AI Tools](https://www.sverigesradio.se/artikel/chat-gpt-och-claude-forbjuder-regeringskansliet) ⭐️ 7.0/10

Starting next week, Sweden’s Government Office \(Regeringskansliet\) will block access to ChatGPT and Claude on all employee work computers. The ban is enforced because uncontracted AI services are deemed a security risk, and staff are required to use only approved AI tools such as Microsoft Copilot. The office had previously restricted the use of DeepSeek, extending its policy to additional generative AI services.

telegram · zaihuapd · Oct 23, 14:11

**「Prior AI restrictions in Swedish public sector」** Swedish authorities have already limited the use of external AI services, notably restricting the Chinese model DeepSeek and seeing similar bans imposed by the Swedish Tax Agency and the National Agency for Special Needs \(SiS\). These earlier measures illustrate a growing policy that uncontracted AI tools are deemed security risks for government IT environments, setting the context for the new block of ChatGPT and Claude.

**「Impact」** Employees must transition to the approved tools, which may require changes to existing workflows and retraining. Other Swedish agencies, including the Tax Agency and the National Agency for Special Needs, have already implemented similar bans, and the Enforcement Authority \(Kronofogden\) is evaluating a follow‑up, indicating a broader governmental shift toward controlled AI usage.

<details><summary>References</summary>
<ul>
<li><a href="https://madrobot.blog/2026/10/23/sweden-government-offices-block-chatgpt-claude-staff-copilot/">Sweden ’s government blocks ChatGPT and Claude on staff computers</a></li>
<li><a href="https://news.ycombinator.com/item?id=50207405">Swedish government offices to ban ChatGPT and Claude</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#government regulation`, `#AI security`, `#ChatGPT`, `#Claude`

---

## Financial News

<a id="item-finance-news-1"></a>
### [EU lifts 84.2% tariff on Chinese solar glass](https://www.163.com/dy/article/L9R94K6105484D40.html) ⭐️ 7.0/10

The EU Commission announced on 21 Oct 2026 that it is abolishing the 84.2% anti‑dumping and anti‑subsidy duty on Chinese‑origin solar glass, with the measure taking effect on 22 Oct 2026 and duties paid since 22 Jul 2025 eligible for refund \(no interest\).

telegram · zaihuapd · Oct 23, 06:54

**「Background」** The EU had imposed anti‑dumping and anti‑subsidy duties of up to 84.2% on Chinese solar glass since 2014 to protect a domestic industry that no longer has active producers, and Chinese imports fell from about 30.5% during the investigation to roughly 3% of the EU market.

**「Impact」** EU solar‑project developers and installers will face lower glass costs, which could improve project economics and accelerate renewable‑energy deployment in the bloc.

<details><summary>References</summary>
<ul>
<li><a href="https://list.solar/news/eu-repeals-solar-glass-duties-china/">Solar Glass Anti-Dumping Duties on China End After 12 Years</a></li>

</ul>
</details>

**Tags**: `#EU trade policy`, `#Solar energy`, `#China‑EU relations`

---