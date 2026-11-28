---
layout: default
title: "Horizon Summary: 2026-11-28 (ZH)"
date: 2026-11-28
lang: zh
---

> 从 31 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [Google DeepCrossAttention 将 Transformer 残差连接加速至 3 倍并保持质量](#item-tech-news-1) ⭐️ 8.0/10
2. [Minecraft 基岩版资源包漏洞已在 26.65 修复](#item-tech-news-2) ⭐️ 8.0/10
3. [微软计划用 Windows 内置驱动取代第三方驱动](#item-tech-news-3) ⭐️ 8.0/10
4. [Convex 后端技能未披露将用户应用创意发送至远程服务器](#item-tech-news-4) ⭐️ 7.0/10
5. [州检方起诉 SpaceX AI Grok 生成儿童性虐待及复仇色情图像](#item-tech-news-5) ⭐️ 7.0/10
6. [计算机检查证明的可靠性问题](#item-tech-news-6) ⭐️ 7.0/10
7. [豆包工作接入剪映插件，实现一句话视频剪辑](#item-tech-news-7) ⭐️ 7.0/10
8. [任正非称制裁促华为自立 感谢特朗普](#item-tech-news-8) ⭐️ 7.0/10

**财经新闻**
1. [国常会决定加强国家队稳市并优化平准基金功能](#item-finance-news-1) ⭐️ 7.0/10
2. [央行下调大额存单个人起购门槛至 10 万元](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Google DeepCrossAttention 将 Transformer 残差连接加速至 3 倍并保持质量](https://research.google/blog/supercharging-transformer-residual-connections/) ⭐️ 8.0/10

Google 在其博客中公布了 DeepCrossAttention 技术，可将 Transformer 模型的残差连接计算速度提升至 3 倍，同时保持相同的模型质量。该方法通过在残差路径中使用交叉注意力机制来替代传统的全连接投影，从而减少计算量。实验表明，在多个标准基准上，使用 DeepCrossAttention 的模型在吞吐量上提升约 2–3 倍，而准确率或损失与原始实现无显著差异。该技术目前已在 Google 的内部模型训练流水线中可用，尚未公开发布代码或库。

hackernews · ComputedCamp995 · 11月27日 23:06 · [社区讨论](https://news.ycombinator.com/item?id=50672565)

**「Transformer 残差连接概述」** Transformer 模型在每层使用残差连接（Add &amp; Norm）将输入直接加到层输出，以缓解梯度消失并加速收敛。这种结构自原始的《Attention Is All You Need》论文提出后成为标准实现，然而其计算路径仍受限于顺序加法和归一化操作。

**「加速 Transformer 训练与推理」** 使用 DeepCrossAttention 后，Transformer 的残差连接可提升至 3 倍的吞吐量，同时保持原有模型质量，意味着研发团队在训练大模型或部署服务时可显著降低计算成本和时间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.google/blog/supercharging-transformer-residual-connections/">Supercharging transformer residual connections</a></li>
<li><a href="https://research.google/blog/supercharging-transformer-residual-connections/">Supercharging transformer residual connections - Google Research</a></li>

</ul>
</details>

**标签**: `#Transformers`, `#Performance Optimization`, `#Deep Learning`

---

<a id="item-tech-news-2"></a>
### [Minecraft 基岩版资源包漏洞已在 26.65 修复](https://www.zaikei.co.jp/article/20261119/878386.html) ⭐️ 8.0/10

Minecraft 基岩版在 26.52‑26.63 版本中发现资源包漏洞，影响 PC、移动端和主机，Java 版不受影响。该漏洞允许携带 content.zipe 的资源包修改游戏 UI 并执行隐藏脚本，甚至在特定条件下下载恶意软件。Mojang 已在 26.65 版本中修复此问题。

telegram · zaihuapd · 11月27日 18:04

**「资源包机制概述」** 在《我的世界》基岩版（Bedrock）中，资源包是一种可供玩家下载的文件集合，通常以 .zip 或 .content.zipe 形式提供，用于替换游戏的纹理、声音和 UI 布局等资源。基岩版的资源包在加载时会直接写入游戏的 UI 框架文件，并在特定条件下执行其中的脚本或批处理文件，这一行为在早期版本中未受到严格的安全限制。

**「影响」** 使用自动下载资源包的玩家在受影响的版本中可能被植入恶意脚本，建议立即更新至 26.65 或使用 AxmBro 的只读检测工具检查 content.zipe 文件。

**标签**: `#security`, `#gaming`, `#Minecraft`, `#vulnerability`

---

<a id="item-tech-news-3"></a>
### [微软计划用 Windows 内置驱动取代第三方驱动](https://www.techspot.com/news/114721-microsoft-wants-replace-most-third-party-device-drivers.html) ⭐️ 8.0/10

微软在 Ignite 2026 上宣布，将在 Windows 中内置一系列硬件驱动，以取代现有的第三方驱动。首批目标是打印机，已推出 Windows Ready Print 模式用于替代传统打印驱动；随后音频（SoundWire、SDCA）、I3C 总线、USB‑以太网和 MIPI 摄像头等驱动也在开发中。微软产品经理表示，这些内置驱动将直接集成到系统内核，降低第三方代码的渗透。

telegram · zaihuapd · 11月28日 02:09

**「Windows 内置驱动的演进背景」** Windows 操作系统长期依赖第三方厂商提供的内核模式驱动，这导致系统安全和稳定性面临风险。为降低这些风险，Microsoft 早在 2000 年推出了 Windows Driver Model（WDM），随后在 2006 年引入了 Windows Driver Framework（WDF），统一了驱动开发规范并鼓励使用通用的内置驱动组件。近期的 Windows Ready Print 模式和驱动质量倡议（DQI）进一步体现了 Microsoft 将更多硬件功能迁移到系统自带驱动的趋势，为本次在 Ignite 2026 上宣布的以内置驱动取代打印机、音频、I3C、USB‑Ethernet 与摄像头等第三方驱动奠定了技术和安全基础。

**「影响」** OEM 和硬件厂商需要改用 Windows 提供的内置驱动，减少或停止发布自研第三方驱动，否则可能面临兼容性和安全合规问题。

**标签**: `#Windows`, `#Device Drivers`, `#Operating Systems`, `#Hardware Integration`, `#System Security`

---

<a id="item-tech-news-4"></a>
### [Convex 后端技能未披露将用户应用创意发送至远程服务器](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 7.0/10

Convex 的 AI 网关中的一个后端技能被发现会在未提示用户的情况下，将开发者在应用中输入的创意或提示上传至外部服务器。该行为未在文档或使用条款中披露，导致对平台隐私和数据安全的担忧。此问题涉及 Convex 的 “quickstart” 功能，继承自已下线的 Convex Chef 项目。

hackernews · MickyTheMouse · 11月27日 18:02 · [社区讨论](https://news.ycombinator.com/item?id=50669765)

**「背景」** Convex 在其平台上提供 AI gateway 和 “quickstart” 技能（Agent Skills），开发者可通过 npx skills CLI 将这些技能加入项目，这些技能会在本地生成应用概念后，将用户的 app idea 发送到 Convex 的 .site 主机并执行远程脚本，以便快速启动项目。此前已有报道指出，这类技能在应用创建前会发出多次遥测请求，且包含规避安全分类器的指令。

**「潜在数据泄露风险」** Convex 的后端 skill 在未提示用户的情况下将应用创意发送至外部服务器，意味着使用该 AI 网关的开发者其代码和业务构想可能被未经授权地收集，需审查或禁用该 skill，或迁移至自托管模型以防止敏感信息外泄。

**「社区讨论」** Convex CEO Jamie 在评论中说明，该插件用于 Convex 的 “quickstart” 功能，是已停用的 Convex Chef 项目的精神继承者，并负责提示的上传。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/convex/convex-backend-skill/issues/64">Convex skills send the user&#x27;s app idea to a remote server ...</a></li>
<li><a href="https://dev.to/frankchu/3-telemetry-calls-before-your-app-exists-convex-skills-69f">3 telemetry calls before your app exists — Convex skills</a></li>
<li><a href="https://nhimg.org/glossary/ai-data-exfiltration/">What Is AI Data Exfiltration? Definition &amp; Examples</a></li>

</ul>
</details>

**标签**: `#security`, `#AI`, `#backend`, `#privacy`

---

<a id="item-tech-news-5"></a>
### [州检方起诉 SpaceX AI Grok 生成儿童性虐待及复仇色情图像](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 7.0/10

弗吉尼亚州检察长等多州检方于 2026 年 11 月 27 日对 SpaceX 旗下的 AI 模型 Grok 提起诉讼，指控该模型生成并传播儿童性虐待图像和复仇色情内容。诉状称 Grok 的生成能力被用于制作此类非法图像，要求法院强制停止其发布并采取整改措施。

hackernews · DeepLogin · 11月27日 19:42 · [社区讨论](https://news.ycombinator.com/item?id=50670855)

**「背景」** Grok 是 SpaceX 母公司 xAI 开发的对话式生成式人工智能模型，已在公开平台上提供使用。此前已有媒体报道和法律行动指称 Grok 被用于生成未成年人的性剥削图像，例如《卫报》2026 年 9 月的报道以及 CNBC 同年 11 月的诉讼跟踪。

**「影响」** 若诉讼成功，SpaceX 可能被迫在 Grok 中部署更严格的内容过滤和审查机制，甚至暂停该模型的公开使用，以避免法律责任并恢复公众信任。

**「社区讨论」** 评论者对现有平台禁令表示困惑，质疑是否有人故意规避限制；另一位指出应关注实际实施者；还有人提及最高法院已裁定个人使用 AI 生成的儿童性虐待材料受言论保护，但前提是不涉及真实儿童。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/sep/03/elon-musk-ai-grok-child-porn-lawsuit">Child sexual abuse survivor alleges Elon Musk’s AI... | The Guardian</a></li>
<li><a href="https://www.cnbc.com/2026/11/23/oregon-virginia-spacex-grok-deepfake-lawsuits.html">SpaceX sued by 2 states over AI deepfake porn, Grok safety claims</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#generative AI`, `#legal`, `#ethics`

---

<a id="item-tech-news-6"></a>
### [计算机检查证明的可靠性问题](https://cr.yp.to/proofs/falseccp.html) ⭐️ 7.0/10

文章指出多个主流证明助理（如 Lean、nanoda、Metamath 等）曾出现过声音性（soundness）缺陷，导致错误的数学证明能够被计算机误判为有效。这对依赖形式化验证的研究人员、软件工程师以及数学家构成风险，因为即使形式化工具给出“已验证”结果，也可能隐藏未被发现的漏洞。

hackernews · \_tk\_ · 11月27日 15:26 · [社区讨论](https://news.ycombinator.com/item?id=50667989)

**「背景」** Formal proof assistants such as Lean and Metamath rely on a small trusted kernel whose soundness guarantees that any proof accepted by the checker is logically valid. Past incidents have shown that kernels can contain subtle bugs—for example, Lean 4’s kernel accepted a false theorem due to bug \#14576 \(a nested‑inductive phantom‑parameter flaw\) and was later fixed【tool-1-3】. To reduce the impact of such bugs, projects like Metamath require proofs to be validated by several independently written verifiers \(C, Java, Rust, C++\)【tool-2-3】。

**「影响」** 使用这些工具的项目应考虑采用多重独立验证——例如在 Metamath 中要求同一证明通过五种不同语言实现的验证器，以降低单一检查器缺陷导致的误判风险。

**「社区讨论」** 评论者 dwheeler 提到，Metamath 为了确保可靠性，要求提交的证明必须同时通过 C、Java、Python、Haskell 和 Lisp 等五种独立实现的验证器，展示了业界已有的多验证策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://essamamdani.com/blog/lean-4-soundness-bug-14576-postmortem">Lean 4 Soundness Bug #14576: What Broke the Kernel</a></li>
<li><a href="http://at.metamath.org/">Home Page - Metamath</a></li>

</ul>
</details>

**标签**: `#formal verification`, `#theorem proving`, `#software reliability`

---

<a id="item-tech-news-7"></a>
### [豆包工作接入剪映插件，实现一句话视频剪辑](https://36kr.com/newsflashes/4087610228046208) ⭐️ 7.0/10

豆包工作宣布独家接入剪映官方插件，新增“一句话剪辑”功能并支持多轨编辑。用户只需用一句自然语言描述剪辑需求，系统即可调用剪映完成视频剪切，并可通过对话继续修改或打开多轨草稿进行细致调节。此功能为产品层面的发布，尚未涉及第三方评测或性能数据。

telegram · zaihuapd · 11月27日 07:45

**「背景」** Doubao Work 是字节跳动推出的 AI 办公助理，之前已支持文档、邮件等文字任务；而剪映（Jianying）是字节跳动旗下的专业视频剪辑工具，提供插件接口供第三方调用。此次独家接入剪映官方插件，使得用户可以在 Doubao Work 中仅用一句自然语言描述，即可驱动剪映完成视频的粗剪和多轨细调，这基于此前已有的插件化架构和 Doubao Work 的语言理解能力。

**「影响」** 内容创作者和企业用户可通过自然语言快速生成初步剪辑，大幅缩短手动编辑时间，并可在同一平台完成细节微调，提升制作效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.cocoloop.cn/en/2026/11/doubao-work-jianying-plugin/">Doubao Work adds Jianying plugin for one-sentence rough cuts</a></li>

</ul>
</details>

**标签**: `#AI video editing`, `#natural language interface`, `#software tooling`, `#Chinese tech news`

---

<a id="item-tech-news-8"></a>
### [任正非称制裁促华为自立 感谢特朗普](https://thenextweb.com/news/ren-zhengfei-huawei-trump-thanks-nyt-interview) ⭐️ 7.0/10

华为创始人任正非在接受《纽约时报》采访时表示，美国制裁推动华为及中国走向芯片自立，并请该报向前总统特朗普转达感谢。他称华为已成为“我们自己国家的公司”，并预言中国在芯片领域终将超越美国。

telegram · zaihuapd · 11月27日 16:35

**「背景」** 自 2019 年起，美国对华为实施了包括实体清单、芯片出口禁令在内的多轮制裁，旨在切断其获取美国关键半导体和软件的渠道，限制其在 5G 与人工智能领域的竞争力。近期美国陪审团对华为涉及窃取商业机密和伊朗制裁违规的指控作出有罪判决，华为则坚称缺乏法律依据。正是在这种持续的外部压力下，任正非强调华为必须走向芯片自立，并将美国的制裁视为推动中国整体半导体自主的催化剂。

**「影响」** 任正非的表态暗示华为将进一步加大自主芯片研发力度，以降低对美国技术的依赖，这可能推动中国本土半导体产业的投资和产能提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/11/26/business/huawei-trump-china-ai.html">Trump Tried to Cripple Huawei . Now It Is Central to China’s A.I. Push.</a></li>
<li><a href="https://finance.yahoo.com/news/huawei-ceo-ren-zhengfei-exclusive-interview-us-fall-behind-174227834.html">Huawei CEO Ren Zhengfei : &#x27;Shutting Huawei out is the start of the...</a></li>

</ul>
</details>

**标签**: `#Huawei`, `#US sanctions`, `#semiconductors`, `#technology industry`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [国常会决定加强国家队稳市并优化平准基金功能](https://www.tmtpost.com/nictation/8220182.html) ⭐️ 7.0/10

国务院常务会议决定加大“国家队”在资本市场的稳市作用，并进一步优化中央汇金公司类“平准基金”功能，以提供充足流动性支持。

telegram · zaihuapd · 11月27日 05:35

**「背景」** “国家队”指由国家主导的投资机构（如中央汇金、中国证券金融公司等），在市场非理性下跌时逆周期增持股票或 ETF 以维护资本市场稳定；“平准基金”是中央汇金等设立的用于提供充足流动性、在股市波动时进行调节的基金。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://baike.baidu.com/item/%E5%9B%BD%E5%AE%B6%E9%98%9F/68623816">国家队（中国金融市场中的国家投资机构）_百度百科</a></li>
<li><a href="https://news.qq.com/rain/a/20261127A0C82D00">国常会定调资本市场，机构解读：稳市机制迈向制度化升级</a></li>

</ul>
</details>

**标签**: `#China`, `#capital markets`, `#government policy`, `#market stabilization`

---

<a id="item-finance-news-2"></a>
### [央行下调大额存单个人起购门槛至 10 万元](https://www.news.cn/fortune/20261127/70789d77822242cc82216f51a416f872/c.html) ⭐️ 7.0/10

中国人民银行自 2027 年 3 月 21 日起将个人大额存单起购金额下调至 10 万元，机构下调至 500 万元，并要求金融机构自行确定存贷款利率。

telegram · zaihuapd · 11月27日 11:36

**「背景」** 此前《大额存单管理暂行办法》规定个人起点 20 万元、机构 1000 万元，此次下调为原门槛的一半。

**「影响」** 降低个人门槛将使更多散户能够购买大额存单，可能提升银行对高净值客户的存款竞争。

**标签**: `#Monetary Policy`, `#Banking Regulation`, `#Deposits`, `#China`

---