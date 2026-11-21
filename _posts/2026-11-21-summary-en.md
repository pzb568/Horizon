---
layout: default
title: "Horizon Summary: 2026-11-21 (EN)"
date: 2026-11-21
lang: en
---

> From 40 items, 7 important content pieces were selected

---

**Technology News**
1. [SEC launches probe into Nvidia&\#x27;s accounting practices](#item-tech-news-1) ⭐️ 8.0/10
2. [OpenAI adds API background mode with up to 8‑hour async runs and 40% token discount](#item-tech-news-2) ⭐️ 8.0/10
3. [TSMC suspends sub‑16nm chip orders for Chinese firms](#item-tech-news-3) ⭐️ 8.0/10
4. [TikTok launches global AI deepfake detection tool for public figures](#item-tech-news-4) ⭐️ 7.0/10
5. [Apple developing AI agent for coding, browsing and app control, targeting late 2027](#item-tech-news-5) ⭐️ 7.0/10

**Financial News**
1. [Beijing to ban deposit deductions for normal wear](#item-finance-news-1) ⭐️ 8.0/10
2. [U.S. Companies Shift From Buybacks to Equity Issuances, Adding Supply to Bull Market](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [SEC launches probe into Nvidia&\#x27;s accounting practices](https://www.marketscreener.com/news/us-sec-s-nvidia-probe-is-examining-potential-accounting-issues-sources-say-ce785ed3dd8ff627) ⭐️ 8.0/10

The U.S. Securities and Exchange Commission has opened a formal investigation into Nvidia Corp.&\#x27;s accounting practices, reviewing its recent financial statements and financing arrangements. The probe focuses on potential irregularities in how the company records revenue and manages its capital structure, and it involves current CFO Colette Kress, who is also serving as interim CEO.

hackernews · ftchd · Nov 20, 20:22 · [Discussion](https://news.ycombinator.com/item?id=50581438)

**「Background」** Nvidia is the dominant supplier of GPUs for artificial‑intelligence workloads, and its rapid revenue growth and high market valuation have placed its financial reporting under close regulator scrutiny. The U.S. Securities and Exchange Commission can launch an investigation when it receives tips or detects possible violations of accounting or disclosure rules, a tool it has previously used against technology companies for alleged revenue‑recognition or bookkeeping issues. This regulatory backdrop makes the current SEC probe of Nvidia’s accounting practices noteworthy.

**「Impact」** The investigation could trigger heightened stock volatility and may force Nvidia to restate earnings or face penalties, prompting investors and partners to reassess exposure to the company.

**「Community Discussion」** Commenters noted that the CFO&\#x27;s elevation to interim CEO \(e.g., ralph84\) suggests internal concerns, and others warned the probe could deepen the ongoing correction in Nvidia&\#x27;s share price \(eyeat\).

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/world/us-secs-nvidia-probe-is-examining-potential-accounting-issues-sources-say-2026-11-20/">Nvidia&#x27;s accounting is a focus of US SEC investigation ...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#SEC investigation`, `#AI hardware`, `#Tech finance`

---

<a id="item-tech-news-2"></a>
### [OpenAI adds API background mode with up to 8‑hour async runs and 40% token discount](https://developers.openai.com/api/docs/guides/background) ⭐️ 8.0/10

OpenAI has launched a background mode for its API that makes long‑running requests asynchronous. Developers enable it by adding &quot;background&quot;: true to the request and selecting a completion window of 2 hours or 8 hours via &quot;background\_options.completion\_window&quot;; the 2‑hour window receives a 30% token‑price discount and the 8‑hour window a 40% discount compared with standard rates. The discount currently applies to the GPT‑6.2 Astra, GPT‑6.2 Sol, GPT‑6.1 Terra, and GPT‑6 Luna models in beta, while the default &quot;soonest&quot; option provides no discount. Responses are temporarily stored even if &quot;store&quot; is false or zero‑data‑retention is enabled.

telegram · zaihuapd · Nov 20, 11:15

**「Prerequisite concept」** OpenAI’s API has historically required callers to wait for a response synchronously, with each request billed at the standard per‑token rate regardless of how long the model took to generate the output. Developers needing to run lengthy or resource‑intensive prompts therefore had to keep connections open for the entire processing time and could not benefit from any cost reduction based on duration. The new background mode builds on this model by allowing requests to be queued for asynchronous execution, introducing a completion window \(2 hours or 8 hours\) and offering token‑price discounts for the selected window.

**「Impact」** Developers can off‑load lengthy tasks to run for up to eight hours without keeping a live connection, and they can lower token costs by up to 40% for eligible models, improving both workflow efficiency and budgeting for high‑volume applications.

**Tags**: `#OpenAI API`, `#Background mode`, `#Cost optimization`, `#Long-running tasks`

---

<a id="item-tech-news-3"></a>
### [TSMC suspends sub‑16nm chip orders for Chinese firms](https://appleinsider.com/articles/26/11/20/apple-supplier-tsmc-cuts-off-china-chip-orders-amid-tighter-export-controls) ⭐️ 8.0/10

TSMC has told its customers that it will pause all orders for chips using 16nm or smaller process nodes from Chinese companies. Under the tightened U.S. semiconductor export rules, shipments require a prior U.S. export license or exemption, which Chinese firms have not received. As a result, Chinese customers will be limited to older nodes such as 28nm and 40nm and cannot obtain the high‑bandwidth silicon needed for AI data‑center workloads. Previously TSMO could assess exemption eligibility itself, but the new regulation forces customers to apply for permission in advance, and the current U.S. approved list includes Apple, AMD and Nvidia but no Chinese companies.

telegram · zaihuapd · Nov 21, 02:01

**「Export control context」** The United States has tightened its semiconductor export rules, requiring foreign foundries to obtain a U.S. license or exemption before shipping chips that incorporate U.S. technology to certain destinations. Previously, TSMC could assess each customer’s design for exemption eligibility on its own, but the new rules shift that responsibility to the customer and restrict shipments of advanced nodes such as 16 nm and below unless a license is granted.

**「Impact」** Chinese AI‑hardware vendors will have to rely on legacy process technologies, potentially slowing the rollout of AI accelerators that depend on high‑performance memory and bandwidth, and may need to redesign products or seek alternative suppliers.

**Tags**: `#semiconductors`, `#export controls`, `#AI hardware`, `#TSMC`

---

<a id="item-tech-news-4"></a>
### [TikTok launches global AI deepfake detection tool for public figures](https://www.straitstimes.com/world/tiktok-launches-tool-to-help-public-figures-detect-deepfakes-globally) ⭐️ 7.0/10

TikTok began globally rolling out its Likeness Detection tool on November 20, which notifies verified public figures and top creators when AI‑generated content uses their likeness without permission and lets them file reports. The same day TikTok introduced a public transparency tool that allows anyone to upload an image or video to check whether it was produced by TikTok’s AI, without needing an account. The launch is aimed at supporting the 2027 elections in several European countries after the EU’s August rule requiring AI‑generated content to be labelled.

telegram · zaihuapd · Nov 20, 08:14

**「EU AI labeling requirement」** In August 2026 the European Union enacted a rule that any AI‑generated content shared online must be clearly labelled, driving platforms to implement detection, watermarking and transparency tools for AI‑created media.

**「Impact」** Verified public figures and leading creators will start receiving automated alerts about unauthorized AI‑generated likenesses, giving them a direct way to report and potentially remove deepfakes, which should improve content authenticity on the platform.

<details><summary>References</summary>
<ul>
<li><a href="https://support.claude.com/en/articles/16266773-how-claude-marks-ai-generated-content">How Claude marks AI -generated content | Claude Help Center</a></li>

</ul>
</details>

**Tags**: `#AI Ethics`, `#Deepfake Detection`, `#Content Moderation`, `#Social Media`

---

<a id="item-tech-news-5"></a>
### [Apple developing AI agent for coding, browsing and app control, targeting late 2027](https://www.bloomberg.com/news/articles/2026-11-19/apple-is-working-on-ai-agent-for-device-control-apps-browsing-and-coding) ⭐️ 7.0/10

Apple is hiring a senior engineering manager to lead a &quot;proactive AI agent&quot; project that can write code, browse the web, and control applications. The effort is still in an early stage and Bloomberg says the first version is planned for release no earlier than the end of 2027. The report is based on newly posted job listings, not on a shipped product, and Apple has not publicly confirmed the timeline.

telegram · zaihuapd · Nov 20, 08:59

**「Background」** AI agents that can write code, browse the web, and control applications have already been released by companies such as Meta \(Muse\) and OpenAI, establishing a market for proactive, user‑centric assistants. Apple’s recent macOS 27.3 update added a warning page that expands the permission‑granting steps for third‑party agents from four to fourteen, reflecting growing security concerns around such software. These developments provide the context for Apple’s newly announced hiring of a senior engineering manager to lead its own “proactive AI agent” project.

**「Impact」** If the agent arrives as planned, third‑party AI tools will have to navigate Apple’s expanded macOS permission flow—macOS 27.3 now requires 14 steps \(up from four\) for an external agent to gain control of a Mac—potentially increasing development effort and limiting adoption on Apple platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-19/apple-is-working-on-ai-agent-for-device-control-apps-browsing-and-coding">Apple Is Working on AI Agent for Device Control, Apps... - Bloomberg</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#Apple`, `#software development`, `#industry news`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Beijing to ban deposit deductions for normal wear](https://mp.weixin.qq.com/s/PmGxh5knIyxiBRhpRoJnoQ) ⭐️ 8.0/10

Beijing&\#x27;s housing and market regulators have issued a draft rule that would forbid landlords from deducting security deposits for normal wear and tear and would require rental deposits to be placed in a regulated escrow account.

telegram · zaihuapd · Nov 20, 13:46

**「Background」** The draft revises the 2023 sample lease contract—issued by the Beijing Housing and Urban‑Rural Development Commission and the Market Supervision Administration—that previously permitted landlords to deduct security deposits for normal wear.

<details><summary>References</summary>
<ul>
<li><a href="https://www.beijing.gov.cn/fuwu/bmfw/sy/jrts/202611/t20261120_4954272.html">北京拟修订住房租赁合同示范文本，出租人不得以这种理由扣押金_信息提...</a></li>

</ul>
</details>

**Tags**: `#Housing policy`, `#Rental market`, `#Consumer protection`, `#Beijing`

---

<a id="item-finance-news-2"></a>
### [U.S. Companies Shift From Buybacks to Equity Issuances, Adding Supply to Bull Market](https://www.cnbc.com/2026/11/20/equity-issuance-bull-market-problem.html) ⭐️ 7.0/10

U.S. corporations have moved from share repurchases to issuing new equity, with net new issuance equal to 3.1% of total market capitalization this week, according to Acadian analysis.

rss · CNBC Finance · Nov 20, 14:15

**「Background」** Until recently U.S. companies were net repurchasers of equity, using buybacks to shrink the share count and lift earnings per share, but that pattern has ended as net issuance turned positive.

**「Impact」** The added supply could act as a headwind for the four‑year‑old bull market, potentially lowering stock prices for equity investors.

<details><summary>References</summary>
<ul>
<li><a href="https://www.acadian-asset.com/investment-insights/owenomics/the-smart-money-is-selling-equity">The smart money is selling equity | Acadian Asset Management</a></li>

</ul>
</details>

**Tags**: `#equity issuance`, `#bull market`, `#corporate finance`, `#IPO`, `#market trends`

---