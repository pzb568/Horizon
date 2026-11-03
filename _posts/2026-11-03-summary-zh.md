---
layout: default
title: "Horizon Summary: 2026-11-03 (ZH)"
date: 2026-11-03
lang: zh
---

> 从 47 条内容中筛选出 13 条重要资讯。

---

**科技新闻**
1. [vllm-project/vllm released v0.33.0rc3](#item-tech-news-1) ⭐️ 8.0/10
2. [Ubuntu LTS 内核仍未修复 CVE‑2026‑98432 高危 RCE 漏洞](#item-tech-news-2) ⭐️ 8.0/10
3. [ChatGPT 分享链接漏洞导致账号被接管已修复](#item-tech-news-3) ⭐️ 8.0/10
4. [WIRED：400+ AI 应用暗藏色情深伪功能 被平台下架](#item-tech-news-4) ⭐️ 8.0/10
5. [阿布扎比与 OpenAI 签署四项协议 推动机器可读政府](#item-tech-news-5) ⭐️ 8.0/10
6. [sgl-project/sglang released v0.5.23](#item-tech-news-6) ⭐️ 7.0/10
7. [Astra 可读写 Qwen 权重以提升性能](#item-tech-news-7) ⭐️ 7.0/10
8. [Cloudflare 将 DNS 构建延迟减半，内存使用降低 85%](#item-tech-news-8) ⭐️ 7.0/10
9. [llm 0.37](#item-tech-news-9) ⭐️ 7.0/10
10. [LightMIS：面向边缘设备的超轻量医学图像分割模型](#item-tech-news-10) ⭐️ 7.0/10
11. [xAI 推出 Data Bot 为团队提供数据科学助理](#item-tech-news-11) ⭐️ 7.0/10

**科技博客**
1. [LLM 并非超人式读取与编辑网络权重](#item-tech-blog-1) ⭐️ 8.0/10

**财经新闻**
1. [德州州长选举预测市场显示阿博特胜率 60%，希诺霍萨升至约 40%](#item-finance-news-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [vllm-project/vllm released v0.33.0rc3](https://github.com/vllm-project/vllm/releases/tag/v0.33.0rc3) ⭐️ 8.0/10

vLLM 0.33.0rc3 introduces numerous new models and key infrastructure upgrades, making it a high‑value update for AI/ML developers.

github · khluu · 11月2日 10:10

**标签**: `#vLLM`, `#PyTorch`, `#CUDA`, `#LLM inference`, `#Open source`

---

<a id="item-tech-news-2"></a>
### [Ubuntu LTS 内核仍未修复 CVE‑2026‑98432 高危 RCE 漏洞](https://freenode.net/article/ubuntu-lts-kernels-still-unfixed-for-critical-cve-2026-98432) ⭐️ 8.0/10

自漏洞披露近三周后，Ubuntu LTS 系列内核仍未提供针对 CVE‑2026‑98432（可远程代码执行）的补丁。Ubuntu 将该漏洞标记为“High”优先级，而非“Critical”，因此未触发紧急发布流程，也未提供官方缓解措施。

hackernews · majorchord · 11月2日 18:39 · [社区讨论](https://news.ycombinator.com/item?id=50341462)

**「CVE‑2026‑98432 背景概述」** CVE‑2026‑98432 是 2026 年披露的 Linux 内核远程代码执行（RCE）漏洞，攻击者可利用该缺陷在内核层面执行任意代码。漏洞公开后，Linux 上游已发布相应补丁，通常会被各发行版回移至其内核包中。Ubuntu 的长期支持（LTS）内核会根据安全更新的优先级进行处理：若标记为 “Critical”，会触发紧急、非计划的补丁发布；若为 “High”，则遵循常规的安全更新周期。

**「影响」** 使用受影响 Ubuntu LTS 发行版的系统管理员仍面临远程代码执行风险，需自行部署临时防御（如 iptables/u32 过滤规则）或考虑迁移至已发布补丁的发行版。

**「社区讨论」** 评论者指出 Ubuntu 未提供任何官方缓解方案，并质疑其将漏洞定为仅“High”而非“Critical”的原因；另有用户分享使用 iptables u32 规则在 raw PREROUTING 链中阻断攻击的临时办法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://brandefense.io/security-news/cve-2026-98432-ubuntu-kernel-status/">CVE-2026-98432 Ubuntu Kernel Status - Brandefense</a></li>
<li><a href="https://github.com/soroushneshati/cve-2026-98432-ubuntu-mitigation">GitHub - soroushneshati/cve-2026-98432-ubuntu-mitigation ...</a></li>

</ul>
</details>

**标签**: `#Linux`, `#Security`, `#Ubuntu`, `#Kernel Vulnerability`

---

<a id="item-tech-news-3"></a>
### [ChatGPT 分享链接漏洞导致账号被接管已修复](https://www.parameter.ai/labs/we-found-a-gap-at-openai) ⭐️ 8.0/10

OpenAI 于 10 月 26 日修复了 ChatGPT 分享链接功能中的一项严重漏洞，该漏洞允许攻击者通过恶意链接在已登录用户的会话中执行代码，读取私密对话并将数据发送至外部服务器。漏洞利用了预览功能与图表组件之间的消息处理缺陷，已被 OpenAI 定级为 P1，并向发现团队支付了 5000 美元赏金。受影响的用户只需打开恶意链接即可被攻击，无需额外软件或权限。

telegram · zaihuapd · 11月2日 10:24

**「ChatGPT 分享链接功能概述」** ChatGPT 的“分享链接”功能可以生成一个公开 URL，任何人打开后即可在浏览器中预览对应的对话内容，无需登录。该链接会渲染对话中的交互组件（如图表），这些组件在后台通过消息处理与前端交互。此前的实现存在消息处理缺陷，使得恶意链接能够在已登录用户的会话中执行代码，从而读取私密对话并向外部服务器发送数据。

**「影响」** 使用旧版客户端或未及时更新的用户仍可能受到该漏洞的威胁，建议立即升级到最新版本并避免点击来源不明的 ChatGPT 分享链接，以防止账号被接管或私密数据泄露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rrtechpulse.com/stories/chatgpt-shared-link-account-flaw/">ChatGPT shared link flaw, fixed Oct. 26 | RR Tech Pulse</a></li>

</ul>
</details>

**标签**: `#security`, `#AI`, `#ChatGPT`, `#vulnerability`

---

<a id="item-tech-news-4"></a>
### [WIRED：400+ AI 应用暗藏色情深伪功能 被平台下架](https://www.wired.com/story/hundreds-of-mundane-ai-apps-are-hiding-abusive-deepfake-features/) ⭐️ 8.0/10

WIRED 调查发现，超过 400 个以宠物画像、语言学习等普通功能伪装的 AI 应用和网站，在特定条件下会加载色情深度伪造页面，允许用户上传他人照片生成露骨图像或视频。调查依据代码、域名和广告追踪，将该网络与中文开发者及一家香港注册公司关联。随后，苹果下架了 19 款违规应用，谷歌在被联系前已移除多数同类应用，Meta 则阻止了 209 款应用的广告投放。

telegram · zaihuapd · 11月2日 12:45

**「背景」** 深度伪造（deepfake）技术能够利用生成式 AI 将人物图像或视频合成逼真的色情内容，过去已有报告指出部分移动应用在审核通过后通过远程加载网页或代码来隐藏此类功能，导致被应用商店下架。此次 WIRED 调查的 400 多个应用正是利用类似手法，在表面上提供宠物绘图、语言学习等普通功能，却在特定条件下触发色情深伪页面。

**「影响」** 这些平台的下架和广告封禁直接削减了违规 AI 应用的分发渠道，提醒开发者在审核通过后不得更换远端内容，并促使应用商店加强对隐藏功能的审查，以保护用户免受色情深伪内容侵害。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cellularnews.com/mobile-apps/bytedance-hides-deepfake-maker-feature-within-tiktok-code/">ByteDance Hides Deepfake Maker Feature Within... | CellularNews</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#deepfake abuse`, `#app store policy`, `#security`

---

<a id="item-tech-news-5"></a>
### [阿布扎比与 OpenAI 签署四项协议 推动机器可读政府](https://thenextweb.com/news/openai-abu-dhabi-deals-machine-readable-government-mubadala) ⭐️ 8.0/10

阿布扎比政府本周与 OpenAI 签署了四项协议，其中包括“机器可读政府”计划，旨在将政策法规转化为 AI 可读的结构化格式，以帮助官员核查许可和证书申请，已在食品进口审批上进行试点，且官员仍保留最终决定权。穆巴达拉与 OpenAI 以及 G42 子公司 Inception42 合作开展投资分析，并签订了为期五年的协议，向阿联酋政府、企业和学校提供模型。ADNOC 成为首家使用 OpenAI Frontier 平台的能源公司。

telegram · zaihuapd · 11月2日 15:55

**「背景」** 机器可读政府的核心是将政策法规转化为结构化、机器可解析的格式，使 AI 能够检索、比对并辅助官员审查许可和证书申请。此类把法律文本结构化的做法在金融等行业的监管科技（RegTech）已有应用，但在整体政府层面尚属首次。Khaleej Times 于 2026 年 11 月 2 日的报道指出，这一计划是全球首个 AI 原生的机器可读政府项目。

**「影响」** 这些协议使阿联酋政府部门能够通过 AI 快速检索和解读法规，预计将缩短审批流程并提升行政效率；同时，能源企业 ADNOC 通过使用 Frontier 平台，可在能源生产和交易中应用大模型进行预测和优化，需要相应的内部系统集成和数据安全审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.khaleejtimes.com/uae/abu-dhabi-crown-prince-openai-altman-4-deals-key-sectors">Abu Dhabi Crown Prince meets OpenAI &#x27;s Sam Altman... | Khaleej Times</a></li>

</ul>
</details>

**标签**: `#AI governance`, `#OpenAI partnerships`, `#Government technology`, `#Enterprise AI`, `#Middle East tech`

---

<a id="item-tech-news-6"></a>
### [sgl-project/sglang released v0.5.23](https://github.com/sgl-project/sglang/releases/tag/v0.5.23) ⭐️ 7.0/10

sglang v0.5.23 introduces many new models and shows active community involvement, offering useful tools for AI developers.

github · Fridge003 · 11月2日 22:14

**标签**: `#LLM`, `#Diffusion`, `#Open-source`, `#ModelRelease`

---

<a id="item-tech-news-7"></a>
### [Astra 可读写 Qwen 权重以提升性能](https://rikiyat.github.io/blog/weight-space-programming/) ⭐️ 7.0/10

博客介绍了名为 Astra 的新方法，声称能够直接读取和写入 Qwen 大语言模型的权重，从而在特定任务（如数学推理）上实现约 5 倍的性能提升。该技术目前仅在作者的实验报告中展示，尚未得到独立验证或公开发布。

hackernews · dbreunig · 11月2日 18:21 · [社区讨论](https://news.ycombinator.com/item?id=50341174)

**「背景」** Weight‑Space Programming 是一种直接读取和写入大语言模型权重的技术，早在过去几年里研究者就已经能够编辑、生成或定位模型权重，以实现特定功能的微调。该方法在近期的 Astra 项目中被用于对 Qwen 3.5‑0.8B 进行权重编辑，旨在提升其数学推理能力。相关实验和代码已在公开博客和 Hugging Face 仓库中展示。

**「影响」** 如果 Astra 的权重编辑技术可行，AI 开发者将能够在无需大规模再训练的情况下，对 Qwen 等模型进行针对性改进，从而加速特定功能的定制化部署。

**「社区讨论」** 评论区意见分歧：部分用户指出权重编辑已有研究，认为博客夸大了成果；另一些用户对其在小模型上提升数学能力的表现表示惊讶。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rikiyat.github.io/blog/weight-space-programming/">Sparks of Weight - Space Programming : LLMs can natively read...</a></li>
<li><a href="https://huggingface.co/JonathanColetti/Qwen3.5-0.8B-Astra-WeightEdit">JonathanColetti/ Qwen 3.5-0.8B- Astra -WeightEdit · Hugging Face</a></li>

</ul>
</details>

**标签**: `#weight-editing`, `#LLM`, `#Qwen`, `#AI-tools`

---

<a id="item-tech-news-8"></a>
### [Cloudflare 将 DNS 构建延迟减半，内存使用降低 85%](https://blog.cloudflare.com/dns-targeted-zone-builds/) ⭐️ 7.0/10

Cloudflare 的工程团队通过针对 DNS 区域构建的优化，将构建延迟降低了 50%，同时将内存占用削减了约 85%。此改进已在其生产环境中部署，面向使用 Cloudflare DNS 服务的所有客户以及关注大规模基础设施性能的开发者。

hackernews · wondersky · 11月2日 14:47 · [社区讨论](https://news.ycombinator.com/item?id=50337558)

**「DNS 区域构建的传统方式」** 在 Cloudflare 之前，任何 DNS 区域设置的更改都会触发对整个区域的完整重建，即使该区域包含数千万条记录。这种全量构建导致峰值内存占用极高，并显著延长构建延迟，使得频繁的配置更新成本昂贵。

**「实际影响」** 内存需求的大幅下降使得同等硬件可以支撑更多的 DNS 区域，降低了运营成本并提升了系统的可扩展性。

**「社区讨论」** 有评论者（thephyber）关心内存节省的投资回报率，认为在未来 1‑2 年内内存价格仍然偏高，优化内存使用的 ROI 可能值得关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/dns-targeted-zone-builds/">How we halved DNS build delay and cut memory use by 85%</a></li>

</ul>
</details>

**标签**: `#DNS`, `#PerformanceOptimization`, `#CloudInfrastructure`

---

<a id="item-tech-news-9"></a>
### [llm 0.37](https://simonwillison.net/2026/Nov/2/llm/) ⭐️ 7.0/10

Simon Willison’s llm 0.37 release introduces new model options, improved endpoint configuration, and broader embedding support, offering useful upgrades for LLM‑focused developers.

rss · Simon Willison · 11月2日 23:49

**标签**: `#LLM`, `#Python`, `#CLI`, `#OpenAI-compatible`, `#Embeddings`

---

<a id="item-tech-news-10"></a>
### [LightMIS：面向边缘设备的超轻量医学图像分割模型](https://www.reddit.com/r/MachineLearning/comments/1xm8dbo/lightmis_ultralightweight_medical_image/) ⭐️ 7.0/10

LightMIS 是一种 2D 二值医学图像分割模型，仅包含 131K 参数，使用的 GFLOPs 比 nnWNet 少 94.58%，参数量少 98.14%。在相同的 nnU‑Net v2.3.1 训练协议下，LightMIS 在六个数据集、五种成像模态上实现了接近 nnWNet 的 Dice 和 IoU 平均值。实测在 Arm Mali‑G52 MC2 GPU 上，完整模型的推理速度约为 nnWNet 的 10.5 倍，且所有算子均在 GPU 上运行，无需 CPU 回退。代码、检查点和复现细节已在 GitHub 开源。

reddit · r/MachineLearning · /u/OkLion2068 · 11月2日 20:22

**「背景」** nnU‑Net 是一个自动配置的医学图像分割框架，它会根据数据集特性自行设定预处理、数据增强和网络超参数，已成为评估分割模型的统一基准。nnWNet 是在 nnU‑Net 基础上提出的轻量级编码‑解码架构，结合卷积和 transformer 以捕获全局和局部特征，常被用作轻量模型的参考。

**「影响」** 该模型使得在资源受限的边缘设备上进行医学图像分割成为可能，开发者可在保持接近最先进精度的前提下，实现实时或低功耗的临床辅助应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ieeexplore.ieee.org/document/11219025">A Modified nnWNet Architecture With Multi-Scale and State ...</a></li>
<li><a href="https://github.com/MIC-DKFZ/nnUNet">GitHub - MIC-DKFZ/nnUNet · GitHub</a></li>

</ul>
</details>

**标签**: `#medical-imaging`, `#edge-computing`, `#lightweight-models`, `#segmentation`

---

<a id="item-tech-news-11"></a>
### [xAI 推出 Data Bot 为团队提供数据科学助理](https://x.ai/news/data-bot) ⭐️ 7.0/10

xAI 在 Grok Bot 系列中宣布推出 Team Bot「Data Bot」，该 AI 助手可查询团队维护的共享技能数据仓库、执行分析并根据使用者偏好生成图表或报告，同时可加入 Slack 频道主动参与讨论。官方称上周 Data Bot 已承担约 70 小时原本需要数据科学家完成的工作。此功能目前为公告阶段，具体可用性和定价尚未披露。

telegram · zaihuapd · 11月3日 02:44

**「背景」** Data Bot 是 xAI 在其 Grok Bot 平台上推出的 Team Bot，利用共享的只读凭证在 Databricks 数据仓库中查询批准的表格，并可生成图表或报告。Team Bot 的概念源自 xAI 早前在 2026 年 9 月发布的“共享 AI 同事”功能，旨在让团队成员无需等待分析师即可获取数据洞察。

**「影响」** 团队若将 Data Bot 集成至 Slack，可在短期内将约 70 小时的数据分析工作转移给 AI，从而降低对专职数据科学家的即时需求，并加速报告生成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unite.ai/xai-introduces-data-bot-to-bring-shared-analytics-skills-to-grok-bot/">xAI Introduces Data Bot to Bring Shared Analytics Skills to ...</a></li>
<li><a href="https://x.ai/news/team-bots">Team Bots: shared AI teammates that learn as they work</a></li>

</ul>
</details>

**标签**: `#AI`, `#DataScience`, `#CollaborationTools`, `#Bots`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [LLM 并非超人式读取与编辑网络权重](https://seangoedecke.com/llms-are-not-superhuman-at-reading-and-writing-neural-network-weights/) ⭐️ 8.0/10

rss · Sean Goedecke · 11月3日 00:00

**「背景」** 近期一篇论文宣称前沿 LLM（如 GPT‑6 Astra）能够直接读取小网络的权重并识别其训练的游戏，甚至通过编辑权重显著提升 0.8B Qwen 模型的数学能力。作者认为这听起来像是超人般的能力，但实际上这些任务并不超出普通机器学习研究者的范畴。

**「方案」** 作者指出，游戏网络的输入通道已经标记并对应 8×8 网格，使得仅通过计算第一层权重的 L2 范数即可快速生成热图，从而直观看出玩家和移动物体的位置，这在 Python 中只需三行代码即可实现，远非“超人”计算。对于 Qwen 的循环问题，作者解释这其实是模型在超过 32k token 时出现的已知循环错误，传统的“steering”或 Heretic abliteration 方法——即对比循环与非循环文本的残差、测量权重贡献并裁剪关键权重——完全可以手动完成，而 Astra 所做的正是这一步骤。作者进一步将直接权重编辑类比为 LLM 输出机器码并修改二进制的技巧，强调即便 LLM 能够生成权重更新的代码，最有效的模型改进仍然是通过常规训练流程实现。整体来看，作者认为这些实验展示的是 LLM 在辅助实现已有技术手段，而非开创全新、颠覆性的研究范式。

**「启示」** LLM 能直接读取或编辑权重并不意味着它们具备超人级别的 AI 研究能力；它们更适合作为加速传统训练和调试流程的工具，而非取代人类的核心创新手段。

**标签**: `#LLM weight manipulation`, `#Neural network interpretability`, `#AI research methodology`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [德州州长选举预测市场显示阿博特胜率 60%，希诺霍萨升至约 40%](https://www.cnbc.com/2026/11/02/texas-governor-prediction-markets-abbott-hinojosa.html) ⭐️ 7.0/10

根据预测市场平台 Kalshi，现任州长 Greg Abbott 的获胜概率为 60%，民主党候选人 Gina Hinojosa 的获胜概率已从 7 月的约 8%升至约 40%。

rss · CNBC Finance · 11月2日 21:13

**「背景信息」** 2025 年 11 月，德克萨斯州州长格雷格·阿博特与谷歌共同宣布该公司将在州内投入 400 亿美元建设数据中心，并称德克萨斯将成为人工智能发展的中心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gov.texas.gov/news/post/governor-abbott-google-announce-40-billion-investment-in-texas">Governor Abbott, Google Announce $40 Billion Investment In Texas</a></li>
<li><a href="https://www.texastribune.org/2025/11/14/texas-google-data-centers-ai/">Google data centers totaling $40 billion coming to Texas</a></li>
<li><a href="https://texasscorecard.com/state/google-to-bring-more-data-centers-to-texas/">Google To Bring More Data Centers to Texas - Texas Scorecard</a></li>

</ul>
</details>

**标签**: `#politics`, `#prediction‑markets`, `#AI‑data‑centers`, `#Texas‑economy`

---