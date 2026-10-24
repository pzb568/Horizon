---
layout: default
title: "Horizon Summary: 2026-10-24 (ZH)"
date: 2026-10-24
lang: zh
---

> 从 33 条内容中筛选出 8 条重要资讯。

---

**科技新闻**
1. [Amazon’s Trainium Takes a Strike at the Training King](#item-tech-news-1) ⭐️ 8.0/10
2. [微软悄悄测试 Win11 不同于 Recall 的 AI 记忆应用 Pantheon](#item-tech-news-2) ⭐️ 8.0/10
3. [PHP 基金会建议暂时禁用上传进度功能](#item-tech-news-3) ⭐️ 8.0/10
4. [🤖 KIMI K3.1-Pro 模型正式发布](#item-tech-news-4) ⭐️ 8.0/10
5. [iPhone 新漏洞演示及安全影响](#item-tech-news-5) ⭐️ 7.0/10
6. [Dessa: the most authentic full-duplex speech model ever built](#item-tech-news-6) ⭐️ 7.0/10
7. [瑞典政府办公室禁用 ChatGPT 与 Claude](#item-tech-news-7) ⭐️ 7.0/10

**财经新闻**
1. [欧盟取消对中国太阳能玻璃双反关税](#item-finance-news-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Amazon’s Trainium Takes a Strike at the Training King](https://newsletter.semianalysis.com/p/amazons-trainium-takes-a-strike-at) ⭐️ 8.0/10

Amazon enhances Trainium with native PyTorch training, improving its appeal for ML research and production.

rss · Semianalysis · 10月23日 19:06

**标签**: `#AWS Trainium`, `#Machine Learning Hardware`, `#PyTorch`, `#AI Infrastructure`

---

<a id="item-tech-news-2"></a>
### [微软悄悄测试 Win11 不同于 Recall 的 AI 记忆应用 Pantheon](https://www.windowslatest.com/2026/10/23/microsoft-is-quietly-testing-another-recall-for-windows-11-but-this-one-doesnt-record-your-screen/) ⭐️ 8.0/10

Microsoft is testing Project Pantheon, an AI memory app for Windows 11 that stores selected user content for AI queries.

telegram · zaihuapd · 10月23日 07:42

**标签**: `#Windows`, `#AI`, `#Productivity`, `#Operating Systems`, `#Microsoft`

---

<a id="item-tech-news-3"></a>
### [PHP 基金会建议暂时禁用上传进度功能](https://x.com/ThePHPF/status/2113580383875019242) ⭐️ 8.0/10

PHP 基金会在 2026 年 10 月 23 日发布公告，建议在下一个 PHP 版本发布前将 php.ini 中的 session.upload\_progress.enabled 设置为 0，以防止 CVE‑2026‑115560 所导致的远程代码执行漏洞。该漏洞仅影响在运行时将非默认 serialize\_handler 切换为 “php” 的应用。基金会此前已因 CVE‑2026‑109619 建议保持该功能禁用。

telegram · zaihuapd · 10月23日 13:46

**「背景」** PHP 的上传进度功能通过 session.upload\_progress.enabled 开关在会话中记录文件上传的实时状态，依赖于 session.serialize\_handler 的序列化方式。若在运行时将 serialize\_handler 从默认值改为 “php”，则上传进度数据的序列化/反序列化过程会出现不匹配，进而可能被利用触发远程代码执行（RCE），这正是 CVE‑2026‑115560 所描述的漏洞。PHP 基金会此前已因 CVE‑2026‑109619 发布过类似建议，要求在官方修复前禁用该功能，以降低风险。

**「影响」** 受影响的站点应立即在配置文件或运行时关闭上传进度功能，否则可能被利用执行任意代码；同时需检查代码是否在运行时更改 serialize\_handler 为 “php”，并在下个 PHP 版本修复前保持禁用状态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/php-shares-mitigation-for-new-and-unpatched-rce-vulnerability/">PHP shares mitigation for new RCE vulnerability with no patch</a></li>
<li><a href="https://help.nextcloud.com/t/new-php-vulnerability-cve-2026-115560-in-community-docker-image/251425">New PHP vulnerability CVE - 2026 - 115560 in community docker image</a></li>

</ul>
</details>

**标签**: `#php`, `#security`, `#vulnerability`

---

<a id="item-tech-news-4"></a>
### [🤖 KIMI K3.1-Pro 模型正式发布](https://www.kimi.ai/blog/kimi-k3-1-pro) ⭐️ 8.0/10

KIMI releases its 30‑trillion‑parameter K3.1‑Pro model, promising stronger coding, 3D, and finance capabilities with extended context length.

telegram · zaihuapd · 10月23日 17:14

**标签**: `#large-language-model`, `#software-engineering`, `#AI-tools`, `#3D-generation`

---

<a id="item-tech-news-5"></a>
### [iPhone 新漏洞演示及安全影响](https://blog.calif.io/p/iphone) ⭐️ 7.0/10

博客作者披露了一项针对最新 iPhone 型号的漏洞利用演示，展示了可在设备上获取更高权限的攻击路径。文章提供了对硬件和系统安全机制的分析，供安全工程师参考，但未透露足以判断该漏洞是否突破了现有防御的细节。

hackernews · pavel\_lishin · 10月23日 16:21 · [社区讨论](https://news.ycombinator.com/item?id=50211474)

**「背景信息」** iPhone 的安全体系长期依赖硬件根信任、代码签名和沙箱隔离，导致越狱（jailbreak）通常需要利用内核漏洞或硬件调试接口。近期在 2026 年 10 月的 Hexacon（巴黎）上，Calif 团队展示了针对 iOS 27 的一系列攻击演示，包括一键信号拦截和持久化威胁（APT），并计划随后公开细节。这些演示延续了该团队此前在 2026 年 9 月发布的首个通过微信通话实现的跨平台零点击蠕虫的研究。

**「影响」** 安全团队需要将该演示视为潜在风险，评估现有防护（如 Lockdown 模式）是否能阻止相同攻击，并在可行时推动系统更新或补丁以降低被利用的可能性。

**「社区讨论」** 有评论者（如 jeroenhd）询问 Lockdown 模式在实际中能否抵御此类漏洞，反映出社区对现有防御措施有效性的关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.calif.io/p/iphone">iPhone - Calif Newsletter</a></li>
<li><a href="https://blog.calif.io/archive">Archive - Calif Newsletter</a></li>

</ul>
</details>

**标签**: `#security`, `#iOS`, `#jailbreak`, `#hardware`

---

<a id="item-tech-news-6"></a>
### [Dessa: the most authentic full-duplex speech model ever built](https://block.xyz/dessa) ⭐️ 7.0/10

Dessa introduces an impressive low‑data, locally‑run full‑duplex speech model, offering high‑value insight for AI and software engineers.

hackernews · dsr12 · 10月23日 19:09 · [社区讨论](https://news.ycombinator.com/item?id=50213925)

**标签**: `#speech-synthesis`, `#full-duplex`, `#local-inference`, `#low-data-training`

---

<a id="item-tech-news-7"></a>
### [瑞典政府办公室禁用 ChatGPT 与 Claude](https://www.sverigesradio.se/artikel/chat-gpt-och-claude-forbjuder-regeringskansliet) ⭐️ 7.0/10

瑞典政府办公室（Regeringskansliet）自下周起将在员工工作电脑上封禁 ChatGPT 与 Claude，要求改用已获批准的 AI 工具，如微软 Copilot。该部门此前已限制 DeepSeek，理由是未签约的 AI 服务可能危及信息安全。瑞典税务局、国家机构事务局（SiS）已实施类似禁令，Kronofogden 正在评估是否跟进。部分员工仍可通过内部自研平台访问这两款服务。

telegram · zaihuapd · 10月23日 14:11

**「背景」** 瑞典政府办公室此前已对未签约的生成式 AI 服务实施限制，例如去年限制了 DeepSeek，并且税务局和国家机构事务局等其他政府部门也已采取类似封禁措施。此类限制源于对信息安全的担忧，要求使用经批准的 AI 工具如 Microsoft Copilot。

**「影响」** 受限的员工必须迁移至微软 Copilot 等官方批准的工具，这将迫使政府内部的工作流程和文档生成方式进行调整，以符合信息安全要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://madrobot.blog/2026/10/23/sweden-government-offices-block-chatgpt-claude-staff-copilot/">Sweden ’s government blocks ChatGPT and Claude on staff computers</a></li>
<li><a href="https://news.ycombinator.com/item?id=50207405">Swedish government offices to ban ChatGPT and Claude</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#government regulation`, `#AI security`, `#ChatGPT`, `#Claude`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [欧盟取消对中国太阳能玻璃双反关税](https://www.163.com/dy/article/L9R94K6105484D40.html) ⭐️ 7.0/10

欧盟于 10 月 22 日正式取消对中国太阳能玻璃的 84.2%反倾销和反补贴关税，已于 2025 年 7 月起缴纳的关税可申请退还（不计利息）。

telegram · zaihuapd · 10月23日 06:54

**「背景」** 欧盟自 2014 年起对中国太阳能玻璃征收最高 84.2%的反倾销和反补贴关税，理由是保护本土企业，期间该产品在欧盟市场的份额从约 30.5%降至约 3%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://list.solar/news/eu-repeals-solar-glass-duties-china/">Solar Glass Anti-Dumping Duties on China End After 12 Years</a></li>
<li><a href="https://monitorlegal.ro/en/energy/regulation-2026-2310-regulation-2314-repeal-duties-solar-glass-china/">Solar glass from China: EU duties repealed 22 October</a></li>
<li><a href="https://min.news/en/economy/37791710c118db58f79193bfce854a7d.html">After imposing tariffs on Chinese solar glass and engaging in ...</a></li>

</ul>
</details>

**标签**: `#EU trade policy`, `#Solar energy`, `#China‑EU relations`

---