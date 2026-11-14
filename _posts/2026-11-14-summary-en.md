---
layout: default
title: "Horizon Summary: 2026-11-14 (EN)"
date: 2026-11-14
lang: en
---

> From 40 items, 4 important content pieces were selected

---

**Technology News**
1. [GPU‑Accelerated Real‑Time Airband Decoder Streams All Frequencies](#item-tech-news-1) ⭐️ 7.0/10
2. [Claude Code 2.1.323 Adds Experimental JavaScript Code Mode](#item-tech-news-2) ⭐️ 7.0/10
3. [DeepSeek launches multimodal API suite for developers](#item-tech-news-3) ⭐️ 7.0/10

**Financial News**
1. [Fed President Goolsbee warns more action needed on inflation](#item-finance-news-1) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [GPU‑Accelerated Real‑Time Airband Decoder Streams All Frequencies](https://orcasairband.com/) ⭐️ 7.0/10

A hobbyist has built and deployed a system that captures and decodes the entire VHF airband in real time, using an Ettus B210 SDR front‑end and two RTX 4090 GPUs running CUDA. The GPU‑based polyphase channelizer demodulates all frequencies, filters out data transmissions, and streams the live audio from KORS, which proved especially useful during the recent ground stop affecting Victoria, CA.

hackernews · mmaunder · Nov 13, 22:04 · [Discussion](https://news.ycombinator.com/item?id=50490593)

**「Prerequisite concepts」** The airband refers to the range of VHF frequencies \(118‑137 MHz\) used for civil aviation voice communications, which can be captured with a software‑defined radio \(SDR\) front‑end such as an Ettus B210. A polyphase channelizer splits the wide‑band SDR stream into many narrow sub‑bands, and CUDA code running on GPUs \(e.g., dual RTX 4090s\) can perform this channelization and demodulation in real time, enabling live decoding of all active airband channels. This combination of SDR front‑ends and high‑throughput GPU processing makes it possible to monitor an entire region’s aviation chatter without dedicated hardware per frequency.

**「Impact」** Aviation enthusiasts, pilots and researchers can now monitor all regional airband communications—including ground‑stop announcements—in near‑real‑time, though the hobby‑level implementation yields partially garbled audio and is not a substitute for official ATC feeds.

**「Community Discussion」** Commenters noted the transmissions are often difficult to understand and compared the project to other hobby SDR efforts, such as a KiwiSDR‑based ship DSC decoder, highlighting both its novelty and practical limitations.

**Tags**: `#software engineering`, `#GPU computing`, `#software-defined radio`, `#real-time systems`

---

<a id="item-tech-news-2"></a>
### [Claude Code 2.1.323 Adds Experimental JavaScript Code Mode](https://code.claude.com/docs/en/changelog) ⭐️ 7.0/10

Claude Code version 2.1.323, released on November 12, adds an experimental Code Mode that lets Claude invoke tools using JavaScript, and can be disabled at the organization level. The update also tightens plugin management: plugins whose declared version ranges do not match the runtime will no longer be installed or updated, and the plugin validator now checks TypeScript hook types. Additional improvements include .docx document upload and a 30‑second hook heartbeat.

telegram · zaihuapd · Nov 13, 03:47

**「Prerequisite: Claude Code’s prior tool integration and plugin model」** Claude Code is Anthropic’s AI‑assisted coding assistant that already supports tool calls and a plugin system for extending its capabilities. Earlier releases allowed Claude to invoke predefined tools but did not provide a JavaScript‑based execution environment, and plugin validation only warned about mismatches without blocking installation. Understanding this prior architecture clarifies why the new experimental Code Mode—enabling JavaScript tool calls and enforcing strict version‑range checks for plugins—is a notable extension.

**「Impact」** Developers can script tool calls directly in JavaScript, enabling more flexible AI‑assisted coding workflows, but must enable the experimental mode and accommodate stricter plugin version requirements.

**Tags**: `#Claude`, `#AI coding assistant`, `#JavaScript`, `#plugin management`, `#software engineering`

---

<a id="item-tech-news-3"></a>
### [DeepSeek launches multimodal API suite for developers](https://mp.weixin.qq.com/s/78KBHc4-4N5b2vfL9SkutQ) ⭐️ 7.0/10

DeepSeek has opened its full‑suite application API, allowing developers to activate additional capabilities by setting parameters in the existing API. The V4.1‑Flash model now supports three multimodal endpoints, and the Search, Fetch, OCR, ASR and TTS functions can be called individually. An open‑source front‑end demo that can import prior conversation history has also been released, and the demo can be run locally via the provided GitHub repository.

telegram · zaihuapd · Nov 13, 14:27

**「Prerequisite: DeepSeek&\#x27;s earlier API offering」** DeepSeek previously provided a text‑only chat completion API that returned language responses based on user prompts. That service did not include built‑in tools for retrieving web content, performing optical character recognition, speech transcription, or speech synthesis, so developers had to integrate external services themselves. The new announcement builds on that baseline by adding multimodal parameters that automatically invoke search, fetch, OCR, ASR, and TTS functions within the same API call, and by releasing an open‑source front‑end demo for the V4.1‑Flash model.

**「Impact」** Developers can immediately add search, document retrieval, image OCR, speech‑to‑text and text‑to‑speech features to their applications without building separate services, simply by enabling the new flags in DeepSeek’s API. Existing integrations should be updated to include the new parameters to take advantage of the V4.1‑Flash multimodal capabilities.

**Tags**: `#DeepSeek`, `#Multimodal API`, `#AI Tools`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed President Goolsbee warns more action needed on inflation](https://www.cnbc.com/2026/11/13/chicago-feds-goolsbee-says-central-bank-has-definitely-got-work-to-do-on-inflation.html) ⭐️ 8.0/10

Chicago Fed President Austan Goolsbee warned that inflation remains above the 2% target, citing a 0.3% monthly rise and a 6.5% annual gain in the producer price index for October.

rss · CNBC Finance · Nov 13, 14:22

**「Recent inflation data」** The latest Bureau of Labor Statistics reports showed the producer price index rose 0.3% in October and was up 6.5% year‑over‑year—the strongest annual gain since November 2022, while the consumer price index also rose slightly above expectations, keeping inflation well above the Fed’s 2% target.

**「Impact」** If the Fed raises rates as markets anticipate, households and businesses could face higher borrowing costs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bls.gov/news.release/archives/ppi_11132026.htm">Producer Price Index News Release - 2026 M10 Results</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-11/fed-s-goolsbee-says-october-cpi-report-borderline-disturbing-mwbel9qz">Fed’s Goolsbee Says October CPI Report ‘Borderline Disturbing’</a></li>

</ul>
</details>

**Tags**: `#monetary policy`, `#inflation`, `#interest rates`, `#Fed`

---