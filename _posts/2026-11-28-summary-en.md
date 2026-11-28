---
layout: default
title: "Horizon Summary: 2026-11-28 (EN)"
date: 2026-11-28
lang: en
---

> From 31 items, 10 important content pieces were selected

---

**Technology News**
1. [Google DeepCrossAttention speeds transformer residuals up to 3×](#item-tech-news-1) ⭐️ 8.0/10
2. [Minecraft Bedrock resource‑pack vulnerability fixed in 26.65](#item-tech-news-2) ⭐️ 8.0/10
3. [Microsoft to Replace Certain Third‑Party Drivers with Built‑In Windows Drivers](#item-tech-news-3) ⭐️ 8.0/10
4. [Convex backend skill silently exfiltrates user app ideas to remote server](#item-tech-news-4) ⭐️ 7.0/10
5. [States sue SpaceX over Grok&\#x27;s generation of child sexual abuse and revenge porn images](#item-tech-news-5) ⭐️ 7.0/10
6. [Soundness bugs found in proof checkers raise reliability concerns](#item-tech-news-6) ⭐️ 7.0/10
7. [Doubao Work integrates Jianying plugin for one‑sentence video editing](#item-tech-news-7) ⭐️ 7.0/10
8. [Ren Zhengfei credits US sanctions for Huawei’s push to self‑reliance and thanks Trump](#item-tech-news-8) ⭐️ 7.0/10

**Financial News**
1. [China&\#x27;s State Council to Boost &quot;National Team&quot; and Optimize Stabilization Funds](#item-finance-news-1) ⭐️ 7.0/10
2. [China central bank lowers large‑deposit certificate threshold to ¥100,000](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Google DeepCrossAttention speeds transformer residuals up to 3×](https://research.google/blog/supercharging-transformer-residual-connections/) ⭐️ 8.0/10

Google’s DeepCrossAttention technique modifies transformer residual connections to run up to three times faster than standard implementations. The method preserves comparable model quality, meaning accuracy and performance remain on par with unmodified transformers. This optimization is presented as a practical way for engineers and researchers to accelerate large‑scale AI training and inference without sacrificing results.

hackernews · ComputedCamp995 · Nov 27, 23:06 · [Discussion](https://news.ycombinator.com/item?id=50672565)

**「Transformer residual connections」** Standard transformer architectures use sequential residual connections that add the output of each sub‑layer to its input, helping gradients flow and stabilizing training. DeepCrossAttention replaces this fixed addition with a learnable routing mechanism that weights contributions from multiple paths, a variation first described in Google’s recent blog post. Understanding this shift from static to learnable residual routing is key to appreciating the reported speed‑up.

**「Faster transformer training with unchanged quality」** Applying DeepCrossAttention to transformer models can reduce training or inference time by up to three‑fold while keeping model quality comparable, letting developers lower compute costs or iterate more quickly on large‑scale AI systems.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/supercharging-transformer-residual-connections/">Supercharging transformer residual connections</a></li>
<li><a href="https://arxiv.org/abs/2502.06785">[2502.06785] DeepCrossAttention: Supercharging Transformer ...</a></li>
<li><a href="https://research.google/blog/supercharging-transformer-residual-connections/">Supercharging transformer residual connections - Google Research</a></li>

</ul>
</details>

**Tags**: `#Transformers`, `#Performance Optimization`, `#Deep Learning`

---

<a id="item-tech-news-2"></a>
### [Minecraft Bedrock resource‑pack vulnerability fixed in 26.65](https://www.zaikei.co.jp/article/20261119/878386.html) ⭐️ 8.0/10

A cross‑platform security flaw in Minecraft Bedrock resource packs—where a malicious content.zipe file could modify the Ore UI and execute hidden scripts—was confirmed to affect versions 26.52 through 26.63 \(and possibly earlier\). The issue, disclosed by Reddit user 8Crafter on November 15, can be triggered automatically when a server or Realm forces a resource‑pack download, allowing actions such as deleting saves, harvesting player IPs, or launching arbitrary URIs on Windows. Mojang released version 26.65, which patches the vulnerability; the Java edition is not affected.

telegram · zaihuapd · Nov 27, 18:04

**「Prerequisite concept」** Minecraft Bedrock Edition allows players to install resource packs, which are zip archives that can replace game assets and include a special file named content.zipe. When a resource pack is automatically downloaded \(for example, when joining a server or Realm that forces a pack\), the client extracts and loads these files without requiring explicit user interaction. Because the content.zipe file can contain scripts that run in the game’s UI framework, a malicious pack can modify the Ore UI and execute hidden code, leading to actions such as deleting saved worlds, exposing the player’s IP address, or launching arbitrary URIs on Windows systems.

**「Impact」** Players and server operators should update to Bedrock version 26.65 immediately; the fix removes the content.zipe execution path, preventing the described remote code execution and data‑theft attacks.

**Tags**: `#security`, `#gaming`, `#Minecraft`, `#vulnerability`

---

<a id="item-tech-news-3"></a>
### [Microsoft to Replace Certain Third‑Party Drivers with Built‑In Windows Drivers](https://www.techspot.com/news/114721-microsoft-wants-replace-most-third-party-device-drivers.html) ⭐️ 8.0/10

Microsoft announced at Ignite 2026 that it will begin substituting many third‑party device drivers with native Windows drivers. The first focus is printers, using a new Windows Ready Print mode to retire legacy printer drivers. Subsequent built‑in drivers are planned for audio \(SoundWire, SDCA\), I3C bus, USB‑Ethernet, and MIPI camera hardware. The shift is presented as a security and reliability measure to reduce third‑party code in the kernel.

telegram · zaihuapd · Nov 28, 02:09

**「Prerequisite Context」** Windows historically depends on hardware manufacturers and third‑party vendors to provide signed kernel‑mode drivers for most devices, creating a large external driver ecosystem that runs in the OS kernel. Recent Microsoft initiatives—such as the Windows Driver Frameworks, stricter driver‑signing enforcement, and the Windows Ready Print abstraction for printers—have aimed to improve driver reliability and security, setting the stage for the announced shift toward native Windows drivers for categories like printers, audio, I3C, USB‑Ethernet, and cameras.

**「Impact」** Hardware OEMs and driver developers will need to transition to the forthcoming built‑in drivers, revising or retiring their custom kernel drivers to maintain compatibility and benefit from the promised security and stability improvements. OEMs should monitor the Windows Driver Quality Initiative \(DQI\) and plan updates to align with the new native driver stack.

**Tags**: `#Windows`, `#Device Drivers`, `#Operating Systems`, `#Hardware Integration`, `#System Security`

---

<a id="item-tech-news-4"></a>
### [Convex backend skill silently exfiltrates user app ideas to remote server](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 7.0/10

A Convex backend skill was discovered to automatically forward the app idea a developer submits to an external server, without any notice or consent. The exfiltration occurs through Convex’s AI gateway that powers the Quickstart feature, which is the successor to the now‑shut‑down Convex Chef project. This behavior represents a privacy and trust breach for developers who rely on Convex’s platform for AI‑assisted development. No public acknowledgment or mitigation has been provided by Convex at the time of reporting.

hackernews · MickyTheMouse · Nov 27, 18:02 · [Discussion](https://news.ycombinator.com/item?id=50669765)

**「Convex AI gateway and quickstart skills」** Convex offers an AI gateway that developers can invoke through &quot;quickstart&quot; or &quot;agent&quot; skills, which are portable packages that bootstrap a new app by sending the user’s app idea to a Convex‑hosted .site endpoint and executing remote scripts. These skills run before any user code exists and are designed to bypass safety checks, which is why the reported exfiltration is possible. The issue stems from this built‑in telemetry and script‑execution behavior of Convex’s quickstart skill infrastructure.

**「Potential data leakage for Convex users」** Developers who enable Convex’s AI gateway skill may have their app ideas silently transmitted to an external server, exposing proprietary concepts without consent. They should audit or disable the skill, and consider using a self‑hosted model or stricter data‑handling controls to prevent unauthorized data exfiltration.

**「Community discussion」** Convex CEO Jamie replied that the prompt‑upload functionality underlies the Quickstart feature and stems from the former Convex Chef product, but the response did not directly address the undisclosed data transmission concern raised by the issue reporter.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/convex/convex-backend-skill/issues/64">Convex skills send the user&#x27;s app idea to a remote server ...</a></li>
<li><a href="https://dev.to/frankchu/3-telemetry-calls-before-your-app-exists-convex-skills-69f">3 telemetry calls before your app exists — Convex skills</a></li>
<li><a href="https://nhimg.org/glossary/ai-data-exfiltration/">What Is AI Data Exfiltration? Definition &amp; Examples</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI`, `#backend`, `#privacy`

---

<a id="item-tech-news-5"></a>
### [States sue SpaceX over Grok&\#x27;s generation of child sexual abuse and revenge porn images](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 7.0/10

Virginia attorneys general filed a lawsuit against SpaceX, the parent company of xAI and its Grok model, alleging that the AI system has been used to create and promote child sexual exploitation images and non‑consensual \(revenge porn\) content. The complaint seeks an injunction to stop Grok from generating such material and to compel SpaceX to implement safeguards. The claim is based on alleged failures to prevent the model from producing illegal imagery, not on a released technical update from SpaceX.

hackernews · DeepLogin · Nov 27, 19:42 · [Discussion](https://news.ycombinator.com/item?id=50670855)

**「Background」** Grok is the generative‑AI chatbot created by XAI, the SpaceX subsidiary that launched the model in 2024, and it has been the subject of prior legal scrutiny for producing illegal child sexual‑abuse and deep‑fake images. Earlier reports include a September 2026 Guardian article about a survivor suing over AI‑generated abuse images and a June 2026 case where a Pennsylvania man was arrested for using Grok to create child‑pornography images.

**「Impact」** If the court grants the injunction, SpaceX would be required to add or strengthen content‑filtering mechanisms for Grok, potentially setting a precedent that could force other generative‑AI providers to adopt stricter moderation to avoid similar litigation.

**「Community discussion」** Commenters expressed confusion about existing bans on such content and referenced a Supreme Court ruling that AI‑generated child sexual abuse material for personal use is protected speech, while noting that revenge‑porn depictions may not be covered by that protection.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/sep/03/elon-musk-ai-grok-child-porn-lawsuit">Child sexual abuse survivor alleges Elon Musk’s AI... | The Guardian</a></li>
<li><a href="https://www.robertkinglawfirm.com/mass-torts/grok-lawsuit/">Grok Lawsuit for AI Deepfakes &amp; Sexual Exploitation of Minors</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#generative AI`, `#legal`, `#ethics`

---

<a id="item-tech-news-6"></a>
### [Soundness bugs found in proof checkers raise reliability concerns](https://cr.yp.to/proofs/falseccp.html) ⭐️ 7.0/10

The page documents several soundness bugs discovered in popular proof assistants such as Lean, Metamath, and nanoda, showing that a formally checked proof can be accepted even when it is mathematically false. The bugs arise from implementation errors in the checkers, meaning that a false proof may pass verification if the checker’s flaw is not detected, and the issue is not limited to a single system but can affect multiple independent verifiers.

hackernews · \_tk\_ · Nov 27, 15:26 · [Discussion](https://news.ycombinator.com/item?id=50667989)

**「Background」** Proof assistants such as Lean and Metamath verify mathematical arguments by running a small trusted kernel that checks proof terms for logical correctness. When the kernel contains a soundness bug—e.g., Lean 4’s kernel accepted a false theorem via a nested‑inductive phantom‑parameter bug \(bug \#14576\) or the original Metamath C verifier had a flaw—an incorrect proof can be accepted unless it is also checked by independent verifiers written in other languages.

**「Impact」** Users of formal verification tools should not rely solely on a single automated checker; employing multiple independent verifiers or supplementing with manual review is advisable to mitigate the risk of accepting incorrect proofs.

**「Community Discussion」** Commenters note that the Metamath library requires proofs to pass five independently written verifiers in different languages, while a DeepMind researcher demonstrated a proof that passed both Lean and an early version of nanoda by exploiting distinct bugs in each, highlighting the practical relevance of the soundness issues.

<details><summary>References</summary>
<ul>
<li><a href="https://essamamdani.com/blog/lean-4-soundness-bug-14576-postmortem">Lean 4 Soundness Bug #14576: What Broke the Kernel</a></li>
<li><a href="http://at.metamath.org/">Home Page - Metamath</a></li>

</ul>
</details>

**Tags**: `#formal verification`, `#theorem proving`, `#software reliability`

---

<a id="item-tech-news-7"></a>
### [Doubao Work integrates Jianying plugin for one‑sentence video editing](https://36kr.com/newsflashes/4087610228046208) ⭐️ 7.0/10

Doubao Work has integrated the official Jianying plugin, enabling users to edit videos by describing the desired cut in a single sentence. The integration also supports multi‑track editing, allowing users to refine the result through additional dialogue or by opening a multi‑track draft for fine‑tuning. The feature is now available to Doubao Work users via the plugin interface.

telegram · zaihuapd · Nov 27, 07:45

**「Prerequisite concepts」** Doubao Work is ByteDance’s AI‑powered office assistant that provides productivity tools for enterprise users. Jianying \(Jianying Pro\) is a popular video‑editing application that offers an official plugin interface for programmatic control. The integration builds on earlier AI‑driven natural‑language editing concepts, where users can issue simple textual commands to trigger editing actions in a video editor.

**「Impact」** Users can produce a trimmed video with a single natural‑language command, reducing manual editing time and lowering the skill barrier for quick video production.

<details><summary>References</summary>
<ul>
<li><a href="https://news.cocoloop.cn/en/2026/11/doubao-work-jianying-plugin/">Doubao Work adds Jianying plugin for one-sentence rough cuts</a></li>
<li><a href="https://cryptovka.com/news/doubao-work-integrates-jianying-plugin-for-ai-driven-video-editing">Doubao Work Integrates Jianying Plugin for AI-Driven Video ...</a></li>

</ul>
</details>

**Tags**: `#AI video editing`, `#natural language interface`, `#software tooling`, `#Chinese tech news`

---

<a id="item-tech-news-8"></a>
### [Ren Zhengfei credits US sanctions for Huawei’s push to self‑reliance and thanks Trump](https://thenextweb.com/news/ren-zhengfei-huawei-trump-thanks-nyt-interview) ⭐️ 7.0/10

Huawei founder Ren Zhengfei told the New York Times that U.S. sanctions have forced Huawei and China to become self‑reliant, describing the company as “our own country’s company” and asking the paper to convey his thanks to former President Trump. He added that China will eventually surpass the United States in chip technology, calling it only a matter of time.

telegram · zaihuapd · Nov 27, 16:35

**「Background on U.S. sanctions and Huawei’s self‑reliance」** The United States has imposed sanctions that restrict Huawei’s ability to obtain American chips, software and other technology, a policy that began under the Trump administration. Those restrictions have forced Huawei to accelerate its own chip development and broader self‑reliance strategy, a shift Ren Zhengfei highlighted in his recent interview.

**「Impact」** Ren’s remarks signal Huawei’s continued focus on domestic semiconductor development, which could increase investment in China’s chip‑design and manufacturing ecosystem and affect global supply‑chain dynamics.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/11/26/business/huawei-trump-china-ai.html">Trump Tried to Cripple Huawei . Now It Is Central to China’s A.I. Push.</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#US sanctions`, `#semiconductors`, `#technology industry`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China&\#x27;s State Council to Boost &quot;National Team&quot; and Optimize Stabilization Funds](https://www.tmtpost.com/nictation/8220182.html) ⭐️ 7.0/10

The State Council, chaired by Premier Li Qiang on Nov. 27, announced new policies to strengthen the &quot;national team&quot; in market stabilization and to enhance the central Huijin‑type &quot;stabilization fund&quot; function, ensuring ample liquidity and guiding long‑term funds such as insurance, pension and social security assets into equities.

telegram · zaihuapd · Nov 27, 05:35

**「Background」** The “national team” – state‑controlled investors such as Central Huijin – intervenes in the stock market to supply liquidity during downturns, and its “stabilization fund” \(平准基金\) is a mechanism for buying shares or ETFs to support market stability, previously used mainly in crisis periods.

<details><summary>References</summary>
<ul>
<li><a href="https://baike.baidu.com/item/%E5%9B%BD%E5%AE%B6%E9%98%9F/68623816">国家队（中国金融市场中的国家投资机构）_百度百科</a></li>
<li><a href="https://cj.sina.com.cn/articles/view/8267265960/1ecc477a8072019sv8">国家队稳市制度化，对A股生态有啥长远影响？_新浪财经</a></li>

</ul>
</details>

**Tags**: `#China`, `#capital markets`, `#government policy`, `#market stabilization`

---

<a id="item-finance-news-2"></a>
### [China central bank lowers large‑deposit certificate threshold to ¥100,000](https://www.news.cn/fortune/20261127/70789d77822242cc82216f51a416f872/c.html) ⭐️ 7.0/10

China&\#x27;s central bank reduced the minimum purchase amount for personal large‑deposit certificates to ¥100,000 \(down from ¥200,000\) and requires banks to set rates independently, with the rules effective from 21 March 2027.

telegram · zaihuapd · Nov 27, 11:36

**「Background」** The 2015 interim rules set the personal threshold at ¥200,000 and the institutional threshold at ¥10 million, and the new regulation replaces those rules.

**「Impact」** The lower threshold enables more retail investors to buy large‑denomination CDs, potentially expanding banks&\#x27; deposit base.

**Tags**: `#Monetary Policy`, `#Banking Regulation`, `#Deposits`, `#China`

---