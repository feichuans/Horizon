---
layout: default
title: "Horizon Summary: 2026-07-17 (EN)"
date: 2026-07-17
lang: en
---

> From 38 items, 27 important content pieces were selected

---

1. [xAI Open-Sources Grok Build After Privacy Backlash](#item-1) ⭐️ 9.0/10
2. [Moonshot AI Releases Kimi K3: 2.8T Parameter Open-Weight Model](#item-2) ⭐️ 8.0/10
3. [LM Studio Bionic: AI Agent for Open Models](#item-3) ⭐️ 8.0/10
4. [Rust-to-Zig Compiler Rewrite: Progress Report](#item-4) ⭐️ 8.0/10
5. [Firefox Runs Inside Chrome via WebAssembly](#item-5) ⭐️ 8.0/10
6. [Thinking Machines Lab Releases Inkling Open-Weights Model](#item-6) ⭐️ 8.0/10
7. [Linus Torvalds Declares Linux Not Anti-AI](#item-7) ⭐️ 8.0/10
8. [Prompt injection bypasses Claude's web_fetch data exfiltration protection](#item-8) ⭐️ 8.0/10
9. [QLoRA default learning rate 2e-4 is wrong for small datasets](#item-9) ⭐️ 8.0/10
10. [ExTernD: Ternary LLM Quantization Nears Full Precision](#item-10) ⭐️ 8.0/10
11. [PnP-CoSMo: Content/Style Modeling for MRI Reconstruction](#item-11) ⭐️ 8.0/10
12. [Schema Harness Claims 99% on ARC-AGI-3](#item-12) ⭐️ 8.0/10
13. [Disentangling a Convolutional Neuron via Hadamard Product](#item-13) ⭐️ 8.0/10
14. [PyTorch model 170x slower on T4 vs A100: memory bandwidth bottleneck](#item-14) ⭐️ 8.0/10
15. [Microsoft Comic Chat Open-Sourced After 30 Years](#item-15) ⭐️ 7.0/10
16. [Decoy Font: Hiding Text from AI](#item-16) ⭐️ 7.0/10
17. [Classical ML for LLM Text Detection](#item-17) ⭐️ 7.0/10
18. [OnePlus Halts New Product Launches in US and Europe](#item-18) ⭐️ 7.0/10
19. [Interactive Linear Algebra Book Wins Praise](#item-19) ⭐️ 7.0/10
20. [GPT-5.6 Codex Bug Can Delete $HOME Directory](#item-20) ⭐️ 7.0/10
21. [DABSN: New Recurrent Architecture Seeks Collaborators](#item-21) ⭐️ 7.0/10
22. [Rethinking AI Memory: From Facts to Reasoning Patterns](#item-22) ⭐️ 7.0/10
23. [Seeking Devil's Advocate Critique of JEPA Models](#item-23) ⭐️ 7.0/10
24. [uv 0.11.29 Adds JSON Output and CUDA 13.2 Support](#item-24) ⭐️ 6.0/10
25. [Mermaid to ASCII Art with Color via WebAssembly](#item-25) ⭐️ 6.0/10
26. [RTCA Workshop at NeurIPS 2026: Call for Papers](#item-26) ⭐️ 6.0/10
27. [Best Python Tools for Multi-Objective Surrogate-Based Optimization](#item-27) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [xAI Open-Sources Grok Build After Privacy Backlash](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 9.0/10

xAI has open-sourced the entire Grok Build codebase under the Apache 2.0 license after its CLI tool was found to upload entire directories to the cloud, including sensitive user data. The company also deleted all retained coding data and disabled default data retention. This incident highlights critical privacy risks in AI-powered developer tools and underscores the importance of transparency and open-source practices for building user trust. The open-sourcing of a large Rust codebase (844,530 lines) also provides valuable insights for the developer community. The Grok Build repository contains 844,530 lines of Rust code with only about 3% vendored, and includes a self-contained Mermaid diagram renderer and tool implementations inspired by other coding agents. The initial release is a single commit, so no development history is available.

rss · Simon Willison · Jul 15, 23:59

**Background**: The Grok CLI is a terminal-based coding agent powered by xAI's Grok models. It was designed to assist developers with complex coding tasks directly from the command line. The privacy issue arose because the tool, by default, uploaded the entire working directory to xAI's cloud servers, which could include sensitive files like SSH keys and password databases.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apache_License">Apache License</a></li>
<li><a href="https://github.com/superagent-ai/grok-cli">GitHub - superagent-ai/ grok - cli : An open-source coding agent for the...</a></li>

</ul>
</details>

**Discussion**: The community expressed strong backlash over the data upload behavior, with users reporting exposure of SSH keys and password managers. The open-sourcing move was seen as a positive step to rebuild trust, though some remained skeptical about xAI's data handling practices.

**Tags**: `#security`, `#open source`, `#AI`, `#privacy`, `#xAI`

---

<a id="item-2"></a>
## [Moonshot AI Releases Kimi K3: 2.8T Parameter Open-Weight Model](https://www.kimi.com/blog/kimi-k3) ⭐️ 8.0/10

Moonshot AI has released Kimi K3, an open-weight frontier model with 2.8 trillion parameters, a 1 million token context window, and competitive pricing at $3 per million input tokens. It is the first open model to reach 2.8 trillion parameters and is claimed to be competitive with leading models like Anthropic's Sonnet series. Kimi K3 represents a significant step in Chinese AI labs pushing the frontier of open-weight models, potentially commoditizing AI intelligence and challenging US dominance. Its competitive pricing and performance could accelerate adoption of open models in production, while sparking debate on the geopolitical and economic implications of Chinese AI progress. The model uses Kimi Delta Attention, a hybrid linear attention mechanism, and Attention Residuals. It supports text and image input, outputs text, and has a 1M token context window. Pricing is $3/$15 per million tokens for input/output, with cached input at $0.3, matching Anthropic's Sonnet pricing.

hackernews · vincent_s · Jul 16, 14:46 · [Discussion](https://news.ycombinator.com/item?id=48935342)

**Background**: Moonshot AI is a Beijing-based AI company founded in 2023 by Tsinghua University alumni, and is one of China's 'AI Tigers' competing against US frontier labs. Open-weight models release the trained parameters publicly, allowing anyone to download and use them, though they may not be fully open-source. Kimi K3 follows a trend of Chinese labs releasing large open-weight models, such as DeepSeek's V4 series.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://artificialanalysis.ai/models/kimi-k3">Kimi K 3 - Intelligence, Performance & Price Analysis</a></li>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K 3 - Kimi API Platform</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the model's high cost for reasoning-heavy tasks (e.g., $0.25 for a single rendering), but acknowledge its frontier-level performance. Some debate whether Chinese labs are commoditizing intelligence to sell hardware, while others note the immense investment required. Overall sentiment is cautiously optimistic, with comparisons to Anthropic's Sonnet and DeepSeek's models.

**Tags**: `#AI`, `#LLM`, `#open-source`, `#pricing`, `#China`

---

<a id="item-3"></a>
## [LM Studio Bionic: AI Agent for Open Models](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 8.0/10

LM Studio has launched Bionic, a new AI agent app for open models that enables local agentic workflows for coding, document work, and research, with voice input and flexible model execution options. Bionic brings agentic capabilities to local open models, offering a familiar UI and enterprise-friendly features like data security and cost control, potentially accelerating adoption of local AI agents. Bionic supports running models locally, via LM Link, or through LM Studio Secure Cloud for larger frontier open models. It includes automatic checkpointing for document projects and integrates with existing LM Studio model libraries.

hackernews · minimaxir · Jul 16, 20:18 · [Discussion](https://news.ycombinator.com/item?id=48939662)

**Background**: LM Studio is a popular desktop app for running open-source language models locally. Agentic workflows allow AI to autonomously perform multi-step tasks like coding or document editing, traditionally requiring cloud-based services. Bionic aims to bring this capability to local models, addressing privacy and cost concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://lmstudio.ai/blog/introducing-lm-studio-bionic">Introducing LM Studio Bionic : the AI agent for open models</a></li>
<li><a href="https://9to5mac.com/2026/07/16/lm-studio-expands-beyond-chat-with-bionic-a-new-ai-agent-app-for-open-models/">LM Studio launches Bionic , a new AI agent app for open... - 9to5Mac</a></li>
<li><a href="https://daily.dev/posts/the-best-local-agentic-coding-workflow-complete-guide--ejgw3lkco">The Best LOCAL Agentic Coding Workflow (Complete Guide) | daily.dev</a></li>

</ul>
</details>

**Discussion**: Community feedback is positive overall, with users praising the familiar UI and smooth integration with local models. Some users noted rough edges and expressed concerns about the business model shift toward cloud services, while the founder actively engaged by offering credits for testing.

**Tags**: `#AI`, `#open-source`, `#agent`, `#local models`, `#LM Studio`

---

<a id="item-4"></a>
## [Rust-to-Zig Compiler Rewrite: Progress Report](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

The author details their experience rewriting a compiler from Rust to Zig, citing Zig's superior memory control and safety features as key motivations. This post sparks debate on the necessity of unsafe code in compilers and highlights Zig's growing appeal for systems programming, potentially influencing language adoption trends. The rewrite focuses on a compiler that emits machine code, where the author argues memory-unsafe operations are inherent. Zig's ReleaseSafe mode catches use-after-free errors at runtime via panics.

hackernews · jorangreef · Jul 16, 11:39 · [Discussion](https://news.ycombinator.com/item?id=48933149)

**Background**: Rust and Zig are both modern systems programming languages. Rust emphasizes memory safety without garbage collection via its ownership system, while Zig offers explicit memory control with optional runtime safety checks. Compilers often require low-level memory manipulation, making them a testbed for language trade-offs.

<details><summary>References</summary>
<ul>
<li><a href="https://pedropark99.github.io/zig-book/Chapters/01-memory.html">3 Memory and Allocators – Introduction to Zig</a></li>
<li><a href="https://ziggit.dev/t/ai-distracted-by-zig/9147">AI distracted by Zig - News - Ziggit</a></li>
<li><a href="https://piembsystech.com/how-to-optimize-your-code-effectively-in-zig-programming/">How to Optimize Your Code Effectively in Zig Programming...</a></li>

</ul>
</details>

**Discussion**: Steveklabnik argues that emitting machine code does not inherently require unsafe code, except for features like hot patching. Landr0id questions Zig's ability to catch use-after-free, noting no documentation evidence. Arthurbrown wonders why OCaml was not chosen, given its maturity and use in Rust's early compiler.

**Tags**: `#Rust`, `#Zig`, `#compilers`, `#memory safety`, `#programming languages`

---

<a id="item-5"></a>
## [Firefox Runs Inside Chrome via WebAssembly](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 8.0/10

Puter has compiled the full Firefox browser (Gecko engine) to WebAssembly, enabling it to run inside another browser like Chrome. A live demo shows a blog loaded within Firefox running in Chrome. This proof-of-concept demonstrates extreme portability for complex native applications on the web, with potential implications for security sandboxing and cross-platform compatibility. It also highlights the growing capability of WebAssembly to run large-scale software. The project used an estimated $25,000 worth of AI tokens (Claude Opus and Fable) but cost less due to a subscription plan. All network traffic is proxied via the Wisp protocol over WebSocket because browser code cannot open arbitrary network connections.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (WASM) is a low-level binary instruction format that runs in modern web browsers at near-native speed. Emscripten is a toolchain that compiles C/C++ code to WASM. The Gecko engine is Firefox's browser engine, chosen for its strong single-process support, which simplifies the WASM port.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/HeyPuter/firefox-wasm">GitHub - HeyPuter/ firefox -wasm: Firefox in WebAssembly · GitHub</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low ...</a></li>
<li><a href="https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/">Firefox in WebAssembly</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was highly positive, with many impressed by the engineering feat. Some raised concerns about the cost of proxying all traffic through Puter's servers, which the team had to scale up to handle the load.

**Tags**: `#WebAssembly`, `#Firefox`, `#browser`, `#compilation`, `#demo`

---

<a id="item-6"></a>
## [Thinking Machines Lab Releases Inkling Open-Weights Model](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

Thinking Machines Lab, led by Mira Murati, released Inkling, an open-weights multimodal Mixture-of-Experts model with 975B total parameters (41B active), licensed under Apache-2.0 and trained on 45 trillion tokens of text, images, audio, and video. This release strengthens the US open-weights ecosystem, providing a competitive alternative to Chinese open models and NVIDIA Nemotron, while offering a strong base for fine-tuning via the Tinker platform. Inkling is not a frontier model but a strong base for customization; a smaller variant, Inkling-Small (276B total, 12B active), is still being tested. The model card and training data documentation are notably sparse.

rss · Simon Willison · Jul 16, 15:35

**Background**: Mixture-of-Experts (MoE) models use multiple specialized sub-networks (experts) and activate only a subset per input, enabling larger total parameters with lower computational cost. Open-weights models make trained parameters publicly available, allowing modification and fine-tuning under permissive licenses like Apache-2.0.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apache_License">Apache License</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#Mira Murati`

---

<a id="item-7"></a>
## [Linus Torvalds Declares Linux Not Anti-AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds, the top Linux maintainer, stated on the Linux Media mailing list that Linux is not an anti-AI project and that AI is a clearly useful tool, dismissing objections and suggesting dissenters can fork the project or walk away. This authoritative endorsement from the project's leader could shape Linux's direction regarding AI integration, influencing the broader open-source community's stance on AI tools in development. Torvalds emphasized that AI's usefulness is no longer in question, though he acknowledged other open questions like the economy of AI. He made the statement in response to community pushback against AI in kernel development.

rss · Simon Willison · Jul 16, 13:26

**Background**: The Linux kernel is the core of the Linux operating system, maintained by Linus Torvalds and a large community. AI tools, such as large language models, have been increasingly used in software development for tasks like code generation and bug fixing, but some open-source contributors have raised ethical and practical concerns.

**Tags**: `#Linux`, `#AI`, `#Open Source`, `#Kernel Development`

---

<a id="item-8"></a>
## [Prompt injection bypasses Claude's web_fetch data exfiltration protection](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

Researcher Ayush Paul demonstrated a prompt injection attack that exploits a loophole in Claude's web_fetch tool, allowing an attacker to exfiltrate private user memories by tricking the model into following nested links from a malicious page. This attack bypasses Anthropic's designed protections against data exfiltration, highlighting a critical security gap in AI agents that combine access to private data with web browsing capabilities, and underscores the ongoing challenge of securing LLM-based systems. The attack works because web_fetch was allowed to visit URLs embedded in previously fetched pages, enabling a honeypot site to guide the agent through a chain of links to exfiltrate data. Anthropic had already identified the issue internally and closed the hole by removing that ability before the public disclosure.

rss · Simon Willison · Jul 15, 14:21

**Background**: Prompt injection attacks exploit the inability of large language models (LLMs) to distinguish between trusted instructions and untrusted user or web content. Data exfiltration occurs when an attacker tricks the model into sending private data to an external server. Claude's web_fetch tool was designed with safeguards to prevent such attacks, but this research found a loophole in the design.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/Data_exfiltration">Data exfiltration</a></li>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Platform Docs</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (via the provided link) likely includes comments on the cleverness of the attack and concerns about AI safety, though specific comments are not provided here.

**Tags**: `#AI safety`, `#prompt injection`, `#security`, `#Claude`, `#data exfiltration`

---

<a id="item-9"></a>
## [QLoRA default learning rate 2e-4 is wrong for small datasets](https://www.reddit.com/r/MachineLearning/comments/1uy1z8b/the_qlora_2e4_default_is_wrong_under_10k_samples/) ⭐️ 8.0/10

A Reddit user discovered that the default learning rate of 2e-4 for QLoRA fine-tuning causes overfitting on datasets with fewer than 10,000 samples, and reducing it to 1e-4 while increasing epochs significantly improves evaluation performance. This finding challenges a widely-adopted default in the LLM fine-tuning community, potentially saving practitioners time and resources by preventing overfitting on small datasets. It highlights the need for hyperparameter tuning based on dataset size rather than blindly following defaults. The user reports that with 2e-4 learning rate, the model overfits within the first epoch, causing evaluation loss to stagnate or increase. Switching to 1e-4 and increasing epochs from 3 to 5 led to a significant jump in evaluation metrics, confirmed over multiple runs.

reddit · r/MachineLearning · /u/Pretty-Ad774 · Jul 16, 12:50

**Background**: QLoRA is a parameter-efficient fine-tuning method that combines quantization and Low-Rank Adaptation (LoRA) to reduce memory usage. The default learning rate of 2e-4 originates from the Alpaca dataset (52k samples) and is commonly used in tutorials and documentation. However, for smaller datasets, this learning rate can be too aggressive, leading to overfitting.

<details><summary>References</summary>
<ul>
<li><a href="https://tensoria.fr/en/blog/lora-qlora-fine-tuning-guide">LoRA and QLoRA: A Practical Guide to Fine-tuning LLMs on a Budget | Tensoria</a></li>
<li><a href="https://lightning.ai/pages/community/lora-insights/">Finetuning LLMs with LoRA and QLoRA : Insights from... - Lightning AI</a></li>
<li><a href="https://www.geeksforgeeks.org/deep-learning/fine-tuning-using-lora-and-qlora/">Fine-Tuning using LoRA and QLoRA - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: The Reddit post received strong community validation with high upvotes and substantive discussion. Many users shared similar experiences of overfitting on small datasets with the default learning rate, while others debated the optimal learning rate range and the importance of tuning based on dataset size.

**Tags**: `#QLoRA`, `#fine-tuning`, `#learning rate`, `#overfitting`, `#LLM`

---

<a id="item-10"></a>
## [ExTernD: Ternary LLM Quantization Nears Full Precision](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 8.0/10

ExTernD proposes a novel post-training quantization method that decomposes each weight matrix into two ternary matrices and a diagonal scaling matrix, allowing the inner rank to be expanded arbitrarily to reduce quantization error. This approach overcomes the fixed-matrix-size limitation of prior ternary quantization, achieving accuracy that approaches any desired level with only a modest increase in VRAM, potentially enabling efficient deployment of large language models on resource-constrained hardware. The method uses two ternary matrices (values in {-1,0,1}) and a diagonal scaling matrix; the expanded inner rank allows the effective bit-width to be tuned for accuracy versus memory trade-offs. The author claims it takes only slightly more VRAM than current quantization methods.

reddit · r/MachineLearning · /u/LMTLS5 · Jul 16, 13:31

**Background**: Post-training quantization (PTQ) reduces the precision of a pre-trained LLM's weights to lower bit-widths (e.g., 4-bit, ternary) to reduce memory and computation. Ternary quantization restricts weights to three values (-1,0,1), but prior methods suffered from fixed matrix size limiting accuracy. ExTernD addresses this by factorizing the weight matrix into a product of two ternary matrices with an adjustable inner dimension.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2607.13511v1">ExTernD: Expanded-Rank Ternary Decomposition Ternary LLM PTQ ...</a></li>
<li><a href="https://aipapers.ai/paper/26889608">ExTernD: Expanded-Rank Ternary Decomposition Ternary LLM PTQ ...</a></li>
<li><a href="https://www.machinebrief.com/news/externd-the-new-frontier-in-ternary-factorization-for-llms-qkt0">ExTernD: The New Frontier in Ternary Factorization for LLMs</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#ternary`, `#PTQ`, `#decomposition`

---

<a id="item-11"></a>
## [PnP-CoSMo: Content/Style Modeling for MRI Reconstruction](https://www.reddit.com/r/MachineLearning/comments/1uy2h66/pnpcosmo_a_multicontrast_mri_reconstruction/) ⭐️ 8.0/10

PnP-CoSMo is a plug-and-play framework for multi-contrast MRI reconstruction that learns contrast-invariant content and style from image-domain data alone, eliminating the need for raw k-space training data. It achieves competitive performance with state-of-the-art unrolled networks while offering better generalizability. This work addresses a critical data bottleneck in deep learning-based MRI reconstruction by removing the requirement for raw k-space training data, which is often difficult to obtain. It also generalizes across different MR contrasts and forward operators, potentially accelerating clinical adoption of AI-driven reconstruction. The framework first learns a content/style model from image-domain data, then freezes it as a prior in iterative reconstruction. It was published in Medical Image Analysis and demonstrated on the NYU fastMRI dataset and in-house multi-coil raw datasets, achieving up to 32.6% more acceleration over non-guided reconstruction.

reddit · r/MachineLearning · /u/void_gear · Jul 16, 13:10

**Background**: Multi-contrast MRI acquires images with different tissue contrasts (e.g., T1-weighted, T2-weighted) to aid diagnosis. Traditional deep learning reconstruction methods often require raw k-space data for training, which is not always available. PnP-CoSMo uses a content/style disentanglement approach, where content represents structural anatomy and style captures contrast-specific variations, enabling guided reconstruction from a reference scan.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2409.13477v4">A Plug-and-Play Method for Guided Multi-contrast MRI Reconstruction based on Content/Style Modeling</a></li>
<li><a href="https://arxiv.org/abs/2409.13477">[2409.13477] A Plug-and-Play Method for Guided Multi-contrast MRI Reconstruction based on Content/Style Modeling</a></li>
<li><a href="https://www.researchgate.net/publication/384245741_A_Plug-and-Play_Method_for_Guided_Multi-contrast_MRI_Reconstruction_based_on_ContentStyle_Modeling">(PDF) A Plug-and-Play Method for Guided Multi-contrast MRI Reconstruction based on Content/Style Modeling</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion includes technical questions about the content/style disentanglement and comparisons with other methods. The author engages with comments, clarifying that the model is trained purely on image-domain data and that the code is available. Overall sentiment is positive, with interest in the practical implications.

**Tags**: `#MRI reconstruction`, `#deep learning`, `#medical imaging`, `#plug-and-play`, `#content/style modeling`

---

<a id="item-12"></a>
## [Schema Harness Claims 99% on ARC-AGI-3](https://www.reddit.com/r/MachineLearning/comments/1uyf8oo/new_fable5opus48_harness_called_schema_claims_99/) ⭐️ 8.0/10

A new AI reasoning harness called Schema, developed by Impossible Research, claims to achieve 99% on the ARC-AGI-3 Public set using Claude Opus 4.8 and Fable 5, and 95.35% using GPT-5.6 Sol, without modifying model weights. This result suggests that significant improvements on challenging reasoning benchmarks can be achieved by enhancing the process around fixed models, potentially shifting focus from scaling models to improving reasoning harnesses. The harness uses a fallback rule: Opus 4.8 and Sol xhigh run first; games scoring below 80 are rerun with Fable 5 and Sol max, retaining the higher per-game score. Both results are self-reported and have not been verified by ARC Prize.

reddit · r/MachineLearning · /u/we_are_mammals · Jul 16, 21:02

**Background**: ARC-AGI-3 is an interactive reasoning benchmark that tests AI agents on novel, abstract, turn-based environments requiring exploration, goal inference, and planning. A harness (or scaffold) is the external system that manages model inputs, outputs, and execution flow, distinct from the model itself.

<details><summary>References</summary>
<ul>
<li><a href="https://schema-harness.github.io/">Frontier Models with Our Harness Achieve ~99% on ARC-AGI-3 Public — Schema</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://huggingface.co/blog/agent-glossary">Harness, Scaffold, and the AI Agent Terms Worth Getting Right</a></li>

</ul>
</details>

**Discussion**: The Reddit post aims to bring back technical discussions, and the ARC Prize president tweeted that it 'looks cool' and needs further investigation. The community is cautiously optimistic but awaits verification.

**Tags**: `#ARC-AGI`, `#AI reasoning`, `#harness`, `#benchmark`, `#LLM`

---

<a id="item-13"></a>
## [Disentangling a Convolutional Neuron via Hadamard Product](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 8.0/10

A new method uses the Hadamard product of a neuron's receptive field and its weights, followed by clustering, to disentangle patterns detected by a single convolutional neuron in Inceptionv1, revealing monosemantic clusters and unexpected low-valued patterns like letters. This work provides a novel technique for mechanistic interpretability of convolutional neural networks, potentially enabling deeper understanding of how individual neurons encode multiple concepts, which is crucial for model transparency and safety. The method was applied to a 1x1 convolution neuron in Inceptionv1's mixed4e layer; low-valued clusters like letters showed dependent neurons also firing on the same concept, with positive and negative weights evenly distributed to reduce the sum.

reddit · r/MachineLearning · /u/narang_27 · Jul 15, 06:59

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks by breaking them into understandable components. The Hadamard product is an element-wise multiplication operation used in various neural architectures. Inceptionv1 is a convolutional neural network architecture known for its inception modules. Monosemantic features refer to neurons that respond to a single, human-interpretable concept.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hadamard_product_(matrices)">Hadamard product (matrices) - Wikipedia</a></li>
<li><a href="https://transformer-circuits.pub/2023/monosemantic-features/index.html">Towards Monosemanticity: Decomposing Language Models With ...</a></li>
<li><a href="https://arxiv.org/html/2504.13112v1">Hadamard product in deep learning: Introduction, Advances and Challenges</a></li>

</ul>
</details>

**Discussion**: The author notes that starting with convolutions may have limited interest, as the community focuses more on language models. They seek feedback on the usefulness of the findings and plan to shift to language model interpretability.

**Tags**: `#mechanistic interpretability`, `#convolutional neural networks`, `#neuron analysis`, `#interpretability`, `#deep learning`

---

<a id="item-14"></a>
## [PyTorch model 170x slower on T4 vs A100: memory bandwidth bottleneck](https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/) ⭐️ 8.0/10

A PyTorch point-tracking model runs 170x slower on an NVIDIA T4 GPU compared to an A100, taking 85 seconds per half-video on T4 versus 0.5 seconds on A100, despite both GPUs being fully utilized. This extreme performance gap highlights how memory bandwidth and Tensor Core support critically impact real-world deep learning workloads, especially for models with dense correlation volumes and transformers. The model uses pure FP32 precision and builds 4D correlation volumes followed by transformer layers; the T4 has 320 Tensor Cores but they only accelerate FP16/INT8, not FP32, while the A100's Tensor Cores support FP32 via TF32.

reddit · r/MachineLearning · /u/Future-Structure-296 · Jul 15, 13:44

**Background**: The NVIDIA T4 (Turing) and A100 (Ampere) are data center GPUs with different architectures. The T4's Tensor Cores do not accelerate FP32 matrix operations, so FP32 code runs on CUDA cores only, while the A100's Tensor Cores can handle FP32 via TF32. Additionally, the T4 has a memory bandwidth of 320 GB/s versus the A100's 1555 GB/s, making memory-bound operations like 4D correlation volumes much slower on T4.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/tesla-t4/">NVIDIA T4 Tensor Core GPU for AI Inference | NVIDIA Data Center</a></li>
<li><a href="https://www.nvidia.com/content/dam/en-zz/Solutions/Data-Center/tesla-t4/t4-tensor-core-datasheet.pdf">NVIDIA T4 TENSOR CORE GPU</a></li>
<li><a href="https://www.fluence.network/blog/nvidia-t4/">NVIDIA T4: Pricing, Specs, Best Uses & Where to Run (2026)</a></li>

</ul>
</details>

**Discussion**: Comments suggest the slowdown is likely due to memory bandwidth limits and the lack of Tensor Core acceleration for FP32 on T4. Users recommend switching to mixed precision (FP16) or using TF32 on A100 to leverage Tensor Cores, and profiling memory access patterns.

**Tags**: `#PyTorch`, `#GPU performance`, `#NVIDIA T4`, `#NVIDIA A100`, `#deep learning`

---

<a id="item-15"></a>
## [Microsoft Comic Chat Open-Sourced After 30 Years](https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/) ⭐️ 7.0/10

On July 16, 2026, Microsoft open-sourced Comic Chat, the graphical IRC client that visualized chat as comic panels, on GitHub. This release preserves a piece of internet history and allows developers to study and remix a unique chat client that introduced Comic Sans to the world. Comic Chat was originally developed by Microsoft researcher David Kurlander and first released with Internet Explorer 3.0 in 1996. The open-source release includes the source code and is available on GitHub under an MIT license.

hackernews · jervant · Jul 16, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48936426)

**Background**: IRC (Internet Relay Chat) is a text-based chat protocol that was popular in the 1990s and early 2000s. Comic Chat was a graphical IRC client that automatically turned conversations into comic strips with characters, speech bubbles, and expressions, making it a memorable experiment in user interface design.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Comic_Chat">Microsoft Comic Chat</a></li>
<li><a href="https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/">Microsoft Comic Chat is now open source</a></li>
<li><a href="https://en.wikipedia.org/wiki/IRC_client">IRC client</a></li>

</ul>
</details>

**Discussion**: Community members expressed nostalgia and excitement, with one user sharing that Comic Chat inspired their first startup. Another noted that while it was a historical artifact, it was somewhat reviled in the IRC community for extending the protocol with proprietary features.

**Tags**: `#open source`, `#microsoft`, `#IRC`, `#nostalgia`, `#history`

---

<a id="item-16"></a>
## [Decoy Font: Hiding Text from AI](https://www.mixfont.com/experiments/decoy-font) ⭐️ 7.0/10

Decoy Font is a free TTF font that embeds a hidden message in each character using spatial frequency techniques, making the visible text readable to humans but difficult for AI and OCR systems to extract. This adversarial typography technique demonstrates a creative way to protect text from automated scraping and analysis, which could be useful for watermarking, captchas, or poisoning training data. Each letter combines a thin-outlined decoy foreground character with a blurred low-frequency background shape that contains the real letter, exploiting differences in how humans and AI perceive spatial frequencies.

hackernews · ray__ · Jul 16, 16:18 · [Discussion](https://news.ycombinator.com/item?id=48936584)

**Background**: Adversarial typography is a technique that uses text to confuse machine learning models, often by printing misleading words over images. Decoy Font extends this idea to the font level, inspired by hybrid images that display different content at different resolutions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mixfont.com/experiments/decoy-font">Decoy Font: A TTF font that hides what you type - mixfont.com</a></li>
<li><a href="https://daily.dev/posts/decoy-font-a-ttf-font-that-hides-what-you-type-4ez2kvvb1">Decoy Font: A TTF font that hides what you type - daily.dev</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some find it cool but question its practical utility, while others report that models like GPT-4o can still read the hidden text with proper prompting. Experiments show varying success across different AI models.

**Tags**: `#AI`, `#adversarial`, `#typography`, `#security`, `#machine learning`

---

<a id="item-17"></a>
## [Classical ML for LLM Text Detection](https://blog.lyc8503.net/en/post/llm-classifier/) ⭐️ 7.0/10

A blog post explores using classical machine learning methods, such as TF-IDF and logistic regression, to detect LLM-generated text, achieving promising results on a Chinese dataset. This approach offers a lightweight, interpretable alternative to deep learning detectors, potentially enabling real-time detection in browsers or edge devices. It also sparks debate on the feasibility and ethics of AI text detection. The classifier uses TF-IDF features and a logistic regression model, trained on a dataset of human-written and LLM-generated Chinese texts. The model is small enough to run client-side, but its effectiveness may degrade as LLMs evolve.

hackernews · uneven9434 · Jul 16, 16:41 · [Discussion](https://news.ycombinator.com/item?id=48936880)

**Background**: LLM-generated text detection is a binary classification task to determine if a text was produced by an AI. Classical ML methods like TF-IDF and logistic regression are simpler and more transparent than deep neural networks, but may struggle with subtle patterns. Recent surveys highlight watermarking, statistical, and neural approaches as main detection paradigms.

<details><summary>References</summary>
<ul>
<li><a href="https://direct.mit.edu/coli/article/51/1/275/127462/A-Survey-on-LLM-Generated-Text-Detection-Necessity">A Survey on LLM-Generated Text Detection: Necessity, Methods ...</a></li>
<li><a href="https://arxiv.org/abs/2310.14724">[2310.14724] A Survey on LLM-Generated Text Detection ... A Survey on LLM-Generated Text Detection: Necessity, Methods ... AI-generated text detection: A comprehensive review of ... The State of the Art in Detecting LLM-Generated Text in ... The Science of Detecting LLM-Generated Text NLP2CT/LLM-generated-Text-Detection - GitHub</a></li>
<li><a href="https://ieeexplore.ieee.org/document/8945745">An Exploration on Text Classification with Classical Machine ...</a></li>

</ul>
</details>

**Discussion**: Commenters debate the long-term viability of detection, with some arguing that text lacks information density for reliable provenance detection, while others see value in effort-based metrics. One commenter suggests using such classifiers as browser extensions, akin to ad blockers.

**Tags**: `#LLM detection`, `#machine learning`, `#AI-generated text`, `#NLP`, `#classical ML`

---

<a id="item-18"></a>
## [OnePlus Halts New Product Launches in US and Europe](https://community.oneplus.com/thread/2170715118587871237) ⭐️ 7.0/10

OnePlus has decided to stop launching new products in the US and Europe, though it will continue to support existing devices with software updates and security patches. This marks a significant retreat from key Western markets for a brand once celebrated as the 'hacker's choice,' signaling a shift in strategy under parent company OPPO and potentially reducing consumer choice in the premium mid-range segment. The decision only affects new product rollouts, not full operations; existing devices will continue to receive scheduled updates. OnePlus has not halted operations entirely, as some headlines have suggested.

hackernews · pilililo2 · Jul 16, 10:14 · [Discussion](https://news.ycombinator.com/item?id=48932539)

**Background**: OnePlus was founded in 2013 with a 'Never Settle' ethos, offering high-spec, near-stock Android phones at competitive prices with unlocked bootloaders. Over time, it moved away from its enthusiast roots, merging with OPPO and adopting ColorOS, which alienated many early fans.

**Discussion**: Community comments express sadness over OnePlus's decline from its hacker-friendly origins, with users noting the loss of factory images and stock Android. Some correct the misconception that OnePlus is halting all operations, emphasizing that only new product launches are stopping.

**Tags**: `#OnePlus`, `#smartphone`, `#tech industry`, `#consumer hardware`, `#business strategy`

---

<a id="item-19"></a>
## [Interactive Linear Algebra Book Wins Praise](https://immersivemath.com/ila/) ⭐️ 7.0/10

An immersive linear algebra book with interactive figures, available at immersivemath.com, has been highlighted for its educational value and community approval (169 points, 26 comments). This resource demonstrates how interactive visualization can significantly enhance understanding of abstract mathematical concepts, potentially influencing future educational materials. The book features clean presentation, tooltips, and interactive figures that allow users to explore concepts step by step. It is praised for its clarity and potential for expansion to other subjects like statistics and robotics.

hackernews · srean · Jul 16, 15:32 · [Discussion](https://news.ycombinator.com/item?id=48935951)

**Background**: Linear algebra is a foundational branch of mathematics used in computer science, physics, and engineering. Traditional textbooks often rely on static diagrams, which can make abstract concepts like vector spaces and transformations difficult to grasp. Interactive figures allow learners to manipulate parameters and see real-time changes, improving intuition.

**Discussion**: Commenters expressed strong enthusiasm, wishing such resources existed when they were students. Some suggested adding AI-powered explanations or expanding to other fields like statistics and robotics. Overall sentiment is highly positive, with appreciation for the clean design and educational value.

**Tags**: `#linear algebra`, `#interactive learning`, `#education`, `#visualization`

---

<a id="item-20"></a>
## [GPT-5.6 Codex Bug Can Delete $HOME Directory](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 7.0/10

OpenAI has confirmed a bug in GPT-5.6 Codex where the AI coding agent can accidentally delete the user's $HOME directory when attempting to set a temporary directory, especially when running without sandboxing protections. This bug highlights critical safety risks for AI coding agents that have direct file system access, potentially causing irreversible data loss for developers who rely on these tools without proper safeguards. The bug occurs when full access mode is enabled, sandboxing is disabled, and auto review is turned off; the model attempts to override the $HOME environment variable to define a temporary directory but mistakenly deletes $HOME instead.

rss · Simon Willison · Jul 16, 17:45

**Background**: Codex is an AI coding agent developed by OpenAI, released in April 2025 as Codex CLI, designed to automate software engineering tasks like writing code and fixing bugs. Sandboxing is a security mechanism that isolates an AI agent's operations to prevent it from affecting the host system. The $HOME environment variable points to the user's home directory, which contains personal files and configurations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Codex_(AI_agent)">Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://northflank.com/blog/how-to-sandbox-ai-agents">How to sandbox AI agents in 2026: MicroVMs, gVisor ...</a></li>
<li><a href="https://stackoverflow.com/questions/6877727/how-do-i-delete-an-exported-environment-variable">linux - How do I delete an exported environment variable ?</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#bug`

---

<a id="item-21"></a>
## [DABSN: New Recurrent Architecture Seeks Collaborators](https://www.reddit.com/r/MachineLearning/comments/1uycffg/seeking_collaborators_for_scaling_and_independent/) ⭐️ 7.0/10

The author released a preprint and open-source code for DABSN (Dynamic Adaptive Bias State Network), a new recurrent architecture that shows promising results on reasoning, memory, and long-sequence benchmarks, and trained a 24M-parameter language model on 1B tokens with interesting outcomes. If validated, DABSN could offer an efficient alternative to transformers for language modeling, especially for long-context tasks, and the open collaboration model may accelerate independent verification and scaling. The architecture was evaluated on MQAR, Copy, Key-Value retrieval, and A5/60 benchmarks, with PyTorch, C++, and Triton implementations provided. The author seeks collaborators for independent reproduction, stronger baselines, and access to larger GPU clusters.

reddit · r/MachineLearning · /u/BleedingXiko · Jul 16, 19:17

**Background**: Recurrent architectures like LSTMs and GRUs were once dominant for sequence modeling but were largely replaced by transformers due to parallelization and scaling advantages. Recently, state-space models (e.g., Mamba) have revived interest in recurrent approaches for efficient long-context processing. DABSN is a new recurrent design aiming to combine the strengths of both worlds.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2312.04927">[2312.04927] Zoology: Measuring and Improving Recall in ... GitHub - HazyResearch/zoology: Understand and test language ... GitHub - howard-hou/Visual-MQAR: Understand and test multi ... MQAR: Multi-Query Associative Recall - emergentmind.com Zoology (Blogpost 1): Measuring and Improving Recall in ... Published as a workshop paper at SCOPE - ICLR 2025 - OpenReview Understanding Input Selectivity in Mamba: Impact on ...</a></li>
<li><a href="https://github.com/HazyResearch/zoology">GitHub - HazyResearch/zoology: Understand and test language ... GitHub - howard-hou/Visual-MQAR: Understand and test multi ... MQAR: Multi-Query Associative Recall - emergentmind.com Zoology (Blogpost 1): Measuring and Improving Recall in ... Published as a workshop paper at SCOPE - ICLR 2025 - OpenReview Understanding Input Selectivity in Mamba: Impact on ...</a></li>

</ul>
</details>

**Tags**: `#recurrent architecture`, `#language model`, `#open source`, `#machine learning research`, `#scaling`

---

<a id="item-22"></a>
## [Rethinking AI Memory: From Facts to Reasoning Patterns](https://www.reddit.com/r/MachineLearning/comments/1uy6yht/are_current_ai_memory_architectures_optimizing/) ⭐️ 7.0/10

A Reddit post proposes that AI memory systems should evolve from storing descriptive facts to inferring higher-level reasoning patterns, such as explanatory frameworks and reasoning styles, rather than just user preferences and conversation summaries. This shift could fundamentally change how AI systems personalize interactions and maintain context, moving from static note-taking to dynamic user modeling, which may lead to more intuitive and adaptive AI assistants. The author contrasts current descriptive memory (e.g., 'user is interested in economics') with a proposed inferential memory that captures reasoning patterns (e.g., 'user explains economic outcomes through incentives and institutional constraints'). The post questions whether such representations can emerge naturally or require fundamentally new architectures.

reddit · r/MachineLearning · /u/Boris_Ljevar · Jul 16, 16:00

**Background**: Current AI memory systems, such as those used in chatbots and agents, primarily store explicit facts and conversation summaries to maintain context. These systems rely on retrieval-augmented generation (RAG) and persistent context buffers. The post draws inspiration from cognitive architectures like ACT-R and SOAR, which model human reasoning structures, suggesting a move toward more abstract, inferential memory representations.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/IAAR-Shanghai/Awesome-AI-Memory">IAAR-Shanghai/Awesome-AI-Memory - GitHub</a></li>
<li><a href="https://zylos.ai/research/2026-04-05-ai-agent-memory-architectures-persistent-knowledge/">AI Agent Memory Architectures: From Context Windows to ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cognitive_architecture">Cognitive architecture</a></li>

</ul>
</details>

**Tags**: `#AI memory`, `#persistent context`, `#machine learning`, `#cognitive architectures`

---

<a id="item-23"></a>
## [Seeking Devil's Advocate Critique of JEPA Models](https://www.reddit.com/r/MachineLearning/comments/1uxcryc/looking_for_jepa_devil_advocates_r/) ⭐️ 7.0/10

A researcher on Reddit is asking the community to provide devil's advocate arguments against Yann LeCun's Joint Embedding Predictive Architecture (JEPA) for robot learning, seeking balanced critique beyond LeCun's optimistic presentations. JEPA is a prominent approach in world models and robot learning, and critical discussion helps the community identify potential weaknesses and avoid overhyping. This post invites substantive debate that can guide future research directions. The poster has read recent JEPA papers and finds the approach promising but is concerned about LeCun's dismissal of LLMs and RL. They want to know the biggest downsides of JEPA compared to other world model approaches.

reddit · r/MachineLearning · /u/Amazing-Coat5160 · Jul 15, 17:34

**Background**: JEPA (Joint Embedding Predictive Architecture) is a self-supervised learning framework proposed by Yann LeCun that learns abstract representations by predicting future states in an embedding space, rather than reconstructing pixels. It is central to LeCun's vision for autonomous machine intelligence and world models for robot learning. The approach contrasts with generative models and reinforcement learning, which LeCun has criticized as insufficient for achieving human-level intelligence.

<details><summary>References</summary>
<ul>
<li><a href="https://rohitbandaru.github.io/blog/JEPA-Deep-Dive/">Deep Dive into Yann LeCun’s JEPA | Rohit Bandaru</a></li>
<li><a href="https://ai.meta.com/blog/yann-lecun-ai-model-i-jepa/">I-JEPA: The first AI model based on Yann LeCun’s vision for ...</a></li>
<li><a href="https://blog.yucas.net/2026/05/18/beyond-llms-yann-lecuns-critique-and-the-jepa-research-program-2/">Beyond LLMs: Yann LeCun’s Critique and the JEPA Research ...</a></li>

</ul>
</details>

**Discussion**: The Reddit post has generated discussion where some users point out that JEPA's reliance on abstract representations may lose fine-grained details needed for precise control. Others question the scalability of training JEPA models on diverse robotic tasks compared to more established RL methods.

**Tags**: `#JEPA`, `#world models`, `#robot learning`, `#Yann LeCun`, `#AI research`

---

<a id="item-24"></a>
## [uv 0.11.29 Adds JSON Output and CUDA 13.2 Support](https://github.com/astral-sh/uv/releases/tag/0.11.29) ⭐️ 6.0/10

uv 0.11.29 introduces JSON output for the `uv tree` command and adds CUDA 13.2 as a supported PyTorch backend. The release also includes performance improvements and bug fixes for dependency resolution and PyPy downloads. JSON output from `uv tree` enables easier programmatic consumption of dependency trees, benefiting CI/CD pipelines and tooling. CUDA 13.2 support ensures uv users can leverage the latest NVIDIA GPU compute capabilities for PyTorch workloads. The JSON output for `uv tree` is available via the `--json` flag. CUDA 13.2 support aligns with PyTorch 2.12's experimental CUDA 13.2 builds. The release also improves performance by reusing workspace discovery and deferring client setup for no-op syncs.

github · github-actions[bot] · Jul 15, 18:44

**Background**: uv is a fast Python package and project manager written in Rust, developed by Astral. It aims to replace pip, pip-tools, and virtualenv with a single tool. The `uv tree` command displays the project's dependency tree, and JSON output makes it machine-readable. CUDA is NVIDIA's parallel computing platform, and CUDA 13.2 is the latest version with enhanced tile support and Python features.

<details><summary>References</summary>
<ul>
<li><a href="https://dev-discuss.pytorch.org/t/introducing-cuda-13-2-and-deprecating-cuda-12-8-release-2-12/3337">Introducing CUDA 13.2 and Deprecating CUDA 12.8 (Release 2.12)</a></li>
<li><a href="https://developer.nvidia.com/blog/cuda-13-2-introduces-enhanced-cuda-tile-support-and-new-python-features/">CUDA 13.2 Introduces Enhanced CUDA Tile Support and New ...</a></li>

</ul>
</details>

**Tags**: `#uv`, `#python`, `#package-manager`, `#release`

---

<a id="item-25"></a>
## [Mermaid to ASCII Art with Color via WebAssembly](https://simonwillison.net/2026/Jul/16/mermaid-ascii/#atom-everything) ⭐️ 6.0/10

Simon Willison compiled the Go library AlexanderGrooff/mermaid-ascii to WebAssembly, creating a browser-based tool that converts Mermaid diagrams to ASCII art with color support. This tool makes Mermaid diagrams accessible in terminal-like environments and plain-text contexts, with color support improving readability over previous ASCII-only renderers. The tool is available at tools.simonwillison.net/mermaid-ascii and includes options for padding, box padding, and an 'ASCII only' mode. It builds on an earlier Rust-based version that lacked color support.

rss · Simon Willison · Jul 16, 14:57

**Background**: Mermaid is a popular diagramming tool that uses text-based syntax to generate flowcharts, sequence diagrams, and more. ASCII art rendering allows these diagrams to be displayed in terminals or code comments without image support. WebAssembly enables running compiled code from languages like Go and Rust directly in the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/AlexanderGrooff/mermaid-ascii">GitHub - AlexanderGrooff/mermaid-ascii: Render Mermaid graphs ...</a></li>
<li><a href="https://go.dev/wiki/WebAssembly">Go Wiki: WebAssembly - The Go Programming Language</a></li>

</ul>
</details>

**Tags**: `#mermaid`, `#ascii-art`, `#webassembly`, `#developer-tools`

---

<a id="item-26"></a>
## [RTCA Workshop at NeurIPS 2026: Call for Papers](https://www.reddit.com/r/MachineLearning/comments/1uy8e0v/cfp_rtca_neurips_2026_r/) ⭐️ 6.0/10

The inaugural Real-Time Conversational Agents (RTCA) Workshop at NeurIPS 2026 has issued a call for papers and demos, focusing on real-time multimodal interaction including streaming speech, video, and language generation. This workshop addresses the growing need for natural, low-latency conversational AI systems that operate in real-time, a critical step beyond offline generation for applications like voice assistants and embodied avatars. Submissions are due by 29 August 2026, with author notification on 29 September 2026; the workshop is non-archival, allowing authors to publish elsewhere.

reddit · r/MachineLearning · /u/Few-Ferret9700 · Jul 16, 16:51

**Background**: Conversational AI has evolved from text-based chat to real-time multimodal interactions involving speech, video, and shared screens. Achieving naturalness requires handling latency, turn-taking, interruptions, and cross-modal alignment—challenges that offline systems avoid. The RTCA workshop aims to build shared benchmarks and methodologies for this emerging field.

<details><summary>References</summary>
<ul>
<li><a href="https://openreview.net/group?id=NeurIPS.cc/2026/Workshop/RTCA&referrer=[Homepage](/)">NeurIPS 2026 Workshop RTCA | OpenReview</a></li>

</ul>
</details>

**Tags**: `#NeurIPS`, `#workshop`, `#conversational AI`, `#multimodal`, `#real-time`

---

<a id="item-27"></a>
## [Best Python Tools for Multi-Objective Surrogate-Based Optimization](https://www.reddit.com/r/MachineLearning/comments/1uxty9v/best_current_tools_for_multiobjective/) ⭐️ 6.0/10

A Reddit user is seeking recommendations for Python tools to perform multi-objective surrogate-based optimization (MOSBO) on heterogeneous study data with physiological constraints, considering PyMC, pymoo, pysamoo, SMT, and Matlab Global Optimization Toolbox. This query highlights the growing need for accessible, Colab-friendly optimization workflows that combine hierarchical Bayesian modeling with surrogate-assisted multi-objective optimization, which is crucial for meta-analyses in fields like physiology and medicine. The user has data from ~40 studies in Excel, aims to optimize three objectives (total improvement, improvement per unit time, improvement per unit effort), and requires continuous outputs respecting physiological constraints. They prefer Colab-friendly Python solutions.

reddit · r/MachineLearning · /u/BleakReason · Jul 16, 05:43

**Background**: Multi-objective surrogate-based optimization uses surrogate models (e.g., Gaussian processes) to approximate expensive objective functions, enabling efficient optimization of multiple conflicting objectives. Tools like pymoo and pysamoo provide algorithms for surrogate-assisted optimization, while SMT offers a library of surrogate models. PyMC is a probabilistic programming library for Bayesian hierarchical modeling.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/anyoptimization/pysamoo">GitHub - anyoptimization/pysamoo pysamoo · PyPI [2204.05855] pysamoo: Surrogate-Assisted Multi-Objective ... GitHub - anyoptimization/pysamoo MANY - arXiv.org pymoo: Multi-objective Optimization in Python</a></li>
<li><a href="https://smt.readthedocs.io/en/latest/index.html">SMT: Surrogate Modeling Toolbox — SMT 2.14.2.dev1+g0d3602a74 ...</a></li>
<li><a href="https://awesome.ecosyste.ms/projects/github.com/parmoo/parmoo">Python library for parallel multiobjective simulation optimization</a></li>

</ul>
</details>

**Tags**: `#multi-objective optimization`, `#surrogate modeling`, `#Bayesian inference`, `#meta-analysis`, `#Python tools`

---