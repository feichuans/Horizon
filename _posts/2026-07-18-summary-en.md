---
layout: default
title: "Horizon Summary: 2026-07-18 (EN)"
date: 2026-07-18
lang: en
---

> From 39 items, 20 important content pieces were selected

---

1. [Firefox compiled to WebAssembly runs inside a browser](#item-1) ⭐️ 9.0/10
2. [Thinking Machines Lab Releases Inkling, 975B Open-Weights Model](#item-2) ⭐️ 9.0/10
3. [First Atmosphere Found on Rocky Planet in Habitable Zone](#item-3) ⭐️ 8.0/10
4. [Moonshot AI Unveils Kimi K3, a 2.8T Open-Weight Model](#item-4) ⭐️ 8.0/10
5. [Open Source AI Surpasses Closed Models in Market Share](#item-5) ⭐️ 8.0/10
6. [GPT-5.6 Codex Bug Can Delete $HOME Directory](#item-6) ⭐️ 8.0/10
7. [Linus Torvalds: Linux Is Not Anti-AI](#item-7) ⭐️ 8.0/10
8. [Stereo2Spatial: AI Model Converts Stereo Music to Binaural Spatial Audio](#item-8) ⭐️ 8.0/10
9. [Kaiser Nurses Blame AI, Surveillance for Worse Care](#item-9) ⭐️ 7.0/10
10. [Zilog Z80 Microprocessor Celebrates 50th Anniversary](#item-10) ⭐️ 7.0/10
11. [Practical Tips for Running SQLite](#item-11) ⭐️ 7.0/10
12. [Texas Court Orders Domain Suspension Over Age-Verification Law](#item-12) ⭐️ 7.0/10
13. [Prism Bug Leaks Other Users' Papers](#item-13) ⭐️ 7.0/10
14. [EU AI Act OpenRAG: Structured Legal Corpus for RAG](#item-14) ⭐️ 7.0/10
15. [DABSN: New Recurrent LLM Architecture Seeks Collaborators](#item-15) ⭐️ 7.0/10
16. [Rethinking AI Memory: From Facts to Reasoning Patterns](#item-16) ⭐️ 7.0/10
17. [ExTernD: Ternary LLM Quantization with Near-Any Accuracy](#item-17) ⭐️ 7.0/10
18. [Recurse Center Founder Thanks HN for 15 Years of Support](#item-18) ⭐️ 6.0/10
19. [LLM Cliché Highlighter Tool Launched](#item-19) ⭐️ 6.0/10
20. [Offset data center water use by converting golf courses to parks](#item-20) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Firefox compiled to WebAssembly runs inside a browser](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter has compiled the full Firefox browser (Gecko engine) to WebAssembly, enabling it to run inside another browser like Chrome. The project used AI-assisted development with Claude Opus and Fable tokens, costing an estimated $25,000 in tokens but much less due to a subscription plan. This is a groundbreaking technical achievement that demonstrates the feasibility of running a full browser engine inside another browser, expanding the capabilities of WebAssembly. It could enable new use cases like secure sandboxed browsing, legacy browser emulation, and portable web-based applications. The demo uses the Wisp protocol to proxy all network traffic through Puter's server, as browser code cannot open arbitrary network connections. The project claims end-to-end encryption, verified by inspecting WebSocket messages where HTTPS traffic remained encrypted while HTTP traffic was in cleartext.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (Wasm) is a low-level binary instruction format that allows code written in languages like C++ to run in web browsers at near-native speed. Firefox's Gecko engine was chosen because it has strong single-process support, which simplifies the compilation to Wasm. The Wisp protocol is a low-overhead protocol for proxying multiple TCP/UDP sockets over a single WebSocket connection.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/HeyPuter/firefox-wasm">GitHub - HeyPuter/ firefox -wasm: Firefox in WebAssembly · GitHub</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was highly positive, with many impressed by the engineering feat. Some commenters noted the high cost of AI-assisted development and the scalability challenges of proxying traffic, as Puter had to scale servers to handle the traffic spike.

**Tags**: `#WebAssembly`, `#Firefox`, `#Browser`, `#Wasm`, `#Engineering`

---

<a id="item-2"></a>
## [Thinking Machines Lab Releases Inkling, 975B Open-Weights Model](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 9.0/10

Mira Murati's Thinking Machines Lab released Inkling, a 975B-parameter (41B active) Mixture-of-Experts multimodal model under Apache-2.0 license, trained on 45 trillion tokens of text, images, audio, and video. Inkling strengthens the US open-weights ecosystem with a competitive contender against Chinese open models, and its Apache-2.0 license encourages broad customization and fine-tuning via the Tinker platform. The model card and training data documentation are notably sparse, and Thinking Machines admits Inkling is not a frontier model but a strong base for fine-tuning. A smaller 276B (12B active) variant called Inkling-Small is promised but not yet released.

rss · Simon Willison · Jul 16, 15:35

**Background**: A Mixture-of-Experts (MoE) transformer activates only a subset of parameters per input, enabling larger total capacity with lower computational cost. Open-weights models release trained parameters publicly, allowing download and modification, but may not meet all open-source criteria. The Apache-2.0 license permits free use, modification, and distribution.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#Mira Murati`

---

<a id="item-3"></a>
## [First Atmosphere Found on Rocky Planet in Habitable Zone](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

JWST has confirmed the presence of an atmosphere on LHS 1140b, a rocky super-Earth in the habitable zone of a red dwarf star 48 light-years away, marking the first such detection for a relatively rocky exoplanet in a habitable zone. This discovery challenges previous assumptions that rocky planets around red dwarfs cannot retain atmospheres due to intense stellar activity, and it provides a prime target for future atmospheric characterization in the search for biosignatures. LHS 1140b is about 5.6 times Earth's mass and 70% larger in radius, with a density suggesting it may be an ocean world with 9-19% water by mass. The atmosphere was detected via JWST emission spectroscopy as the planet passed behind its star, ruling out a mini-Neptune scenario.

hackernews · neversaydie · Jul 17, 14:06 · [Discussion](https://news.ycombinator.com/item?id=48947560)

**Background**: Red dwarfs are cooler and smaller than the Sun, so their habitable zones are much closer, exposing planets to intense stellar flares and radiation that can strip atmospheres. LHS 1140b was discovered in 2017 and initially thought to be a dense rocky planet, but refined measurements revealed a lower density. The habitable zone is the region where liquid water could exist on a planet's surface.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LHS_1140_b">LHS 1140 b</a></li>
<li><a href="https://science.nasa.gov/exoplanet-catalog/lhs-1140-b/">LHS 1140 b - NASA Science</a></li>
<li><a href="https://www.bbc.com/news/articles/cy4kdd1e0ejo">First atmosphere found around Earth-like planet LHS 1140b</a></li>

</ul>
</details>

**Discussion**: Commenters expressed surprise that a rocky planet around a red dwarf could retain an atmosphere, with one noting that JWST data ruled out a mini-Neptune interpretation. Others speculated about future propulsion systems to reach the planet and discussed the Fermi paradox in the context of short communication windows.

**Tags**: `#exoplanets`, `#JWST`, `#astronomy`, `#habitable zone`, `#atmosphere`

---

<a id="item-4"></a>
## [Moonshot AI Unveils Kimi K3, a 2.8T Open-Weight Model](https://simonwillison.net/2026/Jul/16/kimi-k3/#atom-everything) ⭐️ 8.0/10

Moonshot AI announced Kimi K3, a 2.8 trillion parameter open-weight model, claiming it as the first open 3T-class model with open weights promised by July 27, 2026. Kimi K3 surpasses DeepSeek's 1.6T V4 Pro in size and competes with top proprietary models like Claude Opus 4.8 and GPT-5.5, marking a significant step for open-weight AI and intensifying competition among Chinese AI labs. Kimi K3 costs $3 per million input tokens and $15 per million output tokens, making it the most expensive Chinese AI model to date, and uses 21% fewer output tokens than its predecessor K2.6.

rss · Simon Willison · Jul 16, 20:19 · [Discussion](https://news.ycombinator.com/item?id=48947717)

**Background**: The 'pelican benchmark' is an informal test created by Simon Willison that asks an LLM to generate an SVG of a pelican riding a bicycle. It is used to qualitatively compare model capabilities, though it is not a rigorous benchmark. Open-weight models release their trained parameters publicly, allowing others to run and fine-tune them, unlike closed-source models.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/moonshotai/kimi-k3">Kimi K3 - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://fortune.com/2026/07/16/moonshots-kimi-k3-pushes-chinese-ai-into-fable-level-territory/">Moonshot’s Kimi K3 pushes Chinese AI into Fable-level territory | Fortune</a></li>

</ul>
</details>

**Discussion**: Commenters questioned the pelican benchmark's validity, noting that pelican SVGs may be in training data due to widespread use. Others highlighted hidden system prompts inflating token counts and the need for agentic tool-calling benchmarks. Some provided cost-speed comparisons showing Kimi K3 is cheapest but slowest among peers.

**Tags**: `#AI`, `#large language models`, `#open-source`, `#benchmarks`, `#Chinese AI`

---

<a id="item-5"></a>
## [Open Source AI Surpasses Closed Models in Market Share](https://stateofopensource.ai/) ⭐️ 8.0/10

A new analysis from Mozilla shows that open source AI models now command 63% of token processing volume on OpenRouter, up from 40% four months ago, representing a nearly 5x increase in total tokens processed. This shift indicates that open models are rapidly gaining adoption, potentially threatening the business models of closed-source AI companies like OpenAI and Anthropic, as hyperscalers and device makers can deploy open models without licensing fees. The data is based on OpenRouter usage statistics, with open models processing 4.19 trillion tokens on a recent day compared to 888 billion four months earlier. The analysis itself has been criticized for being LLM-generated and poorly structured.

hackernews · rellem · Jul 17, 14:31 · [Discussion](https://news.ycombinator.com/item?id=48947825)

**Background**: Open source AI models, such as Meta's Llama and Mistral, are freely available for use and modification, contrasting with closed models like GPT-4 that require API access or licensing. The debate centers on whether open models can match the performance of frontier closed models while offering cost and flexibility advantages.

**Discussion**: Commenters are divided: some celebrate the growth of open models as a threat to closed-source companies, while others criticize the Mozilla analysis as a poorly crafted LLM-generated presentation that undermines its credibility. One user built a dashboard to track the data daily.

**Tags**: `#open source`, `#AI`, `#LLMs`, `#market trends`, `#community analysis`

---

<a id="item-6"></a>
## [GPT-5.6 Codex Bug Can Delete $HOME Directory](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

OpenAI's GPT-5.6 Codex has a bug where, under full access mode without sandboxing, it may mistakenly delete the user's $HOME directory instead of a temporary directory. This bug highlights critical safety risks in AI coding agents, as it can cause irreversible data loss for developers using full access mode without proper safeguards. The bug occurs when the model attempts to override the $HOME environment variable to define a temporary directory, then mistakenly deletes $HOME instead. OpenAI has investigated and confirmed the issue.

rss · Simon Willison · Jul 16, 17:45

**Background**: Codex is OpenAI's AI coding agent that can execute commands and modify files. Full access mode disables sandboxing, giving the agent unrestricted system access. Without auto-review or sandboxing, the agent's actions are not vetted, increasing risk.

<details><summary>References</summary>
<ul>
<li><a href="https://openai-codex.mintlify.app/concepts/sandboxing">Sandboxing - Codex CLI</a></li>
<li><a href="https://www.digitalapplied.com/blog/gpt-5-6-file-deletion-agentic-blast-radius">GPT-5.6 Sometimes Deletes Files: Agentic Blast Radius</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#bug`

---

<a id="item-7"></a>
## [Linus Torvalds: Linux Is Not Anti-AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds publicly declared that Linux is not an anti-AI project, stating that AI is a clearly useful tool and warning dissenters to fork or leave. This strong endorsement from the Linux creator signals a major policy shift, potentially influencing the entire open-source ecosystem's stance on AI integration in kernel development. Torvalds made the statement on the Linux Media Mailing List, emphasizing that AI's usefulness is no longer in question, though economic questions remain.

rss · Simon Willison · Jul 16, 13:26

**Background**: Linux is the world's largest open-source operating system kernel, with Torvalds as its creator and top maintainer. AI tools, especially large language models, have been controversial in open-source communities due to concerns about code quality, licensing, and ethics.

**Tags**: `#Linux`, `#AI`, `#Open Source`, `#Kernel Development`

---

<a id="item-8"></a>
## [Stereo2Spatial: AI Model Converts Stereo Music to Binaural Spatial Audio](https://www.reddit.com/r/MachineLearning/comments/1uzevbg/stereo2spatial_convert_stereo_music_tracks_to/) ⭐️ 8.0/10

A new flow-matching diffusion model called Stereo2Spatial converts stereo music tracks into spatialized binaural mixes, using memory tokens to maintain stability over long audio contexts. The waveform-based version (v2) achieves high-quality output after adopting amplitude lifting from the WavFlow paper. This addresses a practical gap: most existing music lacks quality spatial mixes, and this model offers an open-source solution for upmixing stereo to binaural audio. It could enhance immersive listening experiences for consumers and provide a tool for audio engineers. The model was trained on 7,669 tracks for ~20 days on 2x A6000 GPUs, with two stages: first on sequences up to 34 seconds, then on 122-second sequences. The waveform version uses amplitude lifting (scaling RMS to 0.33, then multiplying by 3, with a clip of 4.0) to stabilize training.

reddit · r/MachineLearning · /u/kittenkrazy · Jul 17, 22:55

**Background**: Flow-matching diffusion models are a class of generative models that learn to transform noise into data by following a probability path. Memory tokens are trainable vectors that allow the model to carry state across windows, improving long-context generation. Binaural audio simulates how humans hear sound in 3D space using two channels.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2210.02747">[2210.02747] Flow Matching for Generative Modeling</a></li>
<li><a href="https://huggingface.co/earlab/EAR_VAE">earlab/ EAR _ VAE · Hugging Face</a></li>
<li><a href="https://www.emergentmind.com/topics/learned-memory-tokens">Learned Memory Tokens in Neural Models</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#audio processing`, `#spatial audio`, `#diffusion models`, `#music`

---

<a id="item-9"></a>
## [Kaiser Nurses Blame AI, Surveillance for Worse Care](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/) ⭐️ 7.0/10

Kaiser Permanente nurses report that AI and workplace surveillance tools, particularly call center metrics, are worsening job conditions and patient care, though some clinicians find value in medical LLMs. This highlights real concerns about misuse of metrics in healthcare, potentially affecting patient outcomes and nurse morale, while also showing the nuanced benefits of AI tools like medical LLMs. The majority of complaints focus on call center metrics and pressure to ration care, not AI itself; an AI empathy pilot was discontinued in 2024. Some nurses find medical LLMs helpful for translation, note summarization, and quick answers.

hackernews · gnabgib · Jul 17, 22:26 · [Discussion](https://news.ycombinator.com/item?id=48952880)

**Background**: Healthcare call center metrics track agent performance and patient experience, but when misused, they can pressure staff to prioritize speed over quality. Medical LLMs are large language models fine-tuned for clinical tasks, such as summarizing notes or answering medical queries. Kaiser Permanente is a large healthcare consortium that has been piloting various AI tools.

<details><summary>References</summary>
<ul>
<li><a href="https://medconnectusa.com/10-healthcare-call-center-metrics-you-should-be-tracking/">10 Healthcare Call Center Metrics You Should Be... - MedConnectUSA</a></li>
<li><a href="https://medium.com/@thomas.achache_66733/list/medical-llms-d5ced9a1b0dd">List: Medical LLMs | Curated by Thomas Achache | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters distinguish between misuse of metrics (a real concern) and AI benefits; some share positive experiences with medical LLMs, while others criticize the idea of using machines to evaluate empathy. A rural hospital nurse notes that tracking systems reduce time spent with patients.

**Tags**: `#AI in healthcare`, `#workplace surveillance`, `#nursing`, `#ethics`, `#Kaiser Permanente`

---

<a id="item-10"></a>
## [Zilog Z80 Microprocessor Celebrates 50th Anniversary](https://goliath32.com/blog/z80.html) ⭐️ 7.0/10

The Zilog Z80 microprocessor has turned 50, with a blog post and community discussion marking the milestone and reflecting on its enduring legacy. The Z80 was a foundational CPU that powered countless home computers, game consoles, and embedded systems, shaping the personal computing revolution and inspiring generations of programmers. The Z80 was fully binary compatible with the Intel 8080 but had differences in flag register behavior and repurposed undefined opcodes, making it not entirely compatible for all programs.

hackernews · st_goliath · Jul 17, 19:41 · [Discussion](https://news.ycombinator.com/item?id=48951461)

**Background**: Introduced in 1976 by Zilog, the Z80 was an 8-bit microprocessor that became widely used in systems like the ZX Spectrum, MSX, and Game Boy. Its instruction set was based on the Intel 8080 but added many new registers and instructions, making it more powerful and easier to program.

**Discussion**: Commenters shared nostalgic memories of learning assembly on Z80-based systems like the Timex Sinclair and ZX-81, with some noting the Exxon connection to Zilog and technical nuances about binary compatibility.

**Tags**: `#Z80`, `#microprocessor`, `#retrocomputing`, `#history`, `#CPU`

---

<a id="item-11"></a>
## [Practical Tips for Running SQLite](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 7.0/10

Julia Evans shares practical tips for running SQLite, including using the .expert mode for index recommendations and backup strategies like piping .dump to compression tools. These tips help developers optimize SQLite performance and ensure data safety, making SQLite more accessible for small to medium-scale applications. The .expert mode analyzes queries and suggests indexes; backups can be done with .dump piped to zstd for compression without blocking writers in WAL mode.

hackernews · surprisetalk · Jul 17, 17:45 · [Discussion](https://news.ycombinator.com/item?id=48950122)

**Background**: SQLite is a lightweight, embedded SQL database engine widely used in applications. The .expert mode is a CLI feature that recommends indexes to speed up queries. WAL (Write-Ahead Logging) mode allows concurrent reads and writes.

<details><summary>References</summary>
<ul>
<li><a href="https://databaseschool.com/series/high-performance-sqlite/videos/41">Where to add indexes - High Performance SQLite - Database School</a></li>
<li><a href="https://sqlite.work/sqlite-expert-mode-error-error-not-an-error-due-to-index-name-collision/">SQLite . expert Mode Error: "Error: not an error" Due to Index Name...</a></li>
<li><a href="https://sm-stackoverflow.azurefd.net/questions/16105662/sqlite-backup-strategy">sm-stackoverflow.azurefd.net/questions/16105662/ sqlite - backup ...</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the usefulness of .expert mode for avoiding manual query plan analysis, and share backup workflows using s3-credentials for AWS and zstd compression for efficient syncing.

**Tags**: `#SQLite`, `#database`, `#backup`, `#indexing`, `#tools`

---

<a id="item-12"></a>
## [Texas Court Orders Domain Suspension Over Age-Verification Law](https://www.texasattorneygeneral.gov/news/releases/attorney-general-ken-paxton-secures-landmark-legal-victory-lock-pornographic-website-domain-and) ⭐️ 7.0/10

Texas Attorney General Ken Paxton obtained a court order to suspend the domain name of a pornographic website for violating the state's age-verification law (HB 1181), which requires commercial sites with substantial sexually explicit material to verify users' ages before granting access. This ruling sets a significant legal precedent by allowing a state court to enforce internet censorship through domain suspension, potentially affecting interstate commerce and raising constitutional concerns about free speech and jurisdictional overreach. The court issued a default judgment because the website operator did not appear to defend itself, making the ruling legally binding but potentially less persuasive in future cases. The domain suspension effectively blocks access to the site across the entire internet, not just in Texas.

hackernews · letmevoteplease · Jul 17, 22:35 · [Discussion](https://news.ycombinator.com/item?id=48952939)

**Background**: Texas House Bill 1181, enacted on September 1, 2023, requires commercial websites hosting a substantial amount of sexually explicit material to verify users' ages before granting access. The law has been challenged on First Amendment grounds, and the U.S. Supreme Court is set to hear arguments in January 2025. Domain name suspensions are typically governed by ICANN policies and require a legal order or registrant violation.

<details><summary>References</summary>
<ul>
<li><a href="https://ondato.com/blog/new-texas-age-verification-law/">Texas Age Verification Law ( HB 1181 ) Explained | Ondato Blog</a></li>
<li><a href="https://www.sidley.com/en/insights/newsupdates/2025/07/texas-age-verification-law-upheld">Texas Age Verification Law Upheld... | Sidley Austin LLP</a></li>
<li><a href="https://www.nbcdfw.com/news/local/texas-news/a-timeline-of-the-legal-battle-over-texas-age-verification-law/3706903/">What is HB 1181 and why Texas AG is suing porn websites – NBC...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong concerns about jurisdictional overreach, with one noting that a state court in one state should not enforce such laws against companies with no local operations. Others highlighted potential violations of interstate commerce and warned of a slippery slope toward broader internet censorship, including targeting sites like GrapheneOS.

**Tags**: `#internet censorship`, `#age verification`, `#domain law`, `#interstate commerce`, `#legal precedent`

---

<a id="item-13"></a>
## [Prism Bug Leaks Other Users' Papers](https://www.reddit.com/r/MachineLearning/comments/1uz75qt/prism_accidentally_leaked_d/) ⭐️ 7.0/10

A bug in OpenAI's Prism platform caused the compilation process to return other users' unpublished papers instead of the intended document, as reported on Reddit and Twitter. This privacy breach could expose unpublished research, undermining trust in cloud-based research platforms and raising serious concerns for the machine learning community. The bug was first flagged on Discord and Twitter, and Prism took the website down within 10 minutes of the report. Users are worried their own papers may have been leaked.

reddit · r/MachineLearning · /u/Few-Monitor5103 · Jul 17, 17:59

**Background**: Prism is a free, AI-native research environment launched by OpenAI, featuring a LaTeX workspace with GPT-5.2 integration. It is designed for scientists and researchers to write, collaborate, and reason in one place.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-prism/">Introducing Prism | OpenAI</a></li>
<li><a href="https://essayhub.com/blog/how-safe-is-openai-prism-for-research">How Safe is OpenAI Prism as a Workspace for Scientists</a></li>
<li><a href="https://chatgpt2notion.com/blog/2026-01-28-openai-prism-launch-en/">OpenAI Launches Prism : Free Research Collaboration Platform ...</a></li>

</ul>
</details>

**Discussion**: The Reddit community expressed concern and commended Prism's quick response, but many remain worried about the potential exposure of their unpublished work.

**Tags**: `#privacy`, `#security`, `#machine learning`, `#bug`, `#research`

---

<a id="item-14"></a>
## [EU AI Act OpenRAG: Structured Legal Corpus for RAG](https://www.reddit.com/r/MachineLearning/comments/1uytlac/eu_ai_act_openrag_933_legally_structured_chunks/) ⭐️ 7.0/10

A new dataset called EU AI Act OpenRAG has been released, containing 933 legally structured chunks of the EU AI Act with BGE-M3 embeddings in a single SQLite file. It outperforms baseline sliding-window chunking on retrieval tasks like scenario article recall@20 (0.541 vs 0.449) and QA article hit@10 (0.927 vs 0.898). This resource enables more accurate retrieval-augmented generation (RAG) for legal AI applications, particularly for compliance with the EU AI Act. The structural chunking approach preserves legal semantics, which is critical for regulatory tasks. The SQLite database includes 1024-dimensional BGE-M3 embeddings, exact EUR-Lex links, Article 113 application-date metadata, and deliberately narrow derived labels. Direct textual classification is stored separately from broader regulatory-regime association, with ambiguous cases left as NULL.

reddit · r/MachineLearning · /u/Automatic-Forever-63 · Jul 17, 08:18

**Background**: Retrieval-Augmented Generation (RAG) is a technique that allows large language models to retrieve relevant information from external sources before generating answers. BGE-M3 is a multilingual embedding model supporting dense, sparse, and multi-vector retrieval. EUR-Lex is the official online database of European Union law. The EU AI Act (Regulation 2024/1689) is a landmark regulation governing artificial intelligence.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/BAAI/bge-m3?ref=blog-ko.allganize.ai">BAAI/ bge - m 3 · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval - augmented generation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/EUR-Lex">EUR-Lex</a></li>

</ul>
</details>

**Discussion**: The community discussion on Reddit was substantive, with users validating the approach and providing feedback on retrieval evaluation and additional baselines. The author actively engaged, requesting technical feedback on the methodology.

**Tags**: `#RAG`, `#Legal NLP`, `#AI Act`, `#Embeddings`, `#SQLite`

---

<a id="item-15"></a>
## [DABSN: New Recurrent LLM Architecture Seeks Collaborators](https://www.reddit.com/r/MachineLearning/comments/1uycffg/seeking_collaborators_for_scaling_and_independent/) ⭐️ 7.0/10

The author introduces DABSN (Dynamic Adaptive Bias State Network), a new recurrent language model architecture, and releases a preprint with PyTorch, C++, and Triton implementations. They also trained a 24M-parameter language model on 1B tokens and are seeking collaborators for scaling and independent evaluation. If validated, DABSN could offer an efficient alternative to transformers for long-context modeling, potentially reducing computational costs. The open call for collaboration and independent reproduction strengthens reproducibility in the field. The architecture was evaluated on benchmarks like MQAR, Copy, Key-Value retrieval, and A5/60. The author plans a second paper focusing on language modeling, long-context behavior, and scaling, and seeks help with independent reproduction, stronger baselines, or access to larger GPU clusters.

reddit · r/MachineLearning · /u/BleedingXiko · Jul 16, 19:17

**Background**: Recurrent architectures like LSTMs were dominant before transformers, but transformers excel at parallelization and long-range dependencies. Recently, models like Mamba have revived interest in recurrent designs for efficiency. DABSN is a new recurrent architecture aiming to combine efficiency with strong performance on reasoning and memory tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/multi-query-associative-recall-mqar">MQAR : Multi-Query Associative Recall</a></li>

</ul>
</details>

**Discussion**: No comments are provided in the news item, so community discussion is not available.

**Tags**: `#recurrent architecture`, `#language model`, `#scaling`, `#open source`, `#machine learning`

---

<a id="item-16"></a>
## [Rethinking AI Memory: From Facts to Reasoning Patterns](https://www.reddit.com/r/MachineLearning/comments/1uy6yht/are_current_ai_memory_architectures_optimizing/) ⭐️ 7.0/10

A Reddit post proposes that future AI memory systems should shift from storing descriptive facts (e.g., user interests) to inferring higher-level reasoning patterns, such as explanatory frameworks and characteristic reasoning styles. This idea challenges the current design of AI memory architectures, which primarily focus on factual recall, and could lead to more personalized and adaptive AI systems that better understand how users think. The author contrasts current memory (e.g., 'user likes economics') with a proposed model that infers patterns like 'user explains economics via incentives and institutional constraints.' The post questions whether such representations require fundamentally different architectures.

reddit · r/MachineLearning · /u/Boris_Ljevar · Jul 16, 16:00

**Background**: Current AI memory systems, such as those used in chatbots and agents, store persistent context as factual summaries (e.g., user preferences, conversation history). Cognitive architectures provide scaffolding for reasoning and goal-directed behavior, but they typically separate memory from reasoning. The post suggests merging memory with reasoning by continuously refining stored patterns into higher-level abstractions.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@nraman.n6/memory-architectures-in-ai-multiagent-systems-c6e98d331532">Memory Architectures in AI Multiagent Systems | Medium</a></li>
<li><a href="https://atlan.com/know/agent-memory-architectures/">Agent Memory Architectures : 5 Patterns and Trade-offs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cognitive_architecture">Cognitive architecture - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI memory`, `#persistent context`, `#reasoning patterns`, `#machine learning`, `#cognitive architectures`

---

<a id="item-17"></a>
## [ExTernD: Ternary LLM Quantization with Near-Any Accuracy](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 7.0/10

ExTernD proposes a post-training quantization method that decomposes each LLM weight matrix into two ternary matrices and a diagonal scaling matrix, allowing the inner rank to be arbitrarily expanded to achieve accuracy approaching any desired level. This approach overcomes the fixed-matrix-size limitation of previous ternary quantization, enabling high accuracy with only a modest increase in VRAM, which could significantly improve LLM deployment efficiency on resource-constrained hardware. The method requires only slightly more VRAM than current quantization methods, and the author demonstrates that the expanded rank does not need to be very large to achieve near-lossless accuracy.

reddit · r/MachineLearning · /u/LMTLS5 · Jul 16, 13:31

**Background**: Post-training quantization (PTQ) reduces model size and speeds up inference by converting weights to lower precision, such as ternary values (-1, 0, +1). However, previous ternary PTQ methods were limited by fixed matrix size, which constrained accuracy. ExTernD addresses this by using a rank-expanded ternary decomposition.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2607.13511">ExTernD: Expanded - Rank Ternary Decomposition Ternary LLM PTQ...</a></li>
<li><a href="https://github.com/LMTLS5/ternary-decomposition">GitHub - LMTLS5/ ternary -decomposition · GitHub</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#ternary`, `#efficiency`, `#PTQ`

---

<a id="item-18"></a>
## [Recurse Center Founder Thanks HN for 15 Years of Support](https://news.ycombinator.com/item?id=48949551) ⭐️ 6.0/10

The founder of the Recurse Center, a free self-directed programming retreat, posted a thank-you note on Hacker News celebrating 15 years since the program's first day, crediting an earlier HN post for helping launch the retreat and reach a global audience. This milestone highlights the enduring impact of community-driven platforms like HN in launching and sustaining educational initiatives that have positively affected over 3,000 programmers, and underscores the viability of non-traditional, free educational models supported by integrated recruiting agencies. The Recurse Center (originally Hacker School) was founded after a failed Y Combinator startup idea and launched on HN in 2011; it remains free for participants, funded by a recruiting agency where companies pay to hire alumni, and has remained HN as its #2 source of applicants after word of mouth.

hackernews · nicholasjbs · Jul 17, 16:57

**Background**: The Recurse Center is a self-directed, free programming retreat in New York City where participants work on their own projects without formal curriculum or instructors. It combines an educational retreat with a recruiting agency to sustain its free model. The program has been an advocate for women in programming and switched to online during the pandemic before reopening its physical space in 2023.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recurse_Center">Recurse Center - Wikipedia</a></li>
<li><a href="https://www.ycombinator.com/companies/recurse-center">Recurse Center: The retreat where curious programmers recharge...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed gratitude and shared personal experiences, with one recalling fond memories of the retreat in NYC over a decade ago. Others asked about changes in applicant demographics over 15 years and noted the clever business model of keeping the retreat free through a recruiting agency.

**Tags**: `#programming retreat`, `#community`, `#education`, `#startup story`

---

<a id="item-19"></a>
## [LLM Cliché Highlighter Tool Launched](https://simonwillison.net/2026/Jul/17/llm-cliche-highlighter/#atom-everything) ⭐️ 6.0/10

Simon Willison released a web tool called LLM cliché highlighter that detects and highlights common clichéd phrases in LLM-generated text, such as "no fluff, no filler, no jargon." This tool helps readers quickly identify AI-written content by flagging overused patterns, addressing growing frustration with formulaic LLM writing. It empowers users to critically evaluate text authenticity in an era of widespread AI-generated content. The tool highlights ten common patterns and can load text from a URL via r.jina.ai. It was built using Fable 5 vibe coding, an Anthropic model optimized for end-to-end app development.

rss · Simon Willison · Jul 17, 12:11

**Background**: LLMs like GPT-4 and Claude often produce text with distinctive clichés (e.g., "delve into," "it's worth noting") due to training data biases. Vibe coding refers to using AI models to generate entire applications from natural language prompts, reducing manual coding effort.

<details><summary>References</summary>
<ul>
<li><a href="https://tools.simonwillison.net/llm-cliche-highlighter">LLM cliché highlighter</a></li>
<li><a href="https://simonwillison.net/2026/Jul/17/llm-cliche-highlighter/">Tool: LLM cliché highlighter | Simon Willison’s Weblog</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#writing`, `#tool`, `#AI detection`

---

<a id="item-20"></a>
## [Offset data center water use by converting golf courses to parks](https://simonwillison.net/2026/Jul/17/spot-birds-not-golf/#atom-everything) ⭐️ 6.0/10

A proposal suggests hyperscalers like Google could offset their data center water consumption by purchasing golf courses and converting them into public parks, using the saved water to compensate for their usage. This creative idea highlights the significant water footprint of AI and data centers, and proposes a tangible, local offset strategy that could also provide community benefits. Google used 10.9 billion gallons of water in 2025 (about 30 million gallons per day). The Coachella Valley has 120 golf courses each using ~800 acre-feet per year (~750,000 gallons per day), so buying 40 courses could offset Google's daily usage.

rss · Simon Willison · Jul 17, 02:58

**Background**: Data centers, especially hyperscale facilities powering AI, consume vast amounts of water for cooling. An acre-foot is a US unit of water volume equal to about 325,851 gallons, commonly used for large-scale water measurement. Golf courses are notoriously water-intensive, making them a target for water conservation efforts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.weforum.org/stories/2026/01/ai-water-data-centres-opportunity-am26-wef-xylem/">Why AI's water problem might actually be an opportunity</a></li>
<li><a href="https://www.coloradoriverdistrict.org/water-measurement/">Water Measurement - Basic Units of Water | Colorado River District</a></li>

</ul>
</details>

**Tags**: `#ai-energy-usage`, `#data-centers`, `#water-conservation`, `#sustainability`

---