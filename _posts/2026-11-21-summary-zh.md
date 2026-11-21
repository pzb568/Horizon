---
layout: default
title: "Horizon Summary: 2026-11-21 (ZH)"
date: 2026-11-21
lang: zh
---

> 从 40 条内容中筛选出 7 条重要资讯。

---

**科技新闻**
1. [SEC 调查 Nvidia 潜在会计问题](#item-tech-news-1) ⭐️ 8.0/10
2. [OpenAI 推出后台模式，支持最长 8 小时异步请求，Token 费用最高降 40%](#item-tech-news-2) ⭐️ 8.0/10
3. [台积电暂停对华 16nm 以下芯片订单](#item-tech-news-3) ⭐️ 8.0/10
4. [TikTok 全球上线 AI 深度伪造检测工具](#item-tech-news-4) ⭐️ 7.0/10
5. [苹果计划 2027 年底推出自主 AI 智能体](#item-tech-news-5) ⭐️ 7.0/10

**财经新闻**
1. [北京拟规定租金押金不得因正常损耗扣减并须存入监管账户](#item-finance-news-1) ⭐️ 8.0/10
2. [美国公司转向大规模增发股票，可能给牛市带来压力](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [SEC 调查 Nvidia 潜在会计问题](https://www.marketscreener.com/news/us-sec-s-nvidia-probe-is-examining-potential-accounting-issues-sources-say-ce785ed3dd8ff627) ⭐️ 8.0/10

美国证券交易委员会（SEC）已启动对 Nvidia 的会计做法进行调查，重点审查其可能的收入确认和融资安排等会计处理是否存在违规。该调查目前仍在进行中，尚未公布具体结论或处罚。

hackernews · ftchd · 11月20日 20:22 · [社区讨论](https://news.ycombinator.com/item?id=50581438)

**「背景概述」** Nvidia 是全球领先的人工智能加速器芯片制造商，过去几年因 AI 需求激增其市值和收入快速增长。此前该公司已因收入确认和财务披露方式受到监管审查，例如 2023 年的相关质疑。SEC 对其会计做法的调查正是在此监管关注的背景下展开的。

**「影响」** 如果 SEC 发现违规，Nvidia 可能被要求重新报表或进行财务整改，这将对其股价造成下行压力并增加公司合规成本。

**「社区讨论」** 评论者 eyeat 认为，此次调查是对 Nvidia 过去五年循环融资行为的延续，可能进一步加剧其股价的修正压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reuters.com/world/us-secs-nvidia-probe-is-examining-potential-accounting-issues-sources-say-2026-11-20/">Nvidia&#x27;s accounting is a focus of US SEC investigation ...</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#SEC investigation`, `#AI hardware`, `#Tech finance`

---

<a id="item-tech-news-2"></a>
### [OpenAI 推出后台模式，支持最长 8 小时异步请求，Token 费用最高降 40%](https://developers.openai.com/api/docs/guides/background) ⭐️ 8.0/10

OpenAI 在 API 中新增后台模式，开发者可在请求体中加入 background:true 并通过 background\_options.completion\_window 选择 2 小时或 8 小时的完成窗口。2 小时窗口的 Token 费率比标准价低约 30%，8 小时窗口则低约 40%；未指定窗口时使用默认 soonest，且不享受折扣。该模式目前在 GPT-6.2 Astra、GPT-6.2 Sol、GPT-6.1 Terra 和 GPT-6 Luna 四款模型上进行公测，且即使将 store 设为 false 或启用零数据保留，响应数据仍会临时存储。

telegram · zaihuapd · 11月20日 11:15

**「背景说明」** 在 OpenAI API 之前，所有请求默认是同步执行，调用方必须在请求返回前保持连接，且没有针对长时间运行任务的专门折扣机制。OpenAI 先前已提供标准的 token 计费模型和可选的流式（stream）响应，但并未支持将请求转为异步并在数小时后完成。此次推出的后台模式在此基础上加入了异步执行选项和针对 2 小时或 8 小时完成窗口的显著 token 费用折扣。

**「影响」** 开发者可以将耗时长的生成任务交由后台模式异步处理，最长可挂起 8 小时，同时通过相应的折扣将 Token 成本降低至原价的 60%，有助于降低大规模或批量任务的预算压力。使用时需在请求中显式开启 background 并指定 completion\_window 以获得折扣。

**标签**: `#OpenAI API`, `#Background mode`, `#Cost optimization`, `#Long-running tasks`

---

<a id="item-tech-news-3"></a>
### [台积电暂停对华 16nm 以下芯片订单](https://appleinsider.com/articles/26/11/20/apple-supplier-tsmc-cuts-off-china-chip-orders-amid-tighter-export-controls) ⭐️ 8.0/10

台积电已通知客户，依据收紧的美国半导体出口新规，暂停向中国公司提供 16nm 及以下制程的芯片订单。除非事先取得美国出口许可或豁免，否则不得供货，导致中国企业只能使用 28nm、40nm 等较旧制程，无法获得 AI 数据中心所需的高带宽内存。

telegram · zaihuapd · 11月21日 02:01

**「背景」** 美国近期收紧了对半导体技术的出口管制，要求任何向中国供应 16 nm 及以下制程的芯片都必须事先获得美国政府的出口许可或豁免。此前台积电可以自行评估客户设计是否符合豁免条件，并仍向中国企业提供这些先进制程的芯片。新规下，除非获得许可，否则只能向中国客户交付 28 nm、40 nm 等较旧制程的产品。

**「影响」** 中国的 AI 硬件厂商将失去获取先进 AI‑grade 硅片的渠道，必须转向较老的制程或寻找其他代工厂，可能导致产品性能下降或研发成本上升。

**标签**: `#semiconductors`, `#export controls`, `#AI hardware`, `#TSMC`

---

<a id="item-tech-news-4"></a>
### [TikTok 全球上线 AI 深度伪造检测工具](https://www.straitstimes.com/world/tiktok-launches-tool-to-help-public-figures-detect-deepfakes-globally) ⭐️ 7.0/10

TikTok 自 11 月 20 日起在全球范围内推出 Likeness Detection 工具，经过第三方身份验证的公众人物和头部创作者可收到他人未经授权使用其形象生成的 AI 内容提示并进行举报。同时，平台提供公开的透明工具，任何人无需账号即可上传图片或视频查询是否由 TikTok 的 AI 功能生成。

telegram · zaihuapd · 11月20日 08:14

**「背景」** 深度伪造检测工具利用机器学习模型分析图像、视频或音频中的特征，以辨别是否为 AI 合成内容，已被多家平台用于提升内容真实性。欧盟自 2026 年 8 月起要求在其境内发布的 AI 生成内容必须加上机器可读的标记或水印，以便识别和监管，这一法规推动社交媒体公司在全球范围内推出相应的检测与标注功能。TikTok 此次推出的 Likeness Detection 正是响应该监管要求，为经验证的公众人物和创作者提供未授权 AI 形象使用的提醒与举报渠道。

**「影响」** 已通过验证的公众人物和创作者将实时获知并可举报未经授权的深度伪造内容，帮助提升平台内容真实性，并协助满足欧盟自 2026 年 8 月起对 AI 生成内容标注的合规要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.claude.com/en/articles/16266773-how-claude-marks-ai-generated-content">How Claude marks AI -generated content | Claude Help Center</a></li>

</ul>
</details>

**标签**: `#AI Ethics`, `#Deepfake Detection`, `#Content Moderation`, `#Social Media`

---

<a id="item-tech-news-5"></a>
### [苹果计划 2027 年底推出自主 AI 智能体](https://www.bloomberg.com/news/articles/2026-11-19/apple-is-working-on-ai-agent-for-device-control-apps-browsing-and-coding) ⭐️ 7.0/10

彭博通过本周苹果新增的招聘信息发现，苹果正在招聘高级工程经理负责“主动式 AI 智能体”项目。该智能体旨在代替用户完成写代码、浏览网页和操控应用等任务，预计最早于 2027 年末面世，当前仍处于早期研发阶段。此信息基于招聘泄露，尚未有官方确认或产品原型公开。

telegram · zaihuapd · 11月20日 08:59

**「背景」** AI 智能体是一类能够替用户编写代码、浏览网页、控制应用等的代理软件，已由 Meta 的 Muse、OpenAI 等公司推出。苹果在 macOS 27.3 中加入了针对第三方智能体的权限警告页面，将获取系统控制的步骤从 4 步增至 14 步，表明系统已在为此类功能做安全准备。此次招聘信息显示苹果正组建团队开发“主动式 AI 智能体”，属于对已有行业趋势的内部跟进。

**「影响」** 如果按计划推出，开发者届可能需要在 2027 年后适配苹果的 AI 编码与自动化助手，届时相关工具和工作流将受到影响，但因发布时间较远，短期内对现有开发生态的直接冲击有限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-19/apple-is-working-on-ai-agent-for-device-control-apps-browsing-and-coding">Apple Is Working on AI Agent for Device Control, Apps... - Bloomberg</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#Apple`, `#software development`, `#industry news`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [北京拟规定租金押金不得因正常损耗扣减并须存入监管账户](https://mp.weixin.qq.com/s/PmGxh5knIyxiBRhpRoJnoQ) ⭐️ 8.0/10

北京发布《住房租赁合同（示范文本）修订征求意见稿》，明确承租人因正常使用导致的房屋损耗不承担赔偿责任，出租人不得以此扣减押金，并要求租金押金存入监管账户。

telegram · zaihuapd · 11月20日 13:46

**「背景」** 此前，北京市于 2023 年发布了《住房租赁合同（示范文本）》，为租赁双方权益提供框架，现正由住建委和市场监管局修订。

**「影响」** 北京的租户将更有可能全额收回押金，出租人和租赁企业则需将押金存入监管账户，增加合规成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.beijing.gov.cn/fuwu/bmfw/sy/jrts/202611/t20261120_4954272.html">北京拟修订住房租赁合同示范文本，出租人不得以这种理由扣押金_信息提...</a></li>

</ul>
</details>

**标签**: `#Housing policy`, `#Rental market`, `#Consumer protection`, `#Beijing`

---

<a id="item-finance-news-2"></a>
### [美国公司转向大规模增发股票，可能给牛市带来压力](https://www.cnbc.com/2026/11/20/equity-issuance-bull-market-problem.html) ⭐️ 7.0/10

美国公司正从回购转向增发股票，最新数据显示本周净新增发行占总市值的 3.1%。

rss · CNBC Finance · 11月20日 14:15

**「背景」** 在此之前，美国公司大多通过回购股票来缩减流通股本、提升每股收益，形成了以买入为主的市场环境。

**「影响」** 新增股票供应可能削弱牛市的上涨动力，对持股投资者的回报构成下行压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/20/equity-issuance-bull-market-problem.html">equity issuance bull market problem</a></li>

</ul>
</details>

**标签**: `#equity issuance`, `#bull market`, `#corporate finance`, `#IPO`, `#market trends`

---