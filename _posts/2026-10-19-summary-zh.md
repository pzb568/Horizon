---
layout: default
title: "Horizon Summary: 2026-10-19 (ZH)"
date: 2026-10-19
lang: zh
---

> 从 34 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [vllm-project/vllm released v0.32.0](#item-tech-news-1) ⭐️ 8.0/10
2. [混合推理代理：在潜在空间思考、文本执行的 LLM 代理](#item-tech-news-2) ⭐️ 8.0/10
3. [Linux 内核 CVE-2026-99999 允许 KVM 客户机逃逸](#item-tech-news-3) ⭐️ 8.0/10
4. [Google 开源递归智能体框架 Harness²](#item-tech-news-4) ⭐️ 8.0/10
5. [Anthropic 游说 AI 安全法案设定高门槛](#item-tech-news-5) ⭐️ 8.0/10
6. [DeepSeek 推出每千次请求 0.75 美元的搜索 API](#item-tech-news-6) ⭐️ 7.0/10
7. [TempoPFN: Synthetic Pre-training of Linear RNNs for Zero-shot Time Series Forecasting \[R\]](#item-tech-news-7) ⭐️ 7.0/10
8. [Proof Before Reuse: showing agents only what later sessions reproduced keeps a poisoned skill out of procedural memory \[R\]](#item-tech-news-8) ⭐️ 7.0/10
9. [Anthropic 与律所合作制定 AI 代理谈判规则](#item-tech-news-9) ⭐️ 7.0/10
10. [英伟达提升 Kimi K3 推理速度 1.68 倍](#item-tech-news-10) ⭐️ 7.0/10

**财经新闻**
1. [医用外骨骼康复训练纳入医保试点](#item-finance-news-1) ⭐️ 8.0/10
2. [外卖平台利润回升，商家与骑手收入受压](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [vllm-project/vllm released v0.32.0](https://github.com/vllm-project/vllm/releases/tag/v0.32.0) ⭐️ 8.0/10

vllm 0.32.0 introduces new API features and wide low‑precision KV‑cache support, delivering important performance and usability improvements for LLM inference.

github · khluu · 10月18日 06:50

**标签**: `#LLM inference`, `#vllm`, `#performance optimization`, `#API updates`

---

<a id="item-tech-news-2"></a>
### [混合推理代理：在潜在空间思考、文本执行的 LLM 代理](https://arxiv.org/abs/2610.18861) ⭐️ 8.0/10

一篇新论文提出了混合推理代理架构，允许大型语言模型在潜在空间中进行推理，同时通过文本接口执行操作。论文附带了开源代码（GitHub togethercomputer/HybridAgent）和在 arXiv 第 5 节中的初步评估，面向 AI 代理工程师提供了可直接使用的实现。

hackernews · allinonai · 10月18日 20:48 · [社区讨论](https://news.ycombinator.com/item?id=50145337)

**「背景」** 大型语言模型（LLM）代理指的是让语言模型在交互式环境中接收指令、生成文本并调用外部工具完成任务的系统。传统的 LLM 代理全部通过文本序列进行推理和行动，而“潜在空间推理”则利用模型内部的向量表示（即隐藏层特征）直接进行计算，以获得更紧凑或更高效的推理过程。将这两者结合的混合架构，使得模型可以在潜在空间中进行复杂的内部推理，然后再将结果转化为文本指令执行外部操作，从而兼具内部计算效率和文本交互的通用性。

**「影响」** 开发者现在可以下载并运行该开源实现，直接在本地实验潜在空间推理与文本交互的组合，从而评估其在特定任务上的效率和表现。

**「社区讨论」** 评论者 amluto 质疑该设计的成本，指出在生成文本时仍需运行完整的潜在模式，建议探索同时在潜在空间和文本模式下并行推理以降低开销。

**标签**: `#LLM agents`, `#latent space reasoning`, `#AI research`, `#agent architectures`

---

<a id="item-tech-news-3"></a>
### [Linux 内核 CVE-2026-99999 允许 KVM 客户机逃逸](http://pwn.ai/) ⭐️ 8.0/10

PWN.AI 安全研究团队披露的 Linux 内核漏洞 CVE-2026-99999 允许在 KVM 环境中，客体（guest）通过改写 IPv4 头部的网络校验和元数据，实现对宿主机内存的 32 字节信息泄露并完成逃逸。该漏洞已于 2026 年 10 月 14 日的补丁合并至主线内核，修复了相关检查逻辑。

telegram · zaihuapd · 10月18日 09:47

**「KVM 虚拟化与网络校验和 offload 漏洞概述」** KVM（Kernel‑Based Virtual Machine）是 Linux 内核提供的虚拟化层，允许在同一台主机上运行多个客体操作系统。该漏洞利用了网络栈中延迟校验和写入的机制：客体可以提供校验和 offload 元数据，使内核在完成校验后仍能改写已验证的 IPv4 头部，从而泄露约 32 字节的主机内存并为代码执行提供入口。此类基于网络校验和的漏洞此前已有研究报道，为本次 CVE‑2026‑99999 的攻击路径提供了技术前提。

**「影响」** 运行受影响内核的云服务提供商和虚拟化平台若未及时升级到包含 2026‑10‑14 补丁的版本，攻击者可利用该缺陷在 KVM 客户机中执行逃逸，危及宿主机安全。建议立即更新至最新内核并检查系统日志以确认未被利用。

<details><summary>参考链接</summary>
<ul>
<li>PwnEscape: Guest-to-Host KVM Escape (CVE-2026-99999) - pwn.ai</li>
<li>PwnEscape Hid in the Kernel Network Stack for 18 Years - TuxCare</li>
<li>PwnEscape Linux Kernel Flaw Lets Guests Escape to Host</li>

</ul>
</details>

**标签**: `#Linux`, `#KVM`, `#Security`, `#Vulnerability`

---

<a id="item-tech-news-4"></a>
### [Google 开源递归智能体框架 Harness²](https://github.com/google-research/harness2) ⭐️ 8.0/10

Google Research releases Harness², a recursive LLM agent framework with performance improvements and open‑source tooling

telegram · zaihuapd · 10月18日 11:24

**标签**: `#LLM`, `#agent-framework`, `#recursive-optimization`, `#open-source`, `#Google-Research`

---

<a id="item-tech-news-5"></a>
### [Anthropic 游说 AI 安全法案设定高门槛](https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropics-proposed-ai-safety-bill-only-kicks-in-if-50-deaths-or-usd1-billion-in-damages-are-on-the-line-proposal-would-effectively-make-the-commerce-department-the-only-agency-capable-of-stopping-an-ai-model) ⭐️ 8.0/10

Anthropic 正在推动一项美国 AI 安全法案草案，规定只有在模型可能导致超过 10 亿美元损失或造成 50 人以上死亡或受伤时，政府才可介入阻止模型发布。该法案要求由商务部登记的独立第三方定期评估实验室和模型，并在发现生物武器、AI 网络攻击或失控风险时于 72 小时内上报。除商务部外，其他联邦机构不得下达叫停指令，最终是否叫停由联邦法官裁决。此为立法提案，尚未成为法律。

telegram · zaihuapd · 10月18日 12:40

**「背景」** 美国近年来已开始制定针对人工智能的安全监管框架，例如 2023 年的《AI 风险管理框架》以及 2024 年的《AI 安全法案》，均将商务部（Department of Commerce）置于对高风险模型的监督角色。Anthropic 提出的新法案在此基础上进一步设定了具体的触发门槛：只有当模型可能导致超过 10 亿美元的损失或造成 50 人以上死亡或受伤时，才允许政府介入并要求停产，且最终的叫停决定只能由商务部指定的独立第三方评估后，由联邦法官裁定。

**「影响」** 如果该法案通过，AI 开发商和部署方将面临更高的合规门槛，需要证明其模型不会触及上述损失或伤亡阈值，并且只能通过商务部的评估程序和联邦法官的裁决来应对潜在的安全风险，这可能增加合规成本并限制其他监管机构的介入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropics-proposed-ai-safety-bill-only-kicks-in-if-50-deaths-or-usd1-billion-in-damages-are-on-the-line-proposal-would-effectively-make-the-commerce-department-the-only-agency-capable-of-stopping-an-ai-model">Anthropic’s proposed AI safety bill only kicks in if 50 ...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#Regulation`, `#Anthropic`, `#Policy`

---

<a id="item-tech-news-6"></a>
### [DeepSeek 推出每千次请求 0.75 美元的搜索 API](https://api-docs.deepseek.com/guides/search/) ⭐️ 7.0/10

DeepSeek 在其 API 文档中宣布推出搜索与抓取服务，计费为每 1,000 次成功请求 0.75 美元，面向构建 AI 驱动搜索或智能体系统的开发者。该价格明显低于目前公开的商业搜索 API，提供了更具成本效益的选项。

hackernews · fagnerbrack · 10月18日 06:50 · [社区讨论](https://news.ycombinator.com/item?id=50138531)

**「背景说明」** DeepSeek 的 Search 与 Fetch API 是面向 AI 代理的 HTTP 接口，分别通过 POST /v1/tools/search 与 POST /v1/tools/fetch 提供网页搜索结果或页面内容。该服务的计费方式为每 1,000 次成功请求 0.75 美元，成功请求指返回 HTTP 200 且搜索返回非空结果数组或页面内容，错误、空结果或超时不计费。

**「影响」** 使用 DeepSeek 搜索 API 的开发者在同等查询量下可比 Brave（约 5 美元/千次）和 Kagi（约 12 美元/千次）等竞争服务节省约 80%‑94% 的费用，从而降低 AI 应用的运营成本。

**「社区讨论」** 评论中有人指出 Brave Search API 约 5 美元/千次、Kagi API 约 12 美元/千次，强调 DeepSeek 的定价更具竞争力；也有用户提到自建如 searxng‑ai‑kit 等免费方案可进一步降低成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://threatfrontier.com/articles/deepseek-search-fetch-api-pricing-october-31">DeepSeek Search and Fetch API Pricing: $0.75 per 1,000</a></li>
<li><a href="https://www.winzheng.com/en/article/deepseek-search-fetch-api-pricing-0-75-per-1000-calls">DeepSeek Search and Fetch API at $0.75 per Thousand Calls ...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/deepseek-monetizes-agent-retrieval-layer-185236272.html?fr=sycsrp_catchall">DeepSeek Monetizes the Agent Retrieval Layer at $0.75 per ...</a></li>

</ul>
</details>

**标签**: `#search API`, `#LLM integration`, `#cost optimization`, `#AI agents`

---

<a id="item-tech-news-7"></a>
### [TempoPFN: Synthetic Pre-training of Linear RNNs for Zero-shot Time Series Forecasting \[R\]](https://www.reddit.com/r/MachineLearning/comments/1x97v19/tempopfn_synthetic_pretraining_of_linear_rnns_for/) ⭐️ 7.0/10

NeurIPS 2026 paper presents a synthetic pre‑training library and linear RNN model for zero‑shot time‑series forecasting, providing a useful new tool for the community.

reddit · r/MachineLearning · /u/Yossarian\_1234 · 10月18日 16:43

**标签**: `#time-series`, `#synthetic-data`, `#linear-RNN`, `#forecasting`, `#machine-learning`

---

<a id="item-tech-news-8"></a>
### [Proof Before Reuse: showing agents only what later sessions reproduced keeps a poisoned skill out of procedural memory \[R\]](https://www.reddit.com/r/MachineLearning/comments/1x975ea/proof_before_reuse_showing_agents_only_what_later/) ⭐️ 7.0/10

A Reddit case study introduces &\#x27;proof before reuse&\#x27; to block poisoned code from entering an agent&\#x27;s procedural memory, showing promising results.

reddit · r/MachineLearning · /u/maa\_\_\_\_z · 10月18日 16:14

**标签**: `#AI safety`, `#code generation`, `#agent memory`, `#machine learning`

---

<a id="item-tech-news-9"></a>
### [Anthropic 与律所合作制定 AI 代理谈判规则](https://www.ft.com/content/f7c26ac0-f5f2-443a-86b2-39d62f7920a9?syn-25a6b1a6=1) ⭐️ 7.0/10

Anthropic 正与律所等法律机构协商，为能够代表用户进行砍价、处理纠纷或薪资谈判的 AI 代理制定谈判规则和监管框架。公司正研究在代理执行前提供用户签署的授权文件，并已在 2026 年 9 月的虚拟书籍交易实验中测试了“无情”模式的 Claude 代理。与此同时，哈佛大学对超过 18 万次 AI 代理谈判的研究显示，新式削弱对手的谈判手法正在出现。此举属于正在进行的治理研究，而非已发布的产品功能。

telegram · zaihuapd · 10月18日 07:07

**「AI 代理谈判的先行实验」** Anthropic 之前在其旧金山办公室进行过内部实验，让 Claude 代理代表员工在内部交易平台上进行谈判；同年又与全球律所 Freshfields（拥有 2,800 多名律师）合作，研究 AI 代理在合同、薪资和客户纠纷等情境下的谈判伦理。此类实验为公司当前与律所共同制定 AI 代理谈判规则提供了实践基础。

**「影响」** 开发 AI 谈判代理的团队需要提前考虑合规要求，包括获取用户授权并遵守即将形成的法律审查规则，否则其系统可能在实际部署时面临合规风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech-insider.org/anthropic-freshfields-ai-agents-legal-deals-2026/">Anthropic Taps 2,800 Lawyers to Watch AI Agent Deals [2026]</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#negotiation`, `#AI policy`, `#legal tech`

---

<a id="item-tech-news-10"></a>
### [英伟达提升 Kimi K3 推理速度 1.68 倍](https://x.com/SemiAnalysis_/status/2111627094878790023) ⭐️ 7.0/10

英伟达在其上游 vLLM 项目中加入了自研解码专用内核和 Megakernel 融合，实现了对 2.8 万亿参数的 Kimi K3 模型的推理加速。在相同硬件上，每用户每秒可生成 423 token，速度提升 1.68 倍。

telegram · zaihuapd · 10月18日 08:20

**「背景」** Kimi K3 是一款拥有 2.8 万亿参数的开源大模型，采用混合专家架构并支持原生视觉输入和最高 100 万 token 的上下文窗口，因其规模和多模态特性，推理计算需求极高。Nvidia 在其上游的 vLLM 推理框架中加入了专用解码内核和 Megakernel 融合，以提升该模型的每用户每秒 token 处理速率。

**「影响」** 对使用 Kimi K3 或类似大模型进行推理的部署者而言，可在同等 GPU 上处理约 68% 更多的 token，从而降低单位推理成本或提升服务并发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.ai/ai-models/kimi-k3">Kimi K3: 2.8T Open Model for Coding &amp; Knowledge Work</a></li>

</ul>
</details>

**标签**: `#inference optimization`, `#vLLM`, `#large language models`, `#Nvidia`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [医用外骨骼康复训练纳入医保试点](https://wap.eastmoney.com/a/202610173899077871.html) ⭐️ 8.0/10

中国北京、上海、江苏、浙江等地区将医用外骨骼康复训练纳入医保或长护险试点，IDC 估计 2025 年该市场规模约 14.2 亿元。

telegram · zaihuapd · 10月18日 10:38

**「背景」** 《全民医疗保障“十五五”规划》已提出将新技术、新药品和新器械纳入商业健康保险，但医用外骨骼此前未被列入医保。

**「影响」** 这将使当地患者的康复费用得到部分报销，推动医用外骨骼设备的需求和销量增长。

**标签**: `#Healthcare policy`, `#Medical devices`, `#Rehabilitation technology`, `#China`

---

<a id="item-finance-news-2"></a>
### [外卖平台利润回升，商家与骑手收入受压](https://www.latepost.com/news/dj_detail?id=3762) ⭐️ 7.0/10

一年后，外卖平台日均订单合计约 1.4 亿单，比战前约 9000 万单增长约 50%，平台销售费用接近战前水平并实现经营利润回升。

telegram · zaihuapd · 10月18日 07:40

**「背景」** 2025 年初，京东推出自营外卖后，Meituan、阿里巴巴的 Ele.me 与其展开大规模补贴竞争，平台销售费用大幅上升。

**「影响」** 补贴停止后，茶饮咖啡等上市公司单店营收和利润普遍下滑，骑手单均收入降至 7‑8.5 元，约比前一年下降约 50%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hellochinatech.com/p/meituan-delivery-war-limits-of-scale">Meituan and the Limits of Scale: China&#x27;s Delivery War Aftermath</a></li>

</ul>
</details>

**标签**: `#Food Delivery`, `#Chinese Market`, `#Platform Economics`, `#Rider Income`, `#Merchant Impact`

---