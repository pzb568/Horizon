---
layout: default
title: "Horizon Summary: 2026-11-23 (EN)"
date: 2026-11-23
lang: en
---

> From 28 items, 3 important content pieces were selected

---

**Technology News**
1. [Windows Server 2028 Drops Default 32‑bit Support, WoW64 Optional](#item-tech-news-1) ⭐️ 8.0/10
2. [Google builds Mirror Dimension simulated internet for Chrome AI agent testing](#item-tech-news-2) ⭐️ 7.0/10

**Financial News**
1. [Record Super El Niño Temperatures Threaten Food Security](#item-finance-news-1) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Windows Server 2028 Drops Default 32‑bit Support, WoW64 Optional](https://www.windowslatest.com/2026/11/23/32-bit-apps-days-are-numbered-as-microsoft-strips-support-bit-by-bit-starting-with-windows-server-2028-but-windows-11-is-safe-for-now/) ⭐️ 8.0/10

At Ignite 2026 Microsoft announced that Windows Server 2028 will ship without the WoW64 compatibility subsystem, meaning 32‑bit applications cannot run out‑of‑the‑box. The server edition is slated for a fall 2027 release alongside Windows 11 version 27H2. Administrators can reinstall WoW64 on demand via the FoD \(Feature on Demand\) mechanism, typically using PowerShell or DISM on Server Core installations. Microsoft says the change reduces the attack surface and blocks 32‑bit malware, while Windows 11 will continue to include WoW64 for the time being.

telegram · zaihuapd · Nov 23, 03:03

**「WoW64 subsystem and its role」** WoW64 \(Windows‑on‑Windows 64\) is the compatibility layer that lets 64‑bit Windows run 32‑bit applications by translating their system calls. All recent Windows client and server releases have shipped WoW64 by default, allowing legacy 32‑bit software to operate on modern 64‑bit hardware. Removing WoW64 from the default Windows Server 2028 installation therefore eliminates the built‑in support that administrators have relied on for running such applications.

**「Impact」** Organizations that rely on legacy 32‑bit server software will need to modify deployment scripts to add WoW64 after installation, adding extra steps and potential compatibility testing before the Windows Server 2028 rollout.

**Tags**: `#Windows Server`, `#32-bit compatibility`, `#system administration`

---

<a id="item-tech-news-2"></a>
### [Google builds Mirror Dimension simulated internet for Chrome AI agent testing](https://www.landian.news/archives/128701.html) ⭐️ 7.0/10

Google has set up an internal test environment called Mirror Dimension, a large‑scale simulated internet used to evaluate Chrome’s AI browsing agent. The sandbox contains thousands of mock websites and runs over 1,000 isolated test cases per day per engineer, covering actions such as opening pages, searching, logging in, adding items to carts, and completing tasks. A key purpose is to defend the agent against prompt‑injection attacks from malicious webpages. This infrastructure is for internal engineering use and is not a public feature.

telegram · zaihuapd · Nov 23, 01:30

**「Background: Chrome AI agents and safe testing」** Chrome’s AI browsing agents are software components that can navigate the web, search, log in, and perform tasks on behalf of users. To evaluate their behavior safely, Google created a synthetic web environment called Mirror Dimension, which replicates thousands of sites in isolation so agents can be run against realistic pages without exposing real users or services to potential prompt‑injection attacks. This approach extends Google’s prior internal security testing of browser features to the new AI agents.

**「Impact」** The testbed lets Chrome engineers safely validate the AI agent’s functionality and security before any public rollout, helping to reduce the risk of prompt‑injection exploits reaching users.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wired.com/story/google-built-a-giant-mirror-dimension-internet-to-test-its-chrome-ai-agents/">Google Built a Giant ‘ Mirror Dimension ’ Internet to Test Its Chrome ...</a></li>
<li><a href="https://blog.google/security/mirror-dimension-for-agents/">Mirror Dimension for Agents : Evaluating Browser-Use Agents ...</a></li>

</ul>
</details>

**Tags**: `#Chrome`, `#AI agents`, `#Web security`, `#Testing infrastructure`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Record Super El Niño Temperatures Threaten Food Security](https://www.wired.com/story/how-this-years-super-el-nino-will-worsen-global-hunger/) ⭐️ 8.0/10

Record super El Niño sea‑surface temperatures of 3.5 °C \(forecast to peak near 4 °C\) could push an additional 49 million people into acute food insecurity, raising the global total to 274 million, according to the UN World Food Programme.

telegram · zaihuapd · Nov 22, 14:09

**「Background」** El Niño is a periodic warming of the central‑tropical Pacific that this year has reached about 3.5 °C—well above the previous record of roughly 2.75 °C—driving droughts that threaten crops.

**「Impact」** Aid funding has fallen 30% from its 2022 peak, so the World Food Programme can now assist fewer than 1 million people in Somalia instead of 10 million, leaving many vulnerable households without help.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/environment/2026/sep/21/super-el-nino-temperature-record">‘Jaw-dropping’ El Niño bursts through temperature record months...</a></li>

</ul>
</details>

**Tags**: `#Climate`, `#Food Security`, `#El Niño`, `#Global Hunger`, `#Economic Impact`

---