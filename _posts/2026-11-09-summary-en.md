---
layout: default
title: "Horizon Summary: 2026-11-09 (EN)"
date: 2026-11-09
lang: en
---

> From 31 items, 6 important content pieces were selected

---

**Technology News**
1. [Outlook.com Begins Rejecting Mail from Domains Without DMARC](#item-tech-news-1) ⭐️ 8.0/10
2. [KetchUp – Open‑source SketchUp alternative built with Rust and WebGPU](#item-tech-news-2) ⭐️ 7.0/10
3. [Nvidia Board Launches Probe into CEO Jensen Huang Over Espionage Allegations](#item-tech-news-3) ⭐️ 7.0/10
4. [Goldman Sachs pulls Claude Code from traders over security, compliance, and cost](#item-tech-news-4) ⭐️ 7.0/10
5. [Anthropic Report Shows Scientists Use Claude Primarily for Data Analysis and Writing](#item-tech-news-5) ⭐️ 7.0/10
6. [Windows 11 tests unified app‑update page to replace third‑party pop‑ups](#item-tech-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Outlook.com Begins Rejecting Mail from Domains Without DMARC](https://mailroute.net/blog/outlook-rejecting-email-without-dmarc) ⭐️ 8.0/10

Outlook.com has started rejecting email messages that originate from domains without a published DMARC record. The rejection is silent for the sender—messages are dropped or result in a permanent 5xx delivery failure—so no bounce is returned. This change affects any outbound mail sent to Outlook.com users from domains that have not implemented DMARC, prompting senders to add a DMARC policy to maintain deliverability.

hackernews · xmddmx · Nov 8, 19:20 · [Discussion](https://news.ycombinator.com/item?id=50416158)

**「DMARC and email authentication」** DMARC \(Domain-based Message Authentication, Reporting &amp; Conformance\) is an email‑authentication protocol that builds on SPF and DKIM to let domain owners specify how receivers should handle unauthenticated mail. Many large providers, including Outlook.com, have begun to enforce DMARC by rejecting messages from domains that lack a valid DMARC record, often returning a 5xx permanent failure. This policy shift means senders must publish a DMARC DNS record to maintain deliverability to Outlook.com users.

**「Impact」** Mail operators must publish a DMARC policy for their domains; otherwise, messages to Outlook.com recipients will be discarded, potentially causing loss of legitimate email and requiring immediate DNS updates.

**「Community Discussion」** Commenters note that Outlook.com’s behavior is either a silent drop or a 5xx permanent failure, and many consider the move overdue but frustrating for those managing their own mail servers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.factae.eu/en/article/outlook-com-quietly-rejects-emails-from-domains-without-dmarc-182744">Outlook . com quietly rejects emails from domains without DMARC</a></li>
<li><a href="https://news.ycombinator.com/item?id=50416158">Outlook . com Is Quietly Rejecting Email from Domains Without DMARC</a></li>

</ul>
</details>

**Tags**: `#email`, `#security`, `#DMARC`, `#Outlook.com`, `#infrastructure`

---

<a id="item-tech-news-2"></a>
### [KetchUp – Open‑source SketchUp alternative built with Rust and WebGPU](https://ketchup3d.github.io/app/) ⭐️ 7.0/10

KetchUp, an open‑source 3D modeling application, was released and runs in the browser using Rust and the WebGPU graphics API. The tool aims to provide a free, SketchUp‑like experience while showcasing modern, high‑performance graphics tooling for developers. It is available at https://ketchup3d.github.io/app/ and can be built from source on any platform that supports Rust and WebGPU.

hackernews · dcoulmbe · Nov 8, 22:35 · [Discussion](https://news.ycombinator.com/item?id=50418176)

**「Background」** SketchUp is a long‑standing, proprietary 3D modeling application used for architecture, woodworking and other design tasks, typically installed as a desktop program. Recent advances in the Rust language and the WebGPU graphics API let developers compile high‑performance graphics code to WebAssembly, which can run directly in browsers without plugins. KetchUp builds on this stack—Rust, WebAssembly and WebGPU—to deliver a free, open‑source, cross‑platform SketchUp‑style editor that runs in the browser or on desktop and supports importing SketchUp \(.skp\) files and exporting OBJ models.

**「Impact」** Developers can study KetchUp’s code as a concrete example of integrating Rust with WebGPU for cross‑platform UI, potentially accelerating similar web‑based graphics projects. Hobbyists and makers gain a free, lightweight modeling option that mirrors SketchUp’s workflow without licensing constraints.

**「Community Discussion」** Commenters praised the Rust‑driven UI performance and welcomed KetchUp as a spiritual successor to SketchUp, while noting usability quirks such as being prompted to name every rectangle drawn.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Ketchup3D/app">GitHub - Ketchup3D/app: Free, open-source 3D modeling ...</a></li>
<li><a href="https://daily.dev/posts/ketchup-open-source-sketchup-alternative-built-with-rust-and-webgpu-lquqfnjed">KetchUp – Open-source SketchUp alternative built with Rust ...</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#WebGPU`, `#3D Modeling`, `#Open Source`, `#Graphics`

---

<a id="item-tech-news-3"></a>
### [Nvidia Board Launches Probe into CEO Jensen Huang Over Espionage Allegations](https://nvidianews.nvidia.com/news/statement-from-nvidia-board-of-directors) ⭐️ 7.0/10

Nvidia&\#x27;s board of directors has opened an internal investigation concerning CEO Jensen Huang after he disclosed personal misconduct and alleged that he was the target of a foreign intelligence operation. The probe will examine the alleged espionage incident and its potential impact on company governance and security. No details on the investigation’s scope or timeline have been released.

hackernews · vincentchau · Nov 8, 20:26 · [Discussion](https://news.ycombinator.com/item?id=50416801)

**「Context of Nvidia’s Board Investigation」** Board‑level investigations are typically launched when a company’s leadership faces potential security or governance risks. In Nvidia’s case, the board opened an inquiry after CEO Jensen Huang disclosed to the board that he had been involved in an intimate relationship that may have exposed him to a Chinese espionage operation, prompting concerns about foreign influence and corporate security. Similar high‑profile probes have occurred in the tech sector when executives’ personal matters intersect with national‑security concerns, making this step a standard response to protect the company’s assets and reputation.

**「Community Discussion」** Commenters noted that the headline is misleading; the board is investigating a spying case that targeted Huang, not investigating Huang himself \(nrmitchi\). Others cited Bloomberg reporting that the board’s probe follows Huang’s admission of infidelity \(enlyth\).

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-08/nvidia-board-to-probe-spying-case-after-ceo-jensen-huang-admits-infidelity">Nvidia Board to Probe Spying Case After CEO Jensen Huang ...</a></li>
<li><a href="https://www.nytimes.com/2026/11/08/technology/nvidia-investigation-jensen-huang-china.html">Nvidia Opens Investigation Into Jensen Huang’s Relationship ...</a></li>
<li><a href="https://techcrunch.com/2026/11/08/nvidia-says-its-investigating-ceo-jensen-huangs-relationship-with-possible-chinese-spy/">Nvidia will investigate CEO Jensen Huang’s relationship with ...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI Hardware`, `#Corporate Governance`, `#Security`

---

<a id="item-tech-news-4"></a>
### [Goldman Sachs pulls Claude Code from traders over security, compliance, and cost](https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers) ⭐️ 7.0/10

Goldman Sachs has removed Anthropic&\#x27;s Claude Code coding assistant from its traders and bankers, citing security, compliance, and billing concerns. The decision reflects practical hurdles in deploying LLM‑based coding tools on workstations that handle sensitive client and trade data.

hackernews · TheWiggles · Nov 8, 18:16 · [Discussion](https://news.ycombinator.com/item?id=50415628)

**「Claude Code and prior AI restrictions at Goldman Sachs」** Claude Code is Anthropic’s large‑language‑model‑based coding assistant that can generate and edit software code from natural‑language prompts. In October 2026 Goldman Sachs updated internal guidelines to limit the use of advanced AI coding tools after a productivity‑and‑risk review, restricting access to its roughly 12,000 engineers while cutting off traders, bankers and analysts. This prior restriction provides context for the recent decision to pull Claude Code from those non‑engineer staff.

**「Impact」** Traders will no longer have access to Claude Code for on‑the‑fly code generation and must revert to existing internal tools or seek alternative AI assistants that meet the firm’s compliance and cost requirements.

**「Community Discussion」** Commenters note that running semi‑unattended coding agents on primary finance workstations poses a &quot;lethal trifecta&quot; of data leakage, regulatory risk, and uncontrolled billing, underscoring why Goldman pulled the tool.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-02/goldman-restricts-traders-and-bankers-from-using-some-ai-tools">Goldman Restricts Traders and Bankers From Using Some AI ...</a></li>
<li><a href="https://aiweekly.co/alerts/goldman-sachs-pulls-claude-code-and-github-copilot-from-traders-and-bankers">Goldman Sachs Pulls Claude Code and GitHub Copilot From ...</a></li>

</ul>
</details>

**Tags**: `#AI governance`, `#enterprise AI`, `#LLM deployment`, `#finance technology`

---

<a id="item-tech-news-5"></a>
### [Anthropic Report Shows Scientists Use Claude Primarily for Data Analysis and Writing](https://www.anthropic.com/research/how-researchers-use-claude) ⭐️ 7.0/10

Anthropic’s analysis of 207,000 research‑oriented conversations from August‑September 2026 found that 33.7% of Claude usage and 48.1% of Claude Code usage were for data analysis, while 32% of Claude usage was for writing. The report notes that computer science and mathematics researchers use Claude more per‑capita than experimental fields such as chemistry or medicine.

telegram · zaihuapd · Nov 9, 01:29

**「Claude usage context」** Claude is Anthropic’s large‑language‑model platform offered through consumer plans such as the Chat interface \(referred to as “Claude”\) and Claude Code, an agentic coding assistant. These services are used by researchers for conversational and knowledge‑work tasks, including data analysis and scientific writing, which the new report quantifies based on millions of sessions. Understanding Claude’s role as a general‑purpose AI assistant clarifies why its adoption rates in research workflows are noteworthy.

**「Impact」** Anthropic estimates that broad adoption of Claude could double research output in some domains and, if AI handled all non‑physical tasks, could increase productivity up to 15‑fold in fields like computer science.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/how-researchers-use-claude">How scientists use Claude \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Large Language Models`, `#Research Productivity`, `#Data Analysis`, `#Claude`

---

<a id="item-tech-news-6"></a>
### [Windows 11 tests unified app‑update page to replace third‑party pop‑ups](https://www.windowslatest.com/2026/11/09/for-20-years-windows-apps-like-java-have-nagged-you-with-their-own-update-pop-ups-and-windows-11-now-wants-to-end-it/) ⭐️ 7.0/10

Windows 11 is testing a new &quot;App updates&quot; feature that will list third‑party application updates in Settings &gt; Apps, removing the separate pop‑up dialogs that programs such as Java currently show. Developers must register as a provider and supply an update‑check script for their apps. The OS will schedule the installations using the same intelligent logic as Windows Update—considering device usage, battery level, and network conditions—and will scan for updates roughly every 22 hours. The feature is still in the final testing stage and is not yet available to users.

telegram · zaihuapd · Nov 9, 02:09

**「Background」** Historically, Windows has not provided a built‑in mechanism for third‑party applications to receive updates; developers typically implement their own update checkers that show separate pop‑up dialogs \(e.g., Java, Adobe\). While the Microsoft Store can auto‑update apps distributed through it, many legacy and non‑Store apps continue to rely on these independent update prompts. This new unified “App updates” page extends the OS‑level update scheduling used for Windows updates to third‑party software.

**「Impact」** When released, users will see a single, system‑managed page for all app updates instead of scattered pop‑ups, and developers will need to integrate with the new provider registration and scripting API to have their updates appear there.

**Tags**: `#windows`, `#operating-systems`, `#software-updates`, `#developer-tools`

---