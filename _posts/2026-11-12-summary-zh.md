---
layout: default
title: "Horizon Summary: 2026-11-12 (ZH)"
date: 2026-11-12
lang: zh
---

> 从 52 条内容中筛选出 5 条重要资讯。

---

**科技新闻**
1. [GitHub Actions 工作流锁定指南](#item-tech-news-1) ⭐️ 8.0/10
2. [通过电压毛刺解锁 NVIDIA A100 矿卡隐藏显存](#item-tech-news-2) ⭐️ 7.0/10
3. [Operatic AI 发布 CoRL 2100 篇论文浏览器，含 TLDR 与代码链接](#item-tech-news-3) ⭐️ 7.0/10
4. [AMD AI 内存换页技术声称可削减服务器成本至 83%](#item-tech-news-4) ⭐️ 7.0/10

**财经新闻**
1. [阿里巴巴计划在香港上市 AI 芯片子公司 T‑Head](#item-finance-news-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GitHub Actions 工作流锁定指南](https://hugovk.dev/blog/2026/lock-github-actions/) ⭐️ 8.0/10

本文提供了在 GitHub Actions 中使用工作流锁文件（通过提交 SHA 锁定动作）来提升 CI/CD 安全性的实用步骤。该方法可防止动作在未显式更新时被篡改，但目前仅对普通动作调用生效，对可复用工作流和复合动作没有直接锁定，需要手动对其进行哈希固定。

hackernews · gslin · 11月11日 22:16 · [社区讨论](https://news.ycombinator.com/item?id=50459485)

**「背景」** GitHub Actions 在 2026 年 10 月推出工作流锁文件（workflow lockfiles）功能，先在公开预览（10 月 14 日）后于 10 月 28 日正式发布。锁文件会在工作流中记录每个使用的 Action 的确切 SHA，取代过去手动在 YAML 中自行 pin 到 commit 哈希的做法，以防止标签可变导致的供应链攻击。

**「影响」** 开发者在工作流中使用锁文件后，可显著降低供应链攻击风险，但必须额外检查并手动锁定可复用工作流和复合动作的版本，以确保完整的安全覆盖。

**「社区讨论」** 评论者 woodruffw 指出，当前的工作流锁文件只能锁定普通动作调用，若工作流调用可复用工作流或使用复合动作，则需自行对这些组件的哈希进行固定，否则仍可能存在风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-10-14-github-actions-workflow-lockfiles-in-public-preview/">GitHub Actions workflow lockfiles in public preview</a></li>
<li><a href="https://github.blog/changelog/2026-10-28-github-actions-workflow-lockfiles-are-generally-available/">GitHub Actions workflow lockfiles are generally available</a></li>

</ul>
</details>

**标签**: `#GitHub Actions`, `#CI/CD`, `#Security`, `#DevOps`

---

<a id="item-tech-news-2"></a>
### [通过电压毛刺解锁 NVIDIA A100 矿卡隐藏显存](https://blog.kate.land/posts/using-voltage-glitching-to-unlock-the-a100/) ⭐️ 7.0/10

作者展示了一种对 NVIDIA A100 矿卡进行电压毛刺（voltage‑glitching）的方法，可解除芯片上用于限制的熔断器，从而将原本仅可用的 8 GB 显存解锁为完整的 80 GB HBM。该 hack 仅在特定的 8 GB 采矿版 A100 上验证，属于硬件层面的改造，未经过 NVIDIA 官方确认。

hackernews · lae · 11月11日 10:48 · [社区讨论](https://news.ycombinator.com/item?id=50451903)

**「背景」** NVIDIA 为降低良率风险，在面向加密挖矿的 A100 卡上通过熔断保险丝关闭了部分 SM 核心和显存，使其仅启用约 108 个 SM；而通过电压冲击（voltage glitch）等故障注入手段可以在极低电压下触发保险丝熔断，从而解锁全部 SM（约 120‑126）并恢复全部显存，提升约 1.2 倍的计算性能。电压冲击是一种通过瞬时降低供电电压使芯片内部状态异常的硬件攻击技术，常用于研究或破解硬件限制。

**「影响」** 成功解锁后，用户可在同等硬件成本下获得约十倍的显存容量，显著降低 AI/机器学习工作负载的算力成本，但该操作需要精确的电压脉冲并存在永久损坏卡片的风险，适合有硬件经验的少数爱好者。

**「社区讨论」** 评论中有人对能够“打开”80 GB HBM 表示惊讶并计划尝试，也有用户担心熔断器可能是为掩盖制造缺陷而设，且强调此类改造风险高且需要专业知识。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.kate.land/posts/using-voltage-glitching-to-unlock-the-a100/">Using voltage glitching to unleash the A 100 in my mining card</a></li>
<li><a href="https://www.youtube.com/watch?v=16UcoPLdXD4">Glitching and Fault Injection: Finding the Right Voltage - YouTube</a></li>

</ul>
</details>

**标签**: `#GPU`, `#Hardware Hacking`, `#AI Compute`, `#NVIDIA`, `#Memory Unlock`

---

<a id="item-tech-news-3"></a>
### [Operatic AI 发布 CoRL 2100 篇论文浏览器，含 TLDR 与代码链接](https://www.reddit.com/r/MachineLearning/comments/1xtul3j/i_built_an_explorer_of_2100_robotics_papers/) ⭐️ 7.0/10

一个开源的网页工具现已上线，索引了 2017 至 2026 年间的 2100 余篇 CoRL 机器人学习论文。该浏览器在 https://corl.operatic.ai/explore 提供每篇论文的 TLDR 摘要、项目页面、代码仓库、arXiv 链接以及任务标签和统计趋势。源码托管于 GitHub（https://github.com/operatic-ai/corl-explorer），欢迎提交 PR 添加功能或纠错。此工具旨在让机器人学习研究更易检索和分析。

reddit · r/MachineLearning · /u/promptdom · 11月11日 21:42

**「CoRL 会议概述」** CoRL（Conference on Robot Learning）是每年举办的国际会议，聚焦机器人技术与机器学习的交叉研究，自 2017 年起持续发布大量论文。由于这些论文分散在不同的会议记录和预印本平台，研究者往往难以系统检索和比较。该背景说明了建立统一论文浏览工具的需求。

**「影响」** 研究人员可通过该平台快速查找相关工作、获取实现代码并观察研究热点趋势，从而加速文献调研和项目开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.corl.org/">CoRL 2026</a></li>

</ul>
</details>

**标签**: `#robotics`, `#research-tools`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [AMD AI 内存换页技术声称可削减服务器成本至 83%](https://www.theregister.com/systems/2026/11/11/amd-where-were-going-we-dont-need-as-much-dram/5308953) ⭐️ 7.0/10

AMD 将收购的 Mext 技术包装成软件，使用 AI 模型在操作系统或应用感知之前，将内存页面在 DRAM 与更便宜的 NVMe 闪存之间进行换入换出。AMD 声称，用闪存替代一半的 DRAM 可保持最高 99% 的性能，并估算最高可将企业服务器成本降低 83%，该方案需在购买 EPYC 服务器时额外购买 Mext 授权。

telegram · zaihuapd · 11月11日 11:15

**「背景」** AMD 的 MEXT（Memory Extension）是一套软件方案，利用 AI 将低成本的大容量 NVMe 闪存模拟为 DRAM‑速度的内存，以在操作系统或应用感知之前在两者之间预测性地换页。该技术延续了业界已有的内存层次化思路，但通过 AI 预测提升了换页效率，使得在 EPYC 服务器上可显著降低对昂贵 DRAM 的依赖。

**「影响」** 服务器采购者若采用该方案，需要为 EPYC 服务器额外购买 Mext 授权，但可通过减少 DRAM 容量实现显著的成本节约，实际节省幅度取决于工作负载对冷数据的访问频率和 AI 换页模型的有效性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.amd.com/en/products/software/mext.html">AMD MEXT Predictive Memory Software</a></li>

</ul>
</details>

**标签**: `#hardware`, `#systems`, `#AI`, `#cloud‑infrastructure`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [阿里巴巴计划在香港上市 AI 芯片子公司 T‑Head](https://www.cnbc.com/2026/11/11/alibaba-pr.html) ⭐️ 7.0/10

阿里巴巴宣布将在香港证券交易所进行子公司 T‑Head 的分拆上市，上市计划需经交易所和中国证监会批准。

rss · CNBC Finance · 11月11日 07:47

**「背景」** 该公司正加速自主研发 AI 芯片，以应对美国对中国芯片供应的限制。

**标签**: `#Alibaba`, `#Semiconductor IPO`, `#AI chips`, `#Hong Kong market`, `#Chinese tech sector`

---