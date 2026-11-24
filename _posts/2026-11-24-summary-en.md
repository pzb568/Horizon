---
layout: default
title: "Horizon Summary: 2026-11-24 (EN)"
date: 2026-11-24
lang: en
---

> From 38 items, 8 important content pieces were selected

---

**Technology News**
1. [Codex2api Supply‑Chain Attack Injects Backdoored Release](#item-tech-news-1) ⭐️ 8.0/10
2. [HarmonyOS devices top 100 million, apps over 460 k](#item-tech-news-2) ⭐️ 8.0/10
3. [Singapore PM says Singapore will not be conduit for evading US chip export bans](#item-tech-news-3) ⭐️ 8.0/10
4. [Nvidia Board Reinstates Jensen Huang as CEO](#item-tech-news-4) ⭐️ 7.0/10
5. [Stalwart positioned as drop‑in replacement for Microsoft Exchange](#item-tech-news-5) ⭐️ 7.0/10
6. [Alpöge’s AI‑generated Lean proof of Riemann hypothesis admitted as junk](#item-tech-news-6) ⭐️ 7.0/10

**Financial News**
1. [Fed&\#x27;s New York President Williams signals gradual rate hikes](#item-finance-news-1) ⭐️ 8.0/10
2. [Anthropic IPO triggers sell‑off, clouds Chinese AI listings](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Codex2api Supply‑Chain Attack Injects Backdoored Release](https://github.com/WormW/codex2api-incident-2026-11) ⭐️ 8.0/10

The open‑source Codex2api repository was compromised when the author’s account was hijacked and an attacker pushed a tag that bypassed the main branch, publishing version 3.1.11 with authentication removed, allowing unauthenticated remote command execution. A malicious workflow also exfiltrated 16 GitHub Actions secrets, affecting at least 21 repositories under the same account. Users who have installed or updated to versions 3.1.10‑3.1.12 are urged to stop using them, revert to version 3.1.9, and rotate all GitHub tokens, SSH keys, database credentials, and DeepSeek keys.

telegram · zaihuapd · Nov 23, 11:21

**「What is Codex2api」** Codex2api is an open‑source proxy server that forwards requests to the OpenAI Codex Responses API, supporting multiple client formats such as OpenAI Chat, Anthropic Messages and Gemini, and providing features like account pooling and abuse protection. It is maintained as a public GitHub repository and is used by developers to integrate Codex capabilities without direct OpenAI credentials.

**「Impact」** Affected developers must immediately disable the compromised releases, roll back to a safe version, and rotate all related secrets to prevent unauthorized access and potential data leakage.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/rokyplay/codex2api">GitHub - rokyplay/codex2api: OpenAI Codex API proxy with ...</a></li>
<li><a href="https://github.com/ZHX08/codex2api/blob/main/README.md">codex2api/README.md at main · ZHX08/codex2api · GitHub</a></li>

</ul>
</details>

**Tags**: `#security`, `#supply-chain`, `#AI-tools`, `#open-source`

---

<a id="item-tech-news-2"></a>
### [HarmonyOS devices top 100 million, apps over 460 k](https://www.xinhuanet.com/20261124/68842538167d4e59a875056d5eb885ad/c.html) ⭐️ 8.0/10

Huawei Terminal Co announced on November 24 that the number of phones, tablets and computers running HarmonyOS 5, 6 or 7 has surpassed 100 million units. The OS now provides more than 460,000 applications and services and has over 12 million registered developers. HarmonyOS was first released in 2019, with a native version launched in October 2024, and its open‑source project now includes about 14,000 contributors and 120 industry distributions.

telegram · zaihuapd · Nov 24, 01:46

**「Background on HarmonyOS」** HarmonyOS is Huawei’s operating system for phones, tablets and computers. It was first announced in 2019, and a fully native version was released in October 2024. Since then the platform has been open‑sourced, attracting more than 14 000 contributors and over 120 industry‑specific distributions, which underpins the current claim of 100 million devices and a 460 000‑plus app ecosystem.

**「Impact」** The expanded device base and app ecosystem give developers a sizable new market in China, encouraging them to add or port apps to HarmonyOS and to engage with Huawei’s open‑source tooling and distribution channels.

**Tags**: `#Operating Systems`, `#Huawei`, `#Open Source`, `#Mobile Development`

---

<a id="item-tech-news-3"></a>
### [Singapore PM says Singapore will not be conduit for evading US chip export bans](https://www.bloomberg.com/news/articles/2026-11-24/singapore-won-t-be-conduit-to-skirt-us-chip-curbs-wong-says) ⭐️ 8.0/10

Singapore Prime Minister Lawrence Wong announced that Singapore will not be used as a channel to evade U.S. semiconductor export restrictions. He said authorities are investigating Megaspeed’s purchase of Nvidia chips for possible violations. The U.S. Commerce Department has already placed Megaspeed and six other Southeast Asian firms on its trade blacklist for “significant risk” of transferring advanced computing products to unauthorized users, including related entities in Malaysia and Thailand. Alibaba’s Singapore subsidiary Apex Enterprise Solutions was also listed, though the company says it never transferred controlled chips.

telegram · zaihuapd · Nov 24, 05:03

**「Background」** The United States enforces export controls on advanced semiconductor products—such as Nvidia GPUs—through the Export Administration Regulations and the Entity List, targeting firms that might supply them to prohibited end‑users. In recent months the Commerce Department has expanded the blacklist to include several Southeast Asian companies suspected of moving high‑performance compute chips to unauthorized customers, prompting regional governments to clarify their compliance stance.

**「Impact」** Companies operating in Singapore that deal with advanced AI chips must now demonstrate compliance with U.S. export rules, and may face investigations or export licensing hurdles, potentially disrupting supply chains for AI hardware in the region.

**Tags**: `#chip export controls`, `#hardware`, `#AI compute`, `#geopolitics`

---

<a id="item-tech-news-4"></a>
### [Nvidia Board Reinstates Jensen Huang as CEO](https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html) ⭐️ 7.0/10

Nvidia’s board voted on November 23, 2026 to reinstate co‑founder Jensen Huang as chief executive officer, reversing his removal earlier that month. The decision restores Huang’s leadership of Nvidia’s AI‑hardware business and applies to the company’s public shareholders.

hackernews · jaz · Nov 23, 14:00 · [Discussion](https://news.ycombinator.com/item?id=50611576)

**「Context of Jensen Huang’s Reinstatement」** Jensen Huang co‑founded Nvidia in 1993 and has served as its chief executive for more than three decades. Earlier in 2026 the company’s board voted to remove him amid undisclosed concerns that involved senior U.S. government input, prompting a brief leadership change. The board’s recent unanimous vote to reinstate Huang restores the long‑standing leadership structure and signals that the board, after consulting government officials, believes the reinstatement poses no national‑security risk.

**「Impact」** The leadership reversal is expected to stabilize Nvidia’s strategic direction, reassuring investors and enterprise customers who were unsettled by Huang’s brief ouster and potentially supporting the company’s stock price and ongoing AI‑chip roadmap.

**「Community Discussion」** A commenter pointed out that under Delaware’s Caremark precedent, the board faces a high bar for liability, so the unanimous vote and the Department of Justice’s decision not to prosecute are likely to protect directors from legal repercussions.

**Tags**: `#Nvidia`, `#Leadership`, `#AI hardware`, `#Industry news`

---

<a id="item-tech-news-5"></a>
### [Stalwart positioned as drop‑in replacement for Microsoft Exchange](https://stalw.art/blog/microsoft-exchange-replacement/) ⭐️ 7.0/10

Stalwart now markets itself as a drop‑in replacement for Microsoft Exchange, offering an open‑source, on‑premises mail server for organizations whose Exchange deployments are being retired. The server is intended to run in‑house and to handle standard email protocols, allowing sysadmins to replace Exchange without moving to Microsoft’s cloud services. It targets enterprises and administrators needing an on‑prem solution as Microsoft phases out on‑prem Exchange support.

hackernews · shaunpud · Nov 23, 22:32 · [Discussion](https://news.ycombinator.com/item?id=50620349)

**「Background」** Microsoft Exchange has been the de‑facto on‑premises mail server for enterprises for over two decades, tightly integrated with Outlook via proprietary protocols such as MAPI and EWS. In recent releases Microsoft announced that it will discontinue on‑prem Exchange support, pushing customers toward its cloud‑based Office 365 services. Stalwart 1.2.0 adds full implementations of MAPI, EWS, ActiveSync and Autodiscover, allowing existing Outlook, Apple Mail and mobile clients to connect without configuration changes, which is why it can be positioned as a drop‑in replacement.

**「Compliance and client considerations」** Organizations can replace on‑premises Exchange with Stalwart and keep existing mail clients, but they will need to add a separate, tamper‑proof archiving solution to satisfy German GoBD regulations and may have to adjust Outlook or use IMAP because full MAPI integration is not provided.

**「Community discussion」** One commenter noted that Stalwart’s current plans \(including the OSS version\) lack a GoBD‑compliant archiving feature required in Germany, which could limit its adoption for companies subject to that regulation.

<details><summary>References</summary>
<ul>
<li><a href="https://stalw.art/blog/microsoft-exchange-replacement/">Stalwart is now a drop-in replacement for Microsoft Exchange</a></li>
<li><a href="https://www.learn.telusko.com/newsletter/stalwart-1-2-0-is-now-a-drop-in-replacement-for-microsoft-exchange">Stalwart 1.2.0 is now a drop-in replacement for Microsoft ...</a></li>
<li><a href="https://stalw.art/blog/microsoft-exchange-replacement/">Stalwart is now a drop-in replacement for Microsoft Exchange | Stalwart</a></li>

</ul>
</details>

**Tags**: `#email`, `#open-source`, `#enterprise`, `#mail-server`

---

<a id="item-tech-news-6"></a>
### [Alpöge’s AI‑generated Lean proof of Riemann hypothesis admitted as junk](https://x.com/i/web/status/2124987173439209561) ⭐️ 7.0/10

Alpöge and Claude announced an AI‑generated Lean proof of the Riemann hypothesis and its generalization, releasing about 17 million lines of Lean code across 175 000 files but no human‑readable argument. The Lean and Mathlib community initially expressed confidence in the code, but researchers later identified that key definitions were trivialized, making the proof effectively empty. On the 23rd, Alpöge admitted that the 250 000‑page codebase was a joke, describing it as &quot;full of garbage but it compiles,&quot; and acknowledged the criticism as justified.

telegram · zaihuapd · Nov 24, 01:29

**「Prior AI claim of RH proof」** Levent Alpöge announced on 20 Nov 2026 that he and Anthropic’s AI model Claude had generated a purported proof of the Riemann hypothesis in Lean, releasing about 17 million lines of code that the Mathlib community initially said gave them confidence in the result. The claim relied on Lean, a proof‑assistant language, and the extensive Mathlib library to formalise the theorem. This earlier announcement provides the context for Alpöge’s later admission that the code was largely nonsensical.

<details><summary>References</summary>
<ul>
<li><a href="https://www.clarin.com/us-news/who-is-levent-alpoge-the-anthropic-mathematician-who-claims-solved-the-riemann-hypothesis-with-claude_0_2WdGvYKBVM.html">Who is Levent Alpöge ? The Anthropic mathematician who claims he...</a></li>
<li><a href="https://www.npr.org/2026/11/21/g-s1-154922/anthropic-worker-claims-to-have-solved-a-holy-grail-of-math-problems-with-the-help-of-ai">Anthropic worker claims to have solved a Holy Grail of math... : NPR</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Formal Verification`, `#Theorem Proving`, `#Lean`, `#Riemann Hypothesis`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed&\#x27;s New York President Williams signals gradual rate hikes](https://www.cnbc.com/2026/11/23/john-williams-fed-inflation-rate-hikes.html) ⭐️ 8.0/10

New York Fed President John Williams said inflation should near the 2% goal in 2027 and that further rate hikes may occur over time, with markets pricing in a 0.25 percentage‑point increase from the current 3.75‑4% target range at the December FOMC meeting.

rss · CNBC Finance · Nov 23, 21:02

**「Background」** The Federal Reserve aims for 2% inflation and sets the federal funds rate target range; the next policy decision is the FOMC meeting on Dec 8‑9, 2026.

**「Impact」** Borrowers could face slightly higher loan costs if the anticipated 0.25 percentage‑point rate rise is implemented.

**Tags**: `#monetary policy`, `#inflation`, `#Federal Reserve`

---

<a id="item-finance-news-2"></a>
### [Anthropic IPO triggers sell‑off, clouds Chinese AI listings](https://www.bloomberg.com/news/articles/2026-11-23/china-s-next-ai-deals-clouded-by-selloff-after-anthropic-ipo) ⭐️ 7.0/10

Anthropic’s $119.5 billion AI IPO sparked a global sell‑off that has erased about $1.7 trillion of Chinese tech stocks since the end of June, putting the planned listings of DeepSeek and 月之暗面 in doubt.

telegram · zaihuapd · Nov 23, 09:31

**「Background」** DeepSeek was preparing to file for a mainland STAR Market IPO as early as the end of 2026 for a 2027 debut, and Moonshot AI had confidentially filed for a Hong Kong listing planned for early 2027, both before Anthropic’s $119.5 billion record AI IPO sparked a $1.7 trillion sell‑off in Chinese tech stocks since late June.

<details><summary>References</summary>
<ul>
<li><a href="https://www.straitstimes.com/business/deepseek-preparing-for-ipo-filing-as-soon-as-end-2026">DeepSeek IPO plans: Filing by end-2026 for 2027 debut | The ...</a></li>
<li><a href="https://chinaaicompass.com/companies/moonshot-ai">Moonshot AI（月之暗面（Kimi）） — China AI Compass</a></li>

</ul>
</details>

**Tags**: `#AI`, `#IPO`, `#ChineseTech`, `#MarketSelloff`

---