---
layout: default
title: "Horizon Summary: 2026-11-12 (EN)"
date: 2026-11-12
lang: en
---

> From 52 items, 5 important content pieces were selected

---

**Technology News**
1. [Locking GitHub Actions with Workflow Lockfiles](#item-tech-news-1) ⭐️ 8.0/10
2. [Voltage‑glitch hack unlocks hidden memory on NVIDIA A100 mining cards](#item-tech-news-2) ⭐️ 7.0/10
3. [Operatic AI launches open‑source explorer for 2,100+ CoRL robotics papers](#item-tech-news-3) ⭐️ 7.0/10
4. [AMD AI-driven memory tiering claims up to 83% server cost reduction](#item-tech-news-4) ⭐️ 7.0/10

**Financial News**
1. [Alibaba to spin off AI chip unit T‑Head in Hong Kong](#item-finance-news-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Locking GitHub Actions with Workflow Lockfiles](https://hugovk.dev/blog/2026/lock-github-actions/) ⭐️ 8.0/10

The article explains how to use workflow lockfiles to pin GitHub Actions to specific commit hashes, thereby preventing unauthorized changes to action code in CI/CD pipelines. It provides step‑by‑step instructions for creating a lockfile, updating workflows to reference the lockfile, and verifying that only the intended versions run. The guide notes that the mechanism currently locks only standard action calls, while reusable workflows and composite actions require additional manual pinning.

hackernews · gslin · Nov 11, 22:16 · [Discussion](https://news.ycombinator.com/item?id=50459485)

**「Prerequisite: GitHub Actions workflow lockfiles」** GitHub Actions executes code from external repositories, and developers have traditionally mitigated supply‑chain risk by pinning actions to a specific commit SHA because tags are mutable. In October 2026 GitHub introduced workflow lockfiles—first in public preview on Oct 14 and then generally available on Oct 28—which generate a lockfile that records the exact versions of each action and its transitive dependencies. The lockfile can be committed to the repo and enforced with the gh‑actions‑lock extension.

**「Impact」** Adopting workflow lockfiles lets developers and DevOps teams harden their pipelines against supply‑chain attacks by ensuring actions cannot be silently altered, but they must also audit reusable workflows and composite actions separately to maintain full coverage.

**「Community Discussion」** Commenter woodruffw points out two limitations: the lockfile does not automatically lock reusable workflows, and composite actions are only locked indirectly through the workflows that call them, requiring extra manual pinning.

<details><summary>References</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-10-14-github-actions-workflow-lockfiles-in-public-preview/">GitHub Actions workflow lockfiles in public preview</a></li>
<li><a href="https://github.blog/changelog/2026-10-28-github-actions-workflow-lockfiles-are-generally-available/">GitHub Actions workflow lockfiles are generally available</a></li>

</ul>
</details>

**Tags**: `#GitHub Actions`, `#CI/CD`, `#Security`, `#DevOps`

---

<a id="item-tech-news-2"></a>
### [Voltage‑glitch hack unlocks hidden memory on NVIDIA A100 mining cards](https://blog.kate.land/posts/using-voltage-glitching-to-unlock-the-a100/) ⭐️ 7.0/10

A voltage‑glitching hardware hack can blow the fuses on NVIDIA A100 mining cards \(8 GB model\) to enable up to 80 GB of hidden HBM memory, effectively turning a low‑capacity card into a high‑memory GPU for AI workloads. The method is experimental, requires physical modification, and is not supported by NVIDIA.

hackernews · lae · Nov 11, 10:48 · [Discussion](https://news.ycombinator.com/item?id=50451903)

**「Background」** NVIDIA’s A100 GPUs sold for cryptocurrency mining are shipped with many of their streaming multiprocessors \(SMs\) and portions of HBM memory disabled by laser‑blown fuses to improve yield and lower cost. Voltage‑glitching is a fault‑injection technique that briefly drops the supply voltage to cause the fuse‑programming logic to mis‑interpret the intended state, allowing hidden hardware to be re‑enabled. This method has been demonstrated to recover up to the full 80 GB of HBM and enable all functional SMs, yielding about a 1.2× performance boost over the stock mining‑grade part.

**「Impact」** If successfully applied, the hack expands usable GPU memory by tenfold, allowing cheaper access to large‑memory compute for AI/ML tasks, but it carries a high risk of permanently damaging the card and is limited to users comfortable with hardware modifications.

**「Community Discussion」** Commenters expressed amazement at the hidden memory, warned about the risk of blowing fuses, and debated whether the fuses were set due to manufacturing defects; some suggested alternative approaches like external PCIe risers to speed the process.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.kate.land/posts/using-voltage-glitching-to-unlock-the-a100/">Using voltage glitching to unleash the A 100 in my mining card</a></li>
<li><a href="https://www.youtube.com/watch?v=16UcoPLdXD4">Glitching and Fault Injection: Finding the Right Voltage - YouTube</a></li>

</ul>
</details>

**Tags**: `#GPU`, `#Hardware Hacking`, `#AI Compute`, `#NVIDIA`, `#Memory Unlock`

---

<a id="item-tech-news-3"></a>
### [Operatic AI launches open‑source explorer for 2,100+ CoRL robotics papers](https://www.reddit.com/r/MachineLearning/comments/1xtul3j/i_built_an_explorer_of_2100_robotics_papers/) ⭐️ 7.0/10

A web‑based explorer now indexes more than 2,100 papers from the Conference on Robot Learning \(CoRL\) covering 2017‑2026, and presents each with a TLDR, links to code, project pages, arXiv entries, and task tags. The tool is hosted at https://corl.operatic.ai/explore and the source code is available on GitHub \(operatic‑ai/corl‑explorer\). It is intended for robotics researchers and developers who need quick access to prior work and trend statistics across a decade of robot learning research.

reddit · r/MachineLearning · /u/promptdom · Nov 11, 21:42

**「Conference on Robot Learning \(CoRL\)」** The Conference on Robot Learning \(CoRL\) is an annual international conference that focuses on research at the intersection of robotics and machine learning. Since its inception in 2017, CoRL has produced thousands of papers covering topics such as robot perception, control, and learning algorithms. The new explorer aggregates these papers, which were previously scattered across conference proceedings and repositories.

**「Impact」** Researchers can browse or clone the explorer to locate relevant papers, implementations, and datasets far faster than manual searching, streamlining literature reviews and reproducibility efforts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.corl.org/">CoRL 2026</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#research-tools`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [AMD AI-driven memory tiering claims up to 83% server cost reduction](https://www.theregister.com/systems/2026/11/11/amd-where-were-going-we-dont-need-as-much-dram/5308953) ⭐️ 7.0/10

AMD says its AI‑based Mext software can swap cold memory pages between DRAM and cheaper NVMe flash before the OS or applications notice, allowing roughly half of the DRAM to be replaced. The company claims this retains up to 99% of performance while potentially lowering enterprise server costs by as much as 83%. The feature is sold as a license that must be purchased with EPYC servers. These figures are AMD’s own estimates and have not been independently verified.

telegram · zaihuapd · Nov 11, 11:15

**「Predictive memory tiering with flash」** AMD’s MEXT \(Memory Extension\) software builds on its earlier acquisition of a memory‑tiering technology that uses AI to predict which memory pages are “cold” and can be moved from DRAM to lower‑cost NVMe flash before the operating system or application notices. The approach follows a broader industry trend of using flash‑based tiered memory to reduce reliance on expensive DRAM, a concept AMD has previously described as making flash behave like DRAM‑speed memory.

**「Impact」** If the performance and cost claims hold, data‑center operators could reduce DRAM purchases and overall server spend by buying the Mext license, but they will need to evaluate the licensing cost and any workload‑specific performance trade‑offs before adopting the technology.

<details><summary>References</summary>
<ul>
<li><a href="https://www.amd.com/en/products/software/mext.html">AMD MEXT Predictive Memory Software</a></li>
<li><a href="https://www.trendforce.com/news/2026/11/11/news-amd-taps-flash-based-mext-amid-memory-crunch-aims-to-cut-dram-needs-by-up-to-75/">[News] AMD Taps Flash-Based MEXT amid Memory Crunch, Aims to ...</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#systems`, `#AI`, `#cloud‑infrastructure`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Alibaba to spin off AI chip unit T‑Head in Hong Kong](https://www.cnbc.com/2026/11/11/alibaba-pr.html) ⭐️ 7.0/10

Alibaba announced it will seek approval to list its semiconductor subsidiary T‑Head on the Hong Kong Stock Exchange via a public offering, with no date or size disclosed.

rss · CNBC Finance · Nov 11, 07:47

**「Background」** The company filed a confidential listing request on Sept. 11; T‑Head develops AI chips such as the Zhenwu V900 to reduce reliance on U.S. technology amid tightening restrictions.

**「Impact」** Alibaba’s shares slipped about 1% after the announcement, affecting shareholders of the e‑commerce giant.

**Tags**: `#Alibaba`, `#Semiconductor IPO`, `#AI chips`, `#Hong Kong market`, `#Chinese tech sector`

---