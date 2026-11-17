---
layout: default
title: "Horizon Summary: 2026-11-17 (ZH)"
date: 2026-11-17
lang: zh
---

> 从 48 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [Optimizely 被入侵，向多家大型站点投放恶意代码](#item-tech-news-1) ⭐️ 8.0/10
2. [阿里等中国头部 AI 公司削弱新模型网络攻击能力](#item-tech-news-2) ⭐️ 8.0/10
3. [苹果中国区 App Store 新增 AIGC 合规入口，2027 前需补齐备案](#item-tech-news-3) ⭐️ 8.0/10
4. [Windows 11 开始收集开发者使用的编码工具数据](#item-tech-news-4) ⭐️ 7.0/10
5. [JPMorgan Chase 技术故障导致美国银行在线服务延迟](#item-tech-news-5) ⭐️ 7.0/10
6. [美国发布新规，限制远程使用先进 AI 芯片](#item-tech-news-6) ⭐️ 7.0/10

**财经新闻**
1. [伯克希尔哈撒韦第三季度调整持股：增持达美航空 5.37 亿美元，减持美国银行 1.6 亿美元](#item-finance-news-1) ⭐️ 7.0/10
2. [美国原油价格因中东出口回升跌至每桶 85.39 美元](#item-finance-news-2) ⭐️ 7.0/10
3. [微软调整云服务价格：印度涨 15.7%，中国降最高 8.5%](#item-finance-news-3) ⭐️ 7.0/10
4. [英特尔及 CEO 陈立武遭股东集体诉讼](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Optimizely 被入侵，向多家大型站点投放恶意代码](https://blog.report-uri.com/worlds-largest-brands-infected-with-malware-via-optimizely/) ⭐️ 8.0/10

攻击者在 Optimizely 的 JavaScript 代码片段中植入恶意脚本，导致使用该服务的数十个高流量网站（包括 Zoom、GitLab、CNN、BBC 等）向访客分发恶意软件。这是一场供应链攻击，受影响的网站并未直接泄露代码，而是通过 Optimizely 的 CDN 交付了被篡改的内容。Optimizely 自己的站点（如 www.optimizely.com）同样被感染，表明攻击者获得了对其系统的写入权限。该事件凸显了对第三方标签管理平台的安全依赖风险。

hackernews · kristjansson · 11月16日 23:00 · [社区讨论](https://news.ycombinator.com/item?id=50524767)

**「背景」** Optimizely 是一种常用的网页实验和 A/B 测试平台，站点通过在页面嵌入由 Optimizely CDN 提供的 JavaScript 代码来实现功能和营销标签。该平台的脚本在用户浏览器中执行，如果平台被入侵，攻击者即可向所有使用该服务的站点分发恶意代码，形成供应链攻击。2026 年 11 月 16 日的泄露显示，攻击者在 Optimizely Web 实验平台中植入了加密货币劫持和卡片窃取脚本，影响了包括 Zoom、BBC、CNN、GitLab 等 178 家高流量网站。

**「影响」** 受影响的站点需要立即移除并替换被篡改的 Optimizely 代码片段，审计所有通过该平台加载的脚本，并对相关凭证进行轮换；同时，安全团队应评估是否暂时停用第三方标签管理，以防止进一步的恶意内容分发。

**「社区讨论」** 评论者 mcoliver 认为此类供应链攻击本可避免，呼吁 Optimizely 实施更严格的发布审查、分阶段 rollout 和自动安全检测，并要求大型站点对第三方供应商承担更高的安全责任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://shiftdelete.net/en/optimizely-malware">Optimizely Malware Hit 178 Sites: What It Stole and What to Do</a></li>
<li><a href="https://cybersecuritynews.com/optimizely-websites-hijacked/">Hackers Infect 178 Major Websites via Optimizely to Steal ...</a></li>
<li><a href="https://www.stepsecurity.io/blog/optimjack-optimizely-hosted-scripts-crypto-clipper-card-skimmer">OPTIMJACK: Optimizely-Hosted Scripts Loaded a Crypto Clipper ...</a></li>

</ul>
</details>

**标签**: `#security`, `#web-development`, `#supply-chain`, `#malware`

---

<a id="item-tech-news-2"></a>
### [阿里等中国头部 AI 公司削弱新模型网络攻击能力](https://www.bloomberg.com/news/articles/2026-11-16/china-s-top-ai-firms-limit-cyber-capabilities-in-latest-models) ⭐️ 8.0/10

阿里巴巴、腾讯、月之暗面等中国领先的 AI 公司在最新一代模型中主动削减了进攻性网络功能。阿里最新旗舰模型 Qwen 未开放权重，用户无法下载完整版本；腾讯在本月发布的 Hy4 模型已在发布前去除网络攻击能力。此举与商务部上月公布的出口管制草案相呼应，该草案拟禁止出口能够攻击关键基础设施或政府网络的 AI 工具。

telegram · zaihuapd · 11月17日 02:20

**「背景」** AI 大模型具备生成网络攻击代码或策划渗透的潜在能力，过去部分模型以开放权重形式提供，易被滥用。商务部近期提出的出口管制草案旨在限制此类具备攻击性的 AI 工具跨境流通，以防止对关键基础设施的威胁。

**「影响」** 开发者将无法直接利用这些新模型进行攻击性网络实验或产品化，需转向其他工具或自行研发相应功能，同时也为即将生效的出口限制做好合规准备。

**标签**: `#AI safety`, `#China AI policy`, `#Cybersecurity`, `#Machine learning models`

---

<a id="item-tech-news-3"></a>
### [苹果中国区 App Store 新增 AIGC 合规入口，2027 前需补齐备案](https://www.ithome.com/1/028/158.htm) ⭐️ 8.0/10

Apple 在中国区 App Store Connect 后台新增两项强制性合规字段：AIGC 服务声明与备案信息以及安全评估证明。所有已上架的应用必须在 2027 年 1 月 31 日前补齐这些信息，新提交的应用则需立即提供。涉及聊天机器人、图像/视频生成、语音或人脸编辑等生成式 AI 功能的应用均在范围内，使用第三方技术的还需上传授权协议和算法备案号。该要求已写入 Apple 2026 年的审核指南。

telegram · zaihuapd · 11月17日 04:29

**「背景」** Apple 的 App Store Review Guidelines 规定了上架审核的所有要求，2026 年 10 月的指南更新已加入生成式 AI（AIGC）相关条款，明确了对使用聊天机器人、图像/视频生成、语音或人脸编辑等技术的应用的合规要求。该更新为本次在中国区 App Store Connect 后台新增的 AIGC 合规入口提供了政策依据。

**「影响」** 面向中国大陆的开发者必须在截止日期前在 App Store Connect 中填写并提交上述合规材料，否则其应用可能被拒审、下架或无法通过后续更新审核。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/news/?id=92th7e5i">Updated App Review Guidelines are now available - Apple Developer</a></li>

</ul>
</details>

**标签**: `#Apple`, `#App Store`, `#AIGC`, `#Compliance`, `#China`

---

<a id="item-tech-news-4"></a>
### [Windows 11 开始收集开发者使用的编码工具数据](https://xusheng.dev/posts/windows-coding-agent-telemetry/) ⭐️ 7.0/10

Windows 11 在默认开启的“诊断与反馈”设置中，新增对开发者使用的编码代理（如 Git、VS Code 插件）和开发工具的遥测收集，会记录这些工具的名称和路径并随诊断数据上报。用户可在“设置 → 隐私与安全 → 诊断与反馈”中关闭此功能。

hackernews · cwaffles · 11月16日 22:58 · [社区讨论](https://news.ycombinator.com/item?id=50524736)

**「背景」** Windows 11 通过名为 MissionControlAggregator 的系统组件，将已运行的编码代理和开发工具以位图形式记录在可选的诊断报告中，并在启用可选诊断数据时将其上报给 Microsoft。该机制基于 Windows 的 ETW（事件跟踪）框架，属于系统默认的可选遥测功能。

**「影响」** 开发者的工具使用信息将被发送至微软，可能泄露工作流细节；关注隐私的用户可通过上述设置关闭该遥测，以防止数据上报。

**「社区讨论」** 有评论指出，关闭方法是进入设置 → 隐私与安全 → 诊断与反馈，将“最佳遥测”关闭即可停止上报。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://xusheng.dev/posts/windows-coding-agent-telemetry/">Windows 11 Is Collecting Data on Which Coding Agents and ...</a></li>
<li><a href="https://windowsforum.com/news/windows-11-optional-telemetry-can-report-coding-agent-usage-research-finds.452631/">Windows 11 Optional Telemetry Can Report Coding Agent Usage ...</a></li>

</ul>
</details>

**标签**: `#Windows`, `#Telemetry`, `#DeveloperTools`, `#Privacy`, `#SoftwareEngineering`

---

<a id="item-tech-news-5"></a>
### [JPMorgan Chase 技术故障导致美国银行在线服务延迟](https://apnews.com/article/bank-outage-chase-wells-fargo-truist-50fee2693c22f597fa6ca51a97ef2cda) ⭐️ 7.0/10

2026 年 11 月 16 日，JPMorgan Chase 的技术故障导致其在线银行系统中断，进而影响美国多家银行（包括 Wells Fargo、Truist 等）的在线服务，用户在数小时内无法完成登录、转账等操作。该故障被归因于内部数据库或云基础设施问题，具体细节未公开。

hackernews · samk3nny · 11月16日 18:31 · [社区讨论](https://news.ycombinator.com/item?id=50521045)

**「银行系统的共享与核心平台依赖」** 美国的大型银行在在线服务层面高度互联，许多银行（包括富国银行和美国银行）使用 JPMorgan Chase 的核心交易和账户系统进行实时处理。这些核心平台通常运行在传统的主机环境（如 COBOL、CICS、IMS、DB2）上，提供跨行转账、账户查询和支付等关键功能。因此，Chase 的技术故障会导致其自身以及依赖其后端服务的其他银行出现在线取款、账户访问和交易延迟等问题。该事件并未被归因于网络攻击，而是一次内部技术失误导致的系统中断。

**「影响」** 受影响的银行客户在故障期间经历了交易延迟和无法访问账户的情况，建议在服务恢复前暂缓重要转账并关注银行官方通告。

**「社区讨论」** 社区评论中，stmw 指出这些核心业务很可能运行在传统的 COBOL、CICS、IMS、DB2 等老旧但可靠的主机系统上，暗示故障可能与这些遗留平台有关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.foxbusiness.com/money/jpmorgan-chase-systems-recovering-following-hourslong-nationwide-technical-outage">Chase systems coming back online after major outage | Fox ...</a></li>
<li><a href="https://www.usatoday.com/story/money/2026/11/16/bank-outage-nationwide-chase-bofa--live/92814152007/">Banking outage linked to Chase, impacted Wells Fargo and BofA</a></li>
<li><a href="https://chicago.suntimes.com/business/2026/11/16/a-technical-issue-at-jpmorgan-chase-triggers-online-banking-delays-across-major-us-banks">A technical issue at JPMorgan Chase triggers online banking ...</a></li>

</ul>
</details>

**标签**: `#banking`, `#cloud‑outage`, `#system‑reliability`, `#infrastructure`

---

<a id="item-tech-news-6"></a>
### [美国发布新规，限制远程使用先进 AI 芯片](https://www.reuters.com/legal/litigation/us-issues-rule-protect-advanced-ai-chips-being-accessed-remotely-2026-11-16/) ⭐️ 7.0/10

美国商务部于 2026 年 11 月 16 日发布临时最终规则，将对先进 AI 芯片的出口管制扩展至远程访问，要求任何通过第三国数据中心对这些芯片进行的远程调用均受限。该规则由财政部和国家安全委员会共同起草，旨在防止中国等地区通过第三国绕过现有限制。对印尼、马来西亚、新加坡、泰国和巴西的再出口也需申请许可。

telegram · zaihuapd · 11月16日 14:44

**「背景」** 此前美国已将部分高性能 AI 芯片列入《出口管理条例》（EAR）受控清单，限制其直接出口给中国等受限实体。本次规则是对该体系的补充，针对云服务等远程使用场景，以堵住通过跨境数据中心实现的间接获取渠道。

**「影响」** 受此规定约束的芯片制造商和云服务提供商必须为任何远程调用或再出口至上述五国的行为申请出口许可，否则将面临违规处罚，这可能导致向中国客户提供 AI 计算服务的延迟或成本上升。

**标签**: `#AI hardware`, `#export controls`, `#technology policy`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [伯克希尔哈撒韦第三季度调整持股：增持达美航空 5.37 亿美元，减持美国银行 1.6 亿美元](https://www.cnbc.com/2026/11/16/berkshire-hathaway-raised-its-stake-in-delta-air-in-the-third-quarter.html) ⭐️ 7.0/10

伯克希尔哈撒韦在 2023 年第三季度将其在达美航空的持股增至价值 5.37 亿美元（持股比例升至 12%），同时将对美国银行的持股削减约 1.6 亿美元（约 6%）。

rss · CNBC Finance · 11月16日 23:01

**「背景」** 达美航空因美伊冲突导致的燃油成本上升，股价在该季度下跌 11%；美国银行则受利率上升和通胀压力影响，股价下跌逾 4%。

**「影响」** 受此买入提振，达美航空股价在第四季度已回升约 3.8%，而标普 500 指数同期下跌 3.1%。

**标签**: `#Berkshire Hathaway`, `#Delta Air Lines`, `#Bank of America`, `#Equity Investment`, `#Airline Industry`

---

<a id="item-finance-news-2"></a>
### [美国原油价格因中东出口回升跌至每桶 85.39 美元](https://www.cnbc.com/2026/11/16/us-crude-oil-declines-to-87-a-barrel-on-recovering-middle-east-exports.html) ⭐️ 7.0/10

美国西德克萨斯中质原油（WTI）期货收于每桶 85.39 美元，跌幅 3.58%，因中东出口恢复导致 IEA 预测 2026 年第四季度全球供应将日超 170 万桶。

rss · CNBC Finance · 11月16日 22:19

**「背景」** 此前 IEA 曾预测全球原油供需缺口，但随着霍尔木兹海峡出口回升，供应预期转为盈余。

**标签**: `#crude oil`, `#oil prices`, `#supply-demand`, `#Middle East exports`

---

<a id="item-finance-news-3"></a>
### [微软调整云服务价格：印度涨 15.7%，中国降最高 8.5%](https://www.theregister.com/off-prem/2026/11/15/microsoft-lifts-indian-cloud-prices-by-15-percent-cuts-costs-in-china/5309993) ⭐️ 7.0/10

微软宣布自 2027 年 1 月 1 日起将印度云服务价格上调 15.7%，中国最高下调 8.5%，并在新西兰上调 10%、澳大利亚下调 4.5%、挪威下调 5.9%。

telegram · zaihuapd · 11月16日 08:47

**「背景说明」** Microsoft 通常每年会根据汇率波动和成本结构调整 Azure（其云服务）在各地区的价格，并通过官方公告公布具体的地区性涨跌。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/answers/questions/6025662/is-there-any-official-announcement-for-azure-vm-in">Is There any official announcement for Azure VM (in 7 regions ...</a></li>

</ul>
</details>

**标签**: `#cloud computing`, `#Microsoft pricing`, `#regional markets`

---

<a id="item-finance-news-4"></a>
### [英特尔及 CEO 陈立武遭股东集体诉讼](https://www.investing.com/news/stock-market-news/intel-sued-by-shareholders-following-29-stock-plunge-5028171) ⭐️ 7.0/10

英特尔 10 月 29 日发布低于预期的第四季度营收与利润预测，次日股价下跌 28.6%（市值蒸发约 1400 亿美元），随后密歇根州养老基金等股东在圣何塞联邦法院提起集体诉讼，CEO 陈立武和 CFO 津斯纳被列为被告。

telegram · zaihuapd · 11月16日 11:10

**「背景」** 在 10 月 29 日公布低于预期的 2026 财年第四季度营收和利润预测后，英特尔股价次日跌幅达 28.6%，市值蒸发约 1400 亿美元，此前的业绩失误是股东提起诉讼的直接导火索。

**「影响」** 2026 年 7 月 23 日至 10 月 29 日买入英特尔股票的股东可能通过本次集体诉讼寻求赔偿，同时此类诉讼通常会促使公司提升信息披露透明度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reuters.com/business/intel-sued-by-shareholders-following-29-stock-plunge-2026-11-15/">Intel sued by shareholders following 29% stock plunge | Reuters</a></li>
<li><a href="https://spectrum.library.concordia.ca/id/eprint/987254/1/Fardnia_PhD_F2020.pdf">Essays in Corporate Governance</a></li>
<li><a href="https://medium.com/@batoma9181/the-impact-of-class-action-lawsuits-on-corporate-behavior-f46ab6a51c55">The Impact of Class Action Lawsuits on Corporate Behavior | Medium</a></li>

</ul>
</details>

**标签**: `#Intel`, `#Shareholder lawsuit`, `#Earnings miss`, `#Corporate governance`

---