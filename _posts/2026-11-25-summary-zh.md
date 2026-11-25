---
layout: default
title: "Horizon Summary: 2026-11-25 (ZH)"
date: 2026-11-25
lang: zh
---

> 从 27 条内容中筛选出 8 条重要资讯。

---

**科技新闻**
1. [矩阵乘法指数降至 9/4 的新预印本](#item-tech-news-1) ⭐️ 8.0/10
2. [VMware vCenter 再曝 9.8 严重免鉴权漏洞](#item-tech-news-2) ⭐️ 8.0/10
3. [Ternary Bonsai 2.5 27B 模型发布，支持 128k 上下文](#item-tech-news-3) ⭐️ 7.0/10
4. [T3 Code 默认开启遥测并收集本机 Codex 与 Claude 凭证](#item-tech-news-4) ⭐️ 7.0/10
5. [SpaceX 放弃 7.38 亿美元联邦宽带补贴，改为免费提供星链终端](#item-tech-news-5) ⭐️ 7.0/10
6. [OpenAI 将网络安全定位为新增长引擎，推出 GPT‑6 Cyber 并扩大 Daybreak 计划](#item-tech-news-6) ⭐️ 7.0/10

**财经新闻**
1. [小米三季度净利润大幅下滑，交付 10 万辆新能源汽车](#item-finance-news-1) ⭐️ 8.0/10
2. [黄仁勋复职引发英伟达股价上扬](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [矩阵乘法指数降至 9/4 的新预印本](https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf) ⭐️ 8.0/10

OpenAI 的 math 仓库发布了一篇预印本，声称已证明矩阵乘法的指数等于 9/4，即 Θ\(n^2.25\)，并在所有域上成立。该声明尚未经过同行评审或独立验证，属于理论层面的突破。若成立，将把已知的上界提升至与下界相同的 2.25。当前尚未提供可实际使用的实现。

hackernews · E-Reverance · 11月25日 01:19 · [社区讨论](https://news.ycombinator.com/item?id=50637220)

**「矩阵乘法指数概念」** 矩阵乘法指数 ω 是指能够在 O\(n^ω\) 时间内完成 n×n 矩阵乘法的最小可能指数。该概念源自把矩阵乘法视为一种可通过分治和张量分解加速的运算，历史上已知的上界约为 2.37（由 Le Gall 等人在 2010‑2020 年间逐步改进），而已知的下界仅为 2。因而任何将上界推至 2.25（即 Θ\(n^\{2.25\}\)）的声明，都意味着相较于已有理论的显著突破。

**「影响」** 若该指数确凿无误，理论上大规模线性代数运算的渐进复杂度将下降，可能在极大规模的 AI 训练或科学计算中带来潜在的性能提升，但由于缺乏实用算法，短期内对实际系统的影响有限。

**「社区讨论」** 评论者 orlp 指出标题应为 Θ\(n^2.25\) 而非 O\(n^2.25\)；brandonb 说明论文仅证明了 Ω\(n^2.25\) 的下界，上界 2.25 已经存在，且已有一篇实现 O\(n^2.25\) 的算法但仍不可实用。

**标签**: `#algorithms`, `#theoretical-computer-science`, `#matrix-multiplication`, `#AI-infrastructure`

---

<a id="item-tech-news-2"></a>
### [VMware vCenter 再曝 9.8 严重免鉴权漏洞](https://thehackernews.com/2026/11/vmware-vcenter-hit-by-another-critical.html) ⭐️ 8.0/10

Broadcom 为 VMware 产品线发布的补丁中修复了 vCenter 目录服务（vmdir）的认证绕过漏洞 CVE‑2026‑123903，严重程度评分 9.8。只要能够访问受影响的 vCenter 实例，攻击者即可绕过身份验证直接进入系统。该漏洞在数日前已被零日利用，现已公开披露。

telegram · zaihuapd · 11月24日 14:50

**「背景说明」** VMware vCenter 是用于集中管理虚拟机和 ESXi 主机的核心平台，企业和云环境普遍依赖其目录服务 \(vmdir\) 进行身份验证。若出现鉴权绕过漏洞，攻击者只要能够访问 vCenter 服务器，就能在无需登录的情况下直接获取管理权限，导致整个虚拟化基础设施被完全控制。此次披露的 CVE‑2026‑123903 属于此类高危绕过漏洞，属于 Broadcom 为 VMware 产品线一次性修复的 23 项安全缺陷之一。

**「影响」** 受影响的企业和云环境必须尽快部署 Broadcom 提供的补丁，否则攻击者可在未认证的情况下完全控制 vCenter，导致数据泄露和服务中断。

**标签**: `#security`, `#vulnerability`, `#VMware`, `#vCenter`, `#enterprise`

---

<a id="item-tech-news-3"></a>
### [Ternary Bonsai 2.5 27B 模型发布，支持 128k 上下文](https://prismml.com/news/bonsai-2-5-27b) ⭐️ 7.0/10

PrismML 于 2026‑11‑24 推出 27 B 参数的 Ternary Bonsai 2.5 模型（Q2 GGUF 量化），在本地可实现约 128 k 上下文长度。实测在 Mac Mini M5 Pro 上，提示阶段可达 222.9 token/s，生成阶段约 22‑25 token/s，整体表现优于同尺寸的多数开源模型，尤其适合需要长上下文的 agentic 编码任务。

hackernews · b0m · 11月24日 20:08 · [社区讨论](https://news.ycombinator.com/item?id=50633922)

**「背景」** Ternary Bonsai 2.5 采用三元量化技术，将 27 B 参数模型压缩至约 8.6 GB 左右的体积，同时保持约 98% 的 FP16 基准性能，这使得大模型在本地机器上运行成为可能。此前的 Bonsai 2 已经展示了在 5.9 GB 规模下的强劲表现，2.5 版在此基础上进一步提升了对多轮工具使用和代理式编码任务的能力。

**「影响」** 开发者和 AI 工程师现在可以在消费级硬件上运行高达 128 k 上下文的 LLM，省去云端调用成本，直接在本地完成复杂的代码生成和多步代理任务。

**「社区讨论」** 用户 ariwilson 报告称在 Mac Mini M5 Pro 上运行该模型时，提示阶段 222.9 token/s、生成阶段约 22.3 token/s，且能够轻松保持 128 k 上下文，验证了其在本地高效长上下文推理的实际可用性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://prismml.com/news/bonsai-2-5-27b">PrismML — Introducing Ternary Bonsai 2 . 5 27 B : Powering Agentic...</a></li>
<li><a href="https://www.mindstudio.ai/blog/ternary-bonsai-2-27b-ternary-quantization">Ternary - Bonsai - 2 - 27 B : A 27 B Model That Fits in 8.6GB | MindStudio</a></li>

</ul>
</details>

**标签**: `#large-language-models`, `#model-quantization`, `#agentic-coding`, `#benchmarking`

---

<a id="item-tech-news-4"></a>
### [T3 Code 默认开启遥测并收集本机 Codex 与 Claude 凭证](https://x.com/realchendahuang/status/2125153472450527440) ⭐️ 7.0/10

开发者报告称 Theo 的 T3 Code 自 2023 年 3 月合并 PR \#174 起默认启用 PostHog 遥测，并在 2025 年 10 月合并的 PR \#21506 中读取本机的 ~/.codex/auth.json 与 ~/.claude.json，提取 Codex 的 user\_id、Claude 的 accountUuid 与设备 ID，进行无盐 SHA‑256 哈希后上传。官方文档承认浏览器和移动端的中继诊断追踪无法关闭，且四个关闭遥测的 PR 均被拒绝。项目方和 Theo 未作回应。

telegram · zaihuapd · 11月24日 10:58

**「背景说明」** PostHog 是一种开源分析平台，常用于在应用中收集事件遥测，官方文档说明其可通过项目设置发送用户行为数据 \(参见 tool-1-1\)。Codex 的本地身份验证信息保存在用户主目录下的 \`~/.codex/auth.json\`，该文件包含 \`user\_id\` 等字段，可通过头部登录方式获取 \(见 tool-1-2\)。因此，若开发工具在未明确告知的情况下读取这些文件并将哈希值上报，就涉及对已知的本地凭证文件的访问。

**「影响」** 开发者的本地身份凭证可能被远程收集，即使经过哈希仍可能被用于追踪或关联用户行为，建议受影响的用户审查并手动禁用 T3 Code 的遥测或改用不读取凭证的替代工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://posthog.com/docs/workflows/supabase-auth-emails">Send Supabase auth emails with PostHog - Docs - PostHog</a></li>
<li><a href="https://blog.laozhang.ai/en/posts/codex-headless-login">Codex Headless Login: Device Code , SSH Tunnel, or auth . json</a></li>

</ul>
</details>

**标签**: `#telemetry`, `#privacy`, `#AI-tools`, `#developer-tools`

---

<a id="item-tech-news-5"></a>
### [SpaceX 放弃 7.38 亿美元联邦宽带补贴，改为免费提供星链终端](https://x.com/SawyerMerritt/status/2125314062997467640) ⭐️ 7.0/10

SpaceX 同意放弃 7.38 亿美元的美国联邦宽带补贴（BEAD 计划），改为向符合条件的美国家庭免费提供星链终端设备。根据零支出协议，SpaceX 必须保证至少 100 Mbps 下载、20 Mbps 上传的速率，提供低价月费套餐，并承诺服务期限 10 年，且需遵守与其他 BEAD 受资助方相同的交付时间表和性能测试。作为交换，SpaceX 可免除大部分财务审计、采购和行政报告义务，但仍须接受网络性能测试。

telegram · zaihuapd · 11月25日 02:17

**「BEAD 计划与星链背景」** 美国国家电信与信息管理局（NTIA）在 2022 年启动的宽带公平、可及与部署（BEAD）计划，向符合条件的运营商提供联邦补贴，以在未覆盖地区部署高速宽带。SpaceX 通过其星链卫星互联网服务已在美国提供宽带，并在此前通过 FCC 获得许可在国内提供卫星宽带服务。

**「影响」** 符合条件的美国家庭将无需支付星链终端费用，降低了接入高速宽带的门槛，预计将加速 Starlink 在美国的用户增长；同时，SpaceX 通过免除审计等行政负担，能够将资源更多投入网络建设和运营。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.m.wikipedia.org/wiki/SpaceX">SpaceX - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Broadband`, `#Starlink`, `#Telecom Infrastructure`, `#Hardware`

---

<a id="item-tech-news-6"></a>
### [OpenAI 将网络安全定位为新增长引擎，推出 GPT‑6 Cyber 并扩大 Daybreak 计划](https://www.theinformation.com/newsletters/ai-agenda/openais-roadmap-making-cyber-bigger-coding-remains-blurry) ⭐️ 7.0/10

OpenAI 宣称网络安全市场规模超过 3000 亿美元，并将其视为可能超过编程业务的增长引擎。公司已发布面向安全研究的 GPT‑6 Cyber，并将“网络安全受信访问”计划（Daybreak）扩展至数千名已验证的防御者和约 2000 家获批组织与工作空间，支持漏洞发现、代码库分析和二进制逆向。OpenAI CFO 与总裁均强调该领域的商业潜力，但对与 Anthropic、Google 的竞争以及规模化商业化路径未给出明确说明。

telegram · zaihuapd · 11月25日 04:51

**「先前的安全研发与 Daybreak 计划」** OpenAI 之前已推出基于 GPT‑5 的安全研究工具 Aardvark，旨在自动分析代码库以发现漏洞，并通过 Daybreak 计划向经过验证的防御者提供受信访问权限。该计划截至去年已覆盖数千名安全研究员和约 2000 家获批组织，为后续的 GPT‑6 Cyber 打下了技术和合作基础。

**「影响」** 已获批准的组织可通过 Daybreak 计划使用 GPT‑6 Cyber 进行漏洞检测和逆向分析，需完成身份验证后方可接入，从而提升其安全研发效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/dmavik_ai-cybersecurity-openai-activity-7390029689106386944-uwvH">OpenAI &#x27;s Aardvark: AI&#x27;s role in cybersecurity and marketing | LinkedIn</a></li>

</ul>
</details>

**标签**: `#AI security`, `#OpenAI`, `#Cybersecurity`, `#Industry news`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [小米三季度净利润大幅下滑，交付 10 万辆新能源汽车](https://ir.mi.com/static-files/3d372aaa-8ff8-4e33-ba01-68c8d7975a0b) ⭐️ 8.0/10

小米集团 2026 年第三季度经调整净利润为 48.84 亿元，同比下降 56.8%，略高于市场预期的 47.46 亿元。

telegram · zaihuapd · 11月24日 10:09

**「背景说明」** 小米集团是一家以智能手机为主、并在 2025 年启动小米汽车业务的中国科技公司，2026 年第三季度受芯片涨价和研发投入增加影响，导致净利润同比下降 56.8%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Xiaomi">Xiaomi - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Xiaomi`, `#Earnings`, `#Electric Vehicles`, `#Smartphones`, `#China`

---

<a id="item-finance-news-2"></a>
### [黄仁勋复职引发英伟达股价上扬](https://www.cnbc.com/2026/11/25/jensen-huang-nvidia-ai-talent-race.html) ⭐️ 7.0/10

Jensen Huang 在 11 月 23 日复职为英伟达 CEO，导致公司股价在消息公布后出现上涨。

rss · CNBC Finance · 11月25日 01:13

**「背景」** 黄于 11 月 12 日因丑闻辞职，11 天后即 11 月 23 日复职；与此同时，根据卡内基研究，中国在 2025 年已以 41%对美国的 34%超越美国在全球 AI 研究人员的占比，凸显人才竞争。

**「影响」** 英伟达股价的上涨直接惠及持股投资者。

<details><summary>参考链接</summary>
<ul>
<li>China Surpasses U.S. in Global AI Researcher Presence - Aju Press AMP</li>
<li><a href="https://engoo.com/app/daily-news/article/jensen-huang-reinstated-as-nvidia-ceo/OOvrJuf4EfGQy7tn60ZxRQ">Jensen Huang Reinstated as Nvidia CEO | Engoo Daily News</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#AI talent`, `#US‑China tech rivalry`, `#Executive turnover`

---