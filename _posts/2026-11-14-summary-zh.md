---
layout: default
title: "Horizon Summary: 2026-11-14 (ZH)"
date: 2026-11-14
lang: zh
---

> 从 40 条内容中筛选出 4 条重要资讯。

---

**科技新闻**
1. [双 RTX 4090 GPU 实时全频段航空波段解码系统](#item-tech-news-1) ⭐️ 7.0/10
2. [Claude Code 2.1.323 引入实验性 Code Mode 支持 JavaScript 调用工具](#item-tech-news-2) ⭐️ 7.0/10
3. [DeepSeek 开放全家桶多模态 API，支持搜索、OCR、ASR 等功能](#item-tech-news-3) ⭐️ 7.0/10

**财经新闻**
1. [芝加哥联储主席古尔斯比称美联储仍需应对通胀](#item-finance-news-1) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [双 RTX 4090 GPU 实时全频段航空波段解码系统](https://orcasairband.com/) ⭐️ 7.0/10

一位业余爱好者使用双 RTX 4090 显卡和 CUDA 在 ETTUS B210 SDR 上实现了全频段航空波段的实时捕获与解码。该系统采用多相通道化技术在 GPU 上对整个空中频段进行通道化、解调并检测传输，仅保留文本转录。项目在维多利亚（CA）因地面停飞而意外成为飞行员获取空域通话内容的实时信息源。此实现属于业余级别的原型，而非商业化或官方航空通信系统。

hackernews · mmaunder · 11月13日 22:04 · [社区讨论](https://news.ycombinator.com/item?id=50490593)

**「背景」** 航空频段（airband）指用于民用航空通信的 118‑137 MHz VHF 频段，传统上通过专用硬件接收并解调。软件定义无线电（SDR）如 Ettus B210 能将射频信号数字化后交由通用计算平台处理，而利用 CUDA 在 GPU（如 RTX 4090）上实现多相通道化和实时解调，可在单台机器上同时处理整个频段的数百个子信道。

**「影响」** 该原型展示了消费级 GPU（RTX 4090）能够在实时条件下处理完整航空波段，为高性能软件定义无线电和实时信号处理提供了可行的参考路径，可能促使更多开发者尝试类似的 GPU 加速 SDR 项目。

**「社区讨论」** 评论者指出，在地面停飞期间系统提供的实时转录帮助飞行员了解空域情况；也有人提到传输仍然相当嘈杂且多数为模拟信号，暗示解码质量仍有提升空间。

**标签**: `#software engineering`, `#GPU computing`, `#software-defined radio`, `#real-time systems`

---

<a id="item-tech-news-2"></a>
### [Claude Code 2.1.323 引入实验性 Code Mode 支持 JavaScript 调用工具](https://code.claude.com/docs/en/changelog) ⭐️ 7.0/10

Claude Code 于 2026 年 11 月 12 日发布 2.1.323 版本，新增实验性的 Code Mode，允许 Claude 通过 JavaScript 调用外部工具，并可在组织层面关闭此功能。该版本还强化插件管理：若插件声明的版本范围与实际不匹配，将被阻止安装或更新，且 plugin validate 增加了对 TypeScript 钩子类型的检查。除此之外，新增了 .docx 文档上传支持和 30 秒钩子心跳等改进。

telegram · zaihuapd · 11月13日 03:47

**「背景说明」** Claude Code 是 Anthropic 提供的 AI 编码助手，之前只能生成代码或文本回复，无法在对话中直接调用外部工具。此次 2.1.323 版引入的实验性 Code Mode 让模型能够通过嵌入的 JavaScript 脚本执行工具调用，这在此前的版本中并不存在。该功能的加入基于对插件系统的改进，包括更严格的版本匹配和对 TypeScript 钩子类型的检查。

**「影响」** 开发者现在可以在 Claude Code 中编写 JavaScript 脚本以自动化工具调用，提升编码工作流的灵活性；但需确保插件的版本声明符合要求，否则插件将被拒绝安装或更新。

**标签**: `#Claude`, `#AI coding assistant`, `#JavaScript`, `#plugin management`, `#software engineering`

---

<a id="item-tech-news-3"></a>
### [DeepSeek 开放全家桶多模态 API，支持搜索、OCR、ASR 等功能](https://mp.weixin.qq.com/s/78KBHc4-4N5b2vfL9SkutQ) ⭐️ 7.0/10

DeepSeek 在其 V4.1‑Flash 模型上正式开放全家桶应用 API，开发者只需在原有 API 请求中开启相应参数，即可使用深度思考搜索、文件输入、阅读链接、语音等多模态对话能力。当前已在搜索（Search）、抓取（Fetch）和 OCR、ASR、TTS 三类接口实现支持，且每项功能均可单独调用。官方同时开源了可导入历史对话的前端 Demo，用户可通过 https://deepseek-ai.github.io/chat-demo/ 本地部署使用。

telegram · zaihuapd · 11月13日 14:27

**「DeepSeek API 的前置概念」** DeepSeek 早期仅提供基于文本的聊天 API，开发者通过调用单一的语言模型接口获取对话回复。随着其 V4.1‑Flash 多模态模型的发布，平台首次在同一模型上支持搜索、网页抓取、光学字符识别（OCR）、语音识别（ASR）和文本转语音（TTS）等功能，使得开发者可以在同一套 API 中开启相应参数，实现图像、音频和网页内容的自动处理与上下文拼接。

**「影响」** 开发者现在可以直接通过 DeepSeek 的 API 将搜索、文档抓取、光学字符识别、语音识别和语音合成等能力集成到自己的应用中，无需自行搭建复杂的工具链；同时开源的本地部署 Demo 为需要离线或私有化部署的团队提供了快速上手的参考实现。

**标签**: `#DeepSeek`, `#Multimodal API`, `#AI Tools`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [芝加哥联储主席古尔斯比称美联储仍需应对通胀](https://www.cnbc.com/2026/11/13/chicago-feds-goolsbee-says-central-bank-has-definitely-got-work-to-do-on-inflation.html) ⭐️ 8.0/10

芝加哥联储主席古尔斯比在接受采访时表示，美联储仍需采取行动，市场已将 12 月 FOMC 会议加息 0.25 个百分点计入价格，且加息 0.5 个百分点的概率超过 10%。

rss · CNBC Finance · 11月13日 14:22

**「背景说明」** 美联储的通胀目标是 2%，但 10 月生产者物价指数（PPI）同比上涨 6.5%，为 2022 年 11 月以来最高，且消费者物价指数（CPI）也高于预期，使通胀已接近六年维持在目标以上。

**「影响」** 若加息实现，借贷成本上升将直接影响家庭和企业的贷款利率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/13/chicago-feds-goolsbee-says-central-bank-has-definitely-got-work-to-do-on-inflation.html">Chicago Fed&#x27;s Goolsbee says central bank &#x27;has definitely got ...</a></li>
<li><a href="https://www.bls.gov/news.release/archives/ppi_11132026.htm">Producer Price Index News Release - 2026 M10 Results</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-11/fed-s-goolsbee-says-october-cpi-report-borderline-disturbing-mwbel9qz">Fed’s Goolsbee Says October CPI Report ‘Borderline Disturbing’</a></li>

</ul>
</details>

**标签**: `#monetary policy`, `#inflation`, `#interest rates`, `#Fed`

---