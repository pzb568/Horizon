---
layout: default
title: "Horizon Summary: 2026-11-19 (ZH)"
date: 2026-11-19
lang: zh
---

> 从 44 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [Quad9 因法国 DNS 封锁法退出法国](#item-tech-news-1) ⭐️ 8.0/10
2. [curl 重写为 Rust：已转换 185k 行 C 代码并修复 200+ Bug](#item-tech-news-2) ⭐️ 8.0/10
3. [Xint 披露 5 个可导致 root 的 NGINX 漏洞](#item-tech-news-3) ⭐️ 8.0/10
4. [Google DeepMind 发布 Genie 4，面向 AI Ultra 订阅者开放](#item-tech-news-4) ⭐️ 7.0/10
5. [DaisyRose-27B 开源 27B 参数模型发布](#item-tech-news-5) ⭐️ 7.0/10
6. [OpenAI 模型用于芯片设计自动化](#item-tech-news-6) ⭐️ 7.0/10
7. [Anthropic 推出 Claude API 关联计费测试版](#item-tech-news-7) ⭐️ 7.0/10
8. [DeepSeek 将服务端搜索和网页抓取改为免费，仅按模型 Token 计费](#item-tech-news-8) ⭐️ 7.0/10
9. [酷态科 10 Ultra 充电头固件缺陷可能输出 20V 导致外设损坏](#item-tech-news-9) ⭐️ 7.0/10
10. [美政府拟要求企业披露使用中国 AI 模型](#item-tech-news-10) ⭐️ 7.0/10

**财经新闻**
1. [美联储官员沃勒称可能需加息 0.5 个百分点](#item-finance-news-1) ⭐️ 8.0/10
2. [腾讯 2026 年 Q3 营收与资本开支超预期](#item-finance-news-2) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Quad9 因法国 DNS 封锁法退出法国](https://techstackups.com/articles/quad9-leaves-france-dns-blocking/) ⭐️ 8.0/10

Quad9 宣布因法国新通过的 DNS 封锁法而撤出法国市场，停止在法国提供其公共 DNS 解析服务。该法律要求 DNS 解析器对涉嫌侵权的域名进行过滤，Quad9 认为这与其不记录用户查询、注重隐私和安全的运营原则冲突。退出意味着法国用户将不再能够使用 Quad9 的 9.9.9.9 DNS 服务器。

hackernews · ritzaco · 11月18日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=50545958)

**「DNS 解析器与法国强制域名封锁的背景」** Quad9 是一家提供基于安全过滤的公共 DNS 解析服务的非营利组织，用户通过它查询域名时可获得恶意站点拦截。法国于 2026 年通过一项法律，要求所有公共 DNS 解析器在法国境内对特定版权内容（如 beIN Sports 的流媒体）实施域名封锁。此前，Quad9 在德国因 Sony Music 案件采用 GeoIP 屏蔽而被法院认定未遵守类似要求并受到罚款，这为其在法国的法律争议埋下伏笔。

**「影响」** 法国用户需要切换到其他公共 DNS（如 Cloudflare 1.1.1.1 或 Google 8.8.8.8），否则将失去 Quad9 提供的恶意软件和钓鱼防护。

**「社区讨论」** 评论者 trentnix 认为，利用 DNS 解析器来打击盗版实际上是政府压制不喜欢内容的后门。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techstackups.com/articles/quad9-leaves-france-dns-blocking/">Quad 9 Is Leaving France : Why DNS Resolvers Are... | Tech Stackups</a></li>
<li><a href="https://blog.cloudflare.com/quad9-withdrawal-from-france/">Quad 9 ’s withdrawal from France : A canary in the... | Cloudflare Blog</a></li>

</ul>
</details>

**标签**: `#DNS`, `#Internet Policy`, `#Security`

---

<a id="item-tech-news-2"></a>
### [curl 重写为 Rust：已转换 185k 行 C 代码并修复 200+ Bug](https://simonwillison.net/2026/Nov/18/daniel-stenberg/) ⭐️ 8.0/10

在大约三周的时间里，自动化代理将 curl 项目中约 185,000 行 C 代码转换为 340,000 行 Rust 代码，并在此期间合并了 300 多次提交。期间实际修复了 200 多个 bug 并修补了若干安全漏洞。该工作已在 curl 主仓库中完成，而不是仅仅是计划或预览。

rss · Simon Willison · 11月18日 15:58

**「curl 项目与 Rust 重写尝试的背景」** curl 是一个用 C 实现的广泛使用的命令行工具和库，负责在网络上进行数据传输。近期出现了使用 AI 代理将 curl 的约 185,000 行 C 代码转换为约 340,000 行 Rust 代码的尝试，但官方 curl 项目仍在持续合并上游提交并修复漏洞和 bug。

**「影响」** 由于这些 bug 修复和安全补丁已合并到主代码库，使用 curl 的开发者将立即受益于更稳定、更安全的行为，并可在未来的 Rust 实现中获得这些改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/daniel-stenberg-curl-rust-agent-rewrites-vs-maintenance-november-2026">curl vs Rust Rewrites: 200 Fixes Agents Missed | explainx.ai Blog</a></li>
<li><a href="https://daniel.haxx.se/blog/2026/11/17/actual-curl-rewrites-in-rust/">Actual curl rewrites in rust - daniel.haxx.se</a></li>

</ul>
</details>

**标签**: `#curl`, `#rust`, `#security`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [Xint 披露 5 个可导致 root 的 NGINX 漏洞](https://nginx2root.com/) ⭐️ 8.0/10

Xint 公布了 5 项 NGINX 漏洞和一个 Linux 内核缺陷，组合后可实现从 NGINX 访客获取主机 root 权限。其中 CVE‑2026‑123007 为 HTTP/2 流控内存破坏，未认证即可在 worker 进程中执行命令。NGINX 1.30.7 与 1.31.9 已于 11 月 18 日发布修复，覆盖 10 个 CVE，Rapid7 已提供 PoC，当前暂无野外利用报告。若无法立即升级，建议关闭对外的 HTTP/2 功能以降低风险。

telegram · zaihuapd · 11月18日 16:21

**「背景说明」** NGINX 是广泛部署的高性能 Web 服务器和反向代理。HTTP/2 实现中的流控计数错误会导致内存复制异常，进而触发未认证的远程代码执行（CVE‑2026‑123007），该漏洞已被 Ubuntu 安全公告记录并由 Rapid7 与 Wiz 报告为整数下溢导致的 worker 进程 RCE。

**「影响」** 受影响的服务器管理员必须在 11 月 18 日后升级到 NGINX 1.30.7 或 1.31.9，或在无法升级的情况下禁用 HTTP/2，以防止远程攻击者获取 root 权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ubuntu.com/security/CVE-2026-123007">CVE - 2026 - 123007 | Ubuntu</a></li>
<li><a href="https://www.rapid7.com/blog/post/ve-cve-2026-123007-critical-nginx-http-2-integer-underflow-leads-to-rce-fixed/">Rapid7 discloses a critical vulnerability affecting NGINX HTTP / 2 that...</a></li>
<li><a href="https://www.wiz.io/blog/nginx-http2-rce-vulnerabilities">Unauthenticated Remote Code Execution in NGINX ... | Wiz Blog</a></li>

</ul>
</details>

**标签**: `#security`, `#nginx`, `#vulnerability`, `#linux`, `#devops`

---

<a id="item-tech-news-4"></a>
### [Google DeepMind 发布 Genie 4，面向 AI Ultra 订阅者开放](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/genie-4-now-available-project-genie/) ⭐️ 7.0/10

Google DeepMind 宣布 Genie 4 已正式上线，当前仅对符合条件的 Google AI Ultra 订阅者开放使用。官方未提供模型的具体规模、性能或功能细节，仅说明该版本已可供符合资格的用户访问。

hackernews · leumon · 11月18日 18:49 · [社区讨论](https://news.ycombinator.com/item?id=50550415)

**「背景」** Genie 系列是 Google DeepMind 开发的交互式世界模型，能够通过文本和图像提示实时生成并编辑逼真的三维场景。Project Genie 是 Google 为其 AI Ultra 订阅者提供的界面，允许这些用户在云端使用该模型进行实时音频和编辑操作。

**「影响」** 开发者若持有符合条件的 AI Ultra 订阅，可在 Google 平台上尝试 Genie 4；未订阅或不在支持地区的用户仍无法使用，需要先获取相应订阅或等待后续开放。

**「社区讨论」** 评论者 kingrolo 反馈，Google 对 Genie 4 的付费方式和可用地区说明不够明确，导致其在工作区账户和个人 Gmail 账户之间出现访问差异。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/genie/">Genie 4 — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/genie-4-now-available-project-genie/">Project Genie update featuring Genie 4</a></li>

</ul>
</details>

**标签**: `#AI`, `#Large Language Models`, `#Google DeepMind`, `#Model Release`

---

<a id="item-tech-news-5"></a>
### [DaisyRose-27B 开源 27B 参数模型发布](https://www.radixark.com/blog/daisyrose-27b) ⭐️ 7.0/10

RadixArk 在 2026 年 11 月发布了 DaisyRose-27B，一款拥有 27 十亿参数的开源大语言模型。该模型在 144 块 NVIDIA H200 GPU 上完成训练，训练时长约 18 天。模型已在 HuggingFace 上公开，可供社区直接下载和使用。

hackernews · de\_sty · 11月18日 19:39 · [社区讨论](https://news.ycombinator.com/item?id=50551046)

**「背景」** DaisyRose-27B 是在 Qwen3.8‑27B（阿里巴巴开源的 27 B 参数语言模型）基础上，使用 RadixArk 自研的 Miles 强化学习框架进行后训练的模型。该项目在 1,200 条精心挑选的长时序任务上进行训练，耗时 18 天，使用了 144 块 Nvidia H200 GPU，展示了大规模后训练在硬件资源和任务规模上的需求。

**「影响」** AI 开发者现在可以免费获取一个规模相当于商用 27 B 参数模型的参考实现，并据此评估在类似硬件配置下的训练成本与推理性能。

**「社区讨论」** 评论者 xlayn 指出当前尚未提供 GGUF 格式下载，需等待社区转换后才能更方便地在轻量化环境中测试；同时他对 144 块 H200 GPU 的训练需求感到惊讶，强调了大模型训练的硬件门槛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.radixark.com/blog/daisyrose-27b">DaisyRose-27B: Pushing the Frontier of Post-Training Efficiency</a></li>

</ul>
</details>

**标签**: `#large-language-models`, `#open-source`, `#hardware`, `#model-training`, `#AI-research`

---

<a id="item-tech-news-6"></a>
### [OpenAI 模型用于芯片设计自动化](https://openai.com/index/advancing-chip-design-with-our-models/) ⭐️ 7.0/10

OpenAI 在其博客中宣布，正将其大型语言模型用于芯片设计工作流，帮助自动生成 RTL 代码、编写 EDA 脚本并监控长时间仿真，以提升设计效率。该功能目前以内部演示形式发布，尚未对外提供具体模型名称或公开 API。

hackernews · vighneshiyer · 11月18日 17:45 · [社区讨论](https://news.ycombinator.com/item?id=50549493)

**「AI 在芯片设计中的前置技术」** 在 OpenAI 之前的模型（如 GPT‑4）已被用于辅助硬件描述语言（HDL）编写和初步的电路布局优化，帮助工程师加速设计流程。最新的 GPT‑6 Astra 在 OpenAI 的 Jalapeño 项目中进一步提升了电路优化和 RISC‑V 核心设计的自动化程度，展示了 AI 辅助芯片设计的进展。

**「影响」** 芯片设计团队可以尝试使用 OpenAI 的模型来自动化部分设计和仿真任务，从而减少手工编写脚本和监控仿真的时间成本。

**「社区讨论」** 一位评论者（skyberrys）分享称，他将芯片设计视为软件设计问题，使用模型生成电路代码并自动化 EDA 流程，成功让模型负责多小时的仿真运行，提升了工作效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/advancing-chip-design-with-our-models/">Advancing chip design with OpenAI models | OpenAI</a></li>

</ul>
</details>

**标签**: `#chip design`, `#AI for hardware`, `#OpenAI`, `#EDA`, `#RISC-V`

---

<a id="item-tech-news-7"></a>
### [Anthropic 推出 Claude API 关联计费测试版](https://thenextweb.com/news/anthropic-linked-billing-claude-api-customers-pay) ⭐️ 7.0/10

Anthropic 为 Claude API 推出关联计费测试版，允许直接向 Anthropic 付费的组织将 API 使用量计入其自身的 Claude 组织账户，并可设置月度支出上限或随时解除关联。计费失败时请求将被拒绝，不会转由开发者承担费用。该功能仅适用于直接付费的组织，不支持通过 AWS、Google Cloud、Azure 结算或仅订阅的用户；此外，零数据留存和 HIPAA 等合规保护不适用于这些请求。

telegram · zaihuapd · 11月18日 07:24

**「关联计费概念」** Claude 是 Anthropic 提供的对话式大模型，开发者通过 Claude API 调用时通常由 Anthropic 账户统一计费。关联计费（Linked billing）是一种计费模式，允许使用 Claude API 的客户将使用费用直接计入其在 Anthropic 平台创建的组织账户，并可自行设置月度支出上限或随时解除绑定。此功能仅面向直接向 Anthropic 付款的组织，不适用于通过 AWS、Google Cloud、Azure 结算或仅订阅的用户。

**「影响」** 使用该计费模式的开发者需要在 Anthropic 组织中配置关联计费并设定支出上限，否则在超过上限或计费失败时其 API 调用将被阻断，必须提前管理成本和计费设置。

**标签**: `#AI`, `#APIs`, `#Billing`, `#Anthropic`, `#Claude`

---

<a id="item-tech-news-8"></a>
### [DeepSeek 将服务端搜索和网页抓取改为免费，仅按模型 Token 计费](https://www.ithome.com/1/029/058.htm) ⭐️ 7.0/10

自 2026 年 11 月 18 日北京时间 12:00 起，DeepSeek 停止对服务端搜索和网页抓取单独计费，改为仅按模型 Token 用量收费。此前的 Search 与 Fetch API 按每 1,000 次成功请求收取 5 元费用。触发计费的联网工具、Anthropic API 的 web\_search 以及 Responses API 的 web\_search 将不再产生额外请求费用。

telegram · zaihuapd · 11月18日 13:44

**「DeepSeek 搜索与抓取 API 的计费方式」** DeepSeek 在 2026 年 10 月推出的 Search 与 Fetch API，原本按成功请求计费，每 1,000 次收费 5 元。该计费模式与 DeepSeek 其它模型使用方式不同，后者仅按模型输入输出的 Token 数量（每 1M Token 计费）收取费用。了解这两种计费方式有助于理解本次将搜索和抓取功能改为仅按 Token 用量计费的意义。

**「影响」** 开发者在使用 DeepSeek 的搜索或抓取功能时，只需关注模型 Token 消耗即可，预计可显著降低调用成本并简化预算管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/quick_start/pricing/?tool=deepseek">Models &amp; Pricing | DeepSeek API Docs</a></li>
<li><a href="https://www.ababnews.com/en/news/9b98272c-3464-4949-8cac-ae558f22d5be">DeepSeek API Charges 5 Yuan per 1000 Web Searches - ABAB News</a></li>

</ul>
</details>

**标签**: `#AI`, `#APIs`, `#Cost Management`, `#Machine Learning`

---

<a id="item-tech-news-9"></a>
### [酷态科 10 Ultra 充电头固件缺陷可能输出 20V 导致外设损坏](https://www.bilibili.com/opus/1272074321303437312) ⭐️ 7.0/10

酷态科 10 号 Ultra 充电头（型号 AD1204U）因 MCU 固件 bug，在极低概率下协议芯片不响应，可能向耳机、键盘等低压外设输出最高 20 V 的异常电压。厂商已定位并在本周一通过 OTA 推送修复固件，建议用户使用米家 App 通过蓝牙进行升级。首例受损发生在 2026 年 6 月，耐压 20 V 的手机、电脑等设备未受影响。

telegram · zaihuapd · 11月19日 01:30

**「充电协议芯片与电压协商概述」** USB Power Delivery 充电器通过内部协议芯片与被充设备协商输出电压，协议芯片的固件负责在检测到低压设备时切换到安全的 5 V 或 9 V 等电平。若固件出现异常导致芯片不响应，充电头会回退到默认的最高电压（如 20 V），从而可能损坏耳机、键盘等低压外设。该机制正是本次酷态科 10 Ultra（AD1204U）因 MCU 固件 bug 而出现过压风险的技术根源。

**「影响」** 受影响的用户和硬件开发者应尽快通过米家 App 更新固件，以防止低压外设被过压损坏；未更新的设备在极低概率下仍可能出现 20 V 输出风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://onebn.club/en/article/cuktech-issues-firmware-fix-for-10-ultra-charger-over-voltage-bug">CUKTECH Issues Firmware Fix for 10 Ultra Charger Over Voltage Bug</a></li>
<li><a href="https://www.163.com/dy/article/LC3HUBNO0511B8LM.html">酷态科10 Ultra确认存在低压设备损坏隐患，已OTA推送修复固件|充电头|...</a></li>

</ul>
</details>

**标签**: `#hardware`, `#firmware`, `#embedded`, `#consumer-electronics`

---

<a id="item-tech-news-10"></a>
### [美政府拟要求企业披露使用中国 AI 模型](https://www.reuters.com/world/china/trump-administration-weighs-forcing-us-firms-disclose-chinese-ai-use-2026-11-18/) ⭐️ 7.0/10

美国财政部和白宫科技政策办公室正讨论一项方案，可能要求美国企业在官网上公开披露使用的中国人工智能模型，例如 Airbnb 使用的阿里巴巴 Qwen 客服模型。该提议旨在通过公开点名降低对中国开放权重模型的依赖，但目前尚未确定是否获得内部支持或进入立法程序。

telegram · zaihuapd · 11月19日 02:30

**「背景」** 美国政府近期加强对中国人工智能技术的审查，已在多个场合讨论限制或标记使用中国模型的风险。已有美国企业如 Airbnb 在其客服系统中采用阿里巴巴的开源大模型 Qwen，这一实际使用案例被媒体报道。

**「影响」** 如果该政策实施，受影响的公司将需要在其网站上列明所使用的中国 AI 模型，以满足合规要求，这可能导致企业在选择 AI 供应商时面临额外的审查和成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aiusecasehub.com/case/dd44cd65306c24b4d91675442fb4620546c35251dc440569ee9e8fac452c46c2/airbnb-uses-alibaba-qwen-for-customer-service-ai-workloads">Airbnb uses Alibaba Qwen for customer-service AI workloads</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#US-China tech relations`, `#Corporate compliance`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储官员沃勒称可能需加息 0.5 个百分点](https://www.cnbc.com/2026/11/18/federal-reserve-governor-christopher-waller.html) ⭐️ 8.0/10

美联储理事克里斯托弗·沃勒在接受采访时表示，12 月的联邦公开市场委员会会议可能需要加息 0.5 个百分点，以遏制通胀。

rss · CNBC Finance · 11月18日 15:13

**「背景」** 此前美联储去年已降息 0.75 个百分点，近期通胀仍高于 2%目标并超过 3%。

**「影响」** 如果加息 0.5 个百分点，家庭和企业的贷款利率将上升，增加借贷成本。

**标签**: `#Federal Reserve`, `#Monetary Policy`, `#Inflation`, `#Interest Rates`

---

<a id="item-finance-news-2"></a>
### [腾讯 2026 年 Q3 营收与资本开支超预期](https://api3.cls.cn/share/article/2537922?os=android&amp;amp;sv=8.8.5&amp;amp;app=cailianpress&amp;amp;selected=) ⭐️ 8.0/10

腾讯公布 2026 年第三季度营收 2073 亿元，同比增长 8%；资本开支 814.33 亿元，远高于市场预估的 554 亿元，且 WorkBuddy 日均 Token 消耗超过 100 万亿，居国内首位。

telegram · zaihuapd · 11月18日 09:20

**「背景说明」** WorkBuddy 是腾讯面向办公用户的 AI 代理产品，使用大语言模型处理任务时会消耗“Token”，即模型生成或理解的文字单位；其日均 Token 消耗超过 100 万亿，显示出在中国大语言模型市场的最高使用量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.workbuddy.ai/">WorkBuddy - AI Agent for Everyday Office Work</a></li>
<li><a href="https://news.qq.com/rain/a/20261118A0DD3800">腾讯控股：WorkBuddy已成为中国使用量最高的AI产品，每日超千万用户合...</a></li>

</ul>
</details>

**标签**: `#Tencent`, `#Earnings`, `#AI Spending`, `#Capital Expenditure`, `#Chinese Tech`

---