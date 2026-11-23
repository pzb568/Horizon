---
layout: default
title: "Horizon Summary: 2026-11-23 (ZH)"
date: 2026-11-23
lang: zh
---

> 从 28 条内容中筛选出 3 条重要资讯。

---

**科技新闻**
1. [Windows Server 2028 默认移除 32 位兼容子系统，需手动安装](#item-tech-news-1) ⭐️ 8.0/10
2. [谷歌为 Chrome AI 代理搭建 Mirror Dimension 模拟互联网测试环境](#item-tech-news-2) ⭐️ 7.0/10

**财经新闻**
1. [超级厄尔尼诺海温破纪录，粮食援助受压](#item-finance-news-1) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Windows Server 2028 默认移除 32 位兼容子系统，需手动安装](https://www.windowslatest.com/2026/11/23/32-bit-apps-days-are-numbered-as-microsoft-strips-support-bit-by-bit-starting-with-windows-server-2028-but-windows-11-is-safe-for-now/) ⭐️ 8.0/10

微软在 Ignite 2026 上宣布，Windows Server 2028 将在默认安装中不再包含 WoW64 兼容子系统，导致开箱即无法运行 32 位应用。该版本计划于 2027 年秋季与 Windows 11 27H2 同步发布。需要运行 32 位软件时，管理员可通过按需功能（FoD）使用 PowerShell 或 DISM 手动装回 WoW64。微软称此举旨在缩小攻击面并阻止 32 位恶意软件，而 Windows 11 仍保留 WoW64，暂无移除计划。

telegram · zaihuapd · 11月23日 03:03

**「WoW64 子系统概述」** WoW64（Windows‑on‑Windows 64）是 Windows 64 位系统内置的兼容层，负责在 64 位内核上加载并运行 32 位应用程序。自 Windows Server 2008 起，所有 Windows Server 发行版默认包含该子系统，使得企业在迁移到 64 位平台时仍能保留旧的 32 位业务软件。缺失 WoW64 意味着系统开箱即无法直接执行任何 32 位可执行文件，需要管理员手动通过按需功能（FoD）或 DISM 添加。

**「影响」** 服务器管理员在部署 Windows Server 2028 时必须额外执行 FoD 安装步骤才能支持遗留的 32 位应用，否则需迁移或重写这些应用；未按需装回 WoW64 将导致这些应用直接无法启动。

**标签**: `#Windows Server`, `#32-bit compatibility`, `#system administration`

---

<a id="item-tech-news-2"></a>
### [谷歌为 Chrome AI 代理搭建 Mirror Dimension 模拟互联网测试环境](https://www.landian.news/archives/128701.html) ⭐️ 7.0/10

谷歌在内部搭建了名为 Mirror Dimension 的大规模模拟互联网测试环境，用于安全地验证 Chrome AI 代理的网页打开、搜索、登录、加购和任务完成等功能。该环境包含数千个模拟网站，每位工程师在独立的隔离实例中运行测试，每天执行超过 1000 条测试案例，重点防御恶意网页的提示词注入等攻击。此举是针对 Chrome AI 代理的功能和安全性进行的内部工程测试，而非面向用户的产品发布。

telegram · zaihuapd · 11月23日 01:30

**「背景」** Chrome 正在开发能够在浏览器中自主完成搜索、登录、购物等任务的 AI 代理，这类代理需要直接与网页交互并执行指令。为了在不危及真实网络安全的前提下评估其功能和防御能力，Google 创建了名为 “Mirror Dimension” 的合成互联网环境，在其中模拟数千个网站并运行上千条测试案例，以检测如提示词注入等恶意网页攻击。

**「影响」** Chrome AI 代理的开发团队可以在 Mirror Dimension 中提前发现功能缺陷和安全漏洞，从而在正式发布前提升系统的可靠性和防御能力，相关代码需适配该模拟环境的测试流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wired.com/story/google-built-a-giant-mirror-dimension-internet-to-test-its-chrome-ai-agents/">Google Built a Giant ‘ Mirror Dimension ’ Internet to Test Its Chrome ...</a></li>
<li><a href="https://blog.google/security/mirror-dimension-for-agents/">Mirror Dimension for Agents : Evaluating Browser-Use Agents ...</a></li>

</ul>
</details>

**标签**: `#Chrome`, `#AI agents`, `#Web security`, `#Testing infrastructure`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [超级厄尔尼诺海温破纪录，粮食援助受压](https://www.wired.com/story/how-this-years-super-el-nino-will-worsen-global-hunger/) ⭐️ 8.0/10

截至 10 月，厄尔尼诺中热带太平洋海温升至 3.5℃，创纪录，并预计初冬将达约 4℃；世界粮食计划署警告此现象可能在 2027 年底前额外使 4900 万人陷入急性粮食不安全。

telegram · zaihuapd · 11月22日 14:09

**「背景说明」** El Niño 是通过中热带太平洋海表温度衡量的气候现象，今年已升至约 3.5 °C，远超约 2.75 °C 的历史纪录；联合国世界粮食计划署依据急性粮食不安全人数评估饥饿风险，警告此次升温可能在 2027 年前使额外 4900 万人陷入急性不安全状态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/environment/2026/sep/21/super-el-nino-temperature-record">‘Jaw-dropping’ El Niño bursts through temperature record months...</a></li>
<li><a href="https://www.wired.com/story/how-this-years-super-el-nino-will-worsen-global-hunger/">How This Year’s Super El Niño Will Worsen Global Hunger | WIRED</a></li>

</ul>
</details>

**标签**: `#Climate`, `#Food Security`, `#El Niño`, `#Global Hunger`, `#Economic Impact`

---