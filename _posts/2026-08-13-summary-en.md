---
layout: default
title: "Horizon Summary: 2026-08-13 (EN)"
date: 2026-08-13
lang: en
---

> From 33 items, 22 important content pieces were selected

---

1. [Qwen Releases 2.4T-Parameter MoE Model Qwen3.8-2.4T-A95B](#item-1) ⭐️ 9.0/10
2. [Researchers Steal Hidden Reasoning from LLM APIs](#item-2) ⭐️ 9.0/10
3. [DeepSeek V4 Pro 0813 Released with Strong Performance](#item-3) ⭐️ 8.0/10
4. [Zed Introduces Delta: Collaborative AI Agent with Multiplayer Conversations](#item-4) ⭐️ 8.0/10
5. [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](#item-5) ⭐️ 8.0/10
6. [Discovered Materials launches AI agents for semiconductor heat management](#item-6) ⭐️ 8.0/10
7. [xAI Releases Grok 4.6, a New Frontier Model](#item-7) ⭐️ 8.0/10
8. [uBlock Origin Stops Blocking Facebook Ads](#item-8) ⭐️ 8.0/10
9. [Why Tiny JPEGs Look Different in Chrome](#item-9) ⭐️ 8.0/10
10. [Adam's Rotation Dependence Breaks Implicit Low-Rank Bias, Muon Retains It](#item-10) ⭐️ 8.0/10
11. [Decoupled Descent: Enforcing Exact Train-Test Error Tracking via AMP Onsager Corrections](#item-11) ⭐️ 8.0/10
12. [HTML over WebSockets: Real-Time SPAs with Minimal JavaScript](#item-12) ⭐️ 7.0/10
13. [AI Coding Tools Risk Creating Unmaintainable Codebases](#item-13) ⭐️ 7.0/10
14. [No Lossless Transformations of Natural-Language Text](#item-14) ⭐️ 7.0/10
15. [New site ranks CS conferences by destination quality, not prestige](#item-15) ⭐️ 7.0/10
16. [Seeking RL/Planning Advice for Stochastic Merge Puzzle with Afterstates](#item-16) ⭐️ 7.0/10
17. [Developer Shares 2026 Eclipse Webcam Aggregation Site](#item-17) ⭐️ 6.0/10
18. [AmigaDOS Developer Tim King Passes Away](#item-18) ⭐️ 6.0/10
19. [Mass Scans Spoof AI Bots, But Experts Say It's Old News](#item-19) ⭐️ 6.0/10
20. [Datasette Upload DBS 0.5a0 Adds Formalized API for Atomic Database Swaps](#item-20) ⭐️ 6.0/10
21. [AAAI 2027 Reviewers Note Lack of Code Submissions](#item-21) ⭐️ 6.0/10
22. [Agentic World Cup: LLM Agents Compete in 1v1 Soccer](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Qwen Releases 2.4T-Parameter MoE Model Qwen3.8-2.4T-A95B](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen has released Qwen3.8-2.4T-A95B, a massive Mixture-of-Experts (MoE) model with 2.4 trillion total parameters and 95 billion active parameters. The model achieves near-frontier performance, rivaling top models like Opus and Fable, and is available in BF16 and FP8 formats. This release pushes the boundaries of open-weight model scale, demonstrating that massive MoE models can be made available to the community. It also intensifies competition among AI labs, as it directly rivals models like Kimi k3 and DeepSeek V4, potentially accelerating innovation in serving and quantization techniques. The model is text-only and requires thinking mode for all interactions; multimodal inputs are not supported, and thinking cannot be disabled. The BF16 version is approximately 4.9TB, while a 1-bit quantized version is around 397GB, making it feasible to run on consumer hardware. The model card claims performance between Opus 4.8 and Fable 5.

hackernews · Philpax · Aug 12, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49273478)

**Background**: Mixture-of-Experts (MoE) models activate only a subset of parameters per token, allowing for massive total parameter counts while keeping inference costs manageable. Quantization techniques like FP8 and 1-bit reduce memory footprint and improve throughput with minimal accuracy loss. Qwen3.8-Max is the official version based on this model, adding features like vision input and 1M context length, which are not present in the open-weight release.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B">Qwen/Qwen3.8-2.4T-A95B - Hugging Face</a></li>
<li><a href="https://developer.nvidia.com/blog/serve-qwen3-8-2-4t-a95b-a-2-4t-parameter-model-with-configurable-reasoning-on-nvidia-gb300-nvl72/">Serve Qwen3.8-2.4T-A95B, a 2.4T-Parameter Model, with ...</a></li>
<li><a href="https://www.reddit.com/r/LocalLLaMA/comments/1vmgozv/qwen3824ta95b_released/">Qwen3.8-2.4T-A95B Released : r/LocalLLaMA - Reddit</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the model's size and serving challenges, noting that only BF16 and FP8 are released, making it harder to serve than Kimi k3 at launch. Some users are excited about the 1-bit quantized version's small size (397GB) and performance, while others point out the lack of vision support and 1M context in the open-weight version. Comparisons with DeepSeek V4-Pro and Grok 4.6 pricing also feature in the discussion.

**Tags**: `#AI`, `#LLM`, `#Qwen`, `#MoE`, `#HuggingFace`

---

<a id="item-2"></a>
## [Researchers Steal Hidden Reasoning from LLM APIs](https://simonwillison.net/2026/Aug/11/stealing-reasoning-traces/) ⭐️ 9.0/10

Researchers demonstrated a method to recover hidden chain-of-thought reasoning from proprietary LLM APIs by replaying encrypted reasoning blocks into weaker sibling models and jailbreaking them. The attack affected Anthropic, OpenAI, and Google, but has since been mitigated by the providers. This research exposes a significant security flaw in how leading AI providers protect their models' internal reasoning, potentially allowing attackers to extract sensitive or proprietary information. It underscores the need for stronger cryptographic safeguards and highlights the risks of relying on opaque, closed-source AI systems. The attack exploited the fact that models within the same family share the same encryption key for reasoning blocks, allowing cross-model replay. The easiest target was Claude Haiku 4.5, which was jailbroken with a simple prompt to transcribe the reasoning verbatim. The paper includes extensive extracted reasoning traces, revealing raw chain-of-thought content never intended for human consumption.

rss · Simon Willison · Aug 11, 22:40

**Background**: Chain-of-thought (CoT) reasoning is a technique where LLMs generate step-by-step reasoning before producing a final answer. Proprietary models like GPT-4 and Claude often keep this reasoning hidden from users, returning only encrypted blocks to prevent inspection. This research demonstrates a practical attack that bypasses this encryption, raising concerns about the privacy and security of AI reasoning processes.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Aug/11/stealing-reasoning-traces/">Stealing Reasoning Traces from Proprietary LLM APIs</a></li>
<li><a href="https://www.alphaxiv.org/abs/2608.09867">Stealing Reasoning Traces from Proprietary LLM APIs | alphaXiv</a></li>
<li><a href="https://cybersecuritynews.com/top-ai-models-apis-flaw-exposes-hidden-reasoning/">OpenAI, Anthropic, and Google LLM APIs vulnerability Exposes...</a></li>

</ul>
</details>

**Tags**: `#LLM security`, `#chain-of-thought`, `#proprietary APIs`, `#AI privacy`, `#jailbreak`

---

<a id="item-3"></a>
## [DeepSeek V4 Pro 0813 Released with Strong Performance](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek has released DeepSeek V4 Pro 0813, a new large-scale mixture-of-experts model available via API on OpenRouter. It features a 1,048,576-token context window, up to 384,000 output tokens, and pricing of $0.435 per million input tokens and $0.87 per million output tokens. This release is significant because DeepSeek models are known for cost-effectiveness, and early user reports highlight strong performance for development tasks at a low cost. It could intensify competition in the AI model market, especially against models like Opus 4.8 and Kimi-K3. The model supports thinking and non-thinking modes, tool calling, and the Responses API, making it suitable for coding, cybersecurity, automation, and long-horizon agent workflows. DeepSeek reports gains over the preview and scores above Opus 4.8 on benchmarks like Terminal Bench 2.1, Cybergym, and DeepSWE.

hackernews · explosion-s · Aug 12, 16:04 · [Discussion](https://news.ycombinator.com/item?id=49274600)

**Background**: DeepSeek is a Chinese AI company that has released a series of open-weight models, including DeepSeek-V4-Pro in April and July. The '0813' suffix indicates a version dated August 13, and this release is the general-availability version of DeepSeek V4 Pro. The model is available via API only, and it is unclear if open weights will be released.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-pro-0813">DeepSeek V4 Pro 0813 - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://aihubmix.com/model/deepseek-v4-pro-0813">deepseek-v4-pro-0813 - API Pricing & Performance | AIHubMix</a></li>
<li><a href="https://nano-gpt.com/models/text/deepseek/deepseek-v4-pro-0813">DeepSeek V4 Pro 0813 model | NanoGPT</a></li>

</ul>
</details>

**Discussion**: Community comments are generally positive, with users praising the model's cost-effectiveness and performance for development tasks. Some users noted the lack of an official announcement page and questioned the link to OpenRouter, while others shared specific usage experiences and benchmark comparisons.

**Tags**: `#AI`, `#DeepSeek`, `#LLM`, `#model release`, `#machine learning`

---

<a id="item-4"></a>
## [Zed Introduces Delta: Collaborative AI Agent with Multiplayer Conversations](https://zed.dev/blog/introducing-delta) ⭐️ 8.0/10

Zed announced Delta, a collaborative AI agent feature that enables real-time multiplayer conversations and inline commenting on agent threads. DeltaDB makes the worktree itself collaborative, keeping each participant's local copy in sync in real time. Delta could reshape team workflows by allowing multiple developers to collaborate on AI agent tasks in real time, potentially improving code review and mentoring processes. It represents a novel integration of multiplayer editing and AI assistance, which may influence future developer tools. DeltaDB is version control designed to store the process of coding alongside the agent, not just the code itself. The feature allows multiple participants to iterate on a prompt and comment inline in an agent conversation, treating the conversation as a document.

hackernews · khy · Aug 12, 18:19 · [Discussion](https://news.ycombinator.com/item?id=49276574)

**Background**: Zed is a high-performance, multiplayer code editor built from the ground up for collaboration with humans and AI. It was created by the makers of Atom and Tree-sitter, and its collaborative origin resurfaces in DeltaDB, which extends the multiplayer concept to AI agent interactions.

<details><summary>References</summary>
<ul>
<li><a href="https://zed.dev/blog/introducing-delta">Introducing Delta — Zed's Blog</a></li>
<li><a href="https://sesamedisk.com/what-is-zed-deltadb-features/">What Is Zed DeltaDB and Its Key Features - Sesame Disk</a></li>
<li><a href="https://zed.dev/ai">Zed — The AI Code Editor Built for Speed</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some question the utility of multiplayer coding, while others see value in mentoring and reviewing agent-generated work. There is also criticism of AI summaries being verbose or missing edge cases, and a complaint about the blog's low-contrast design.

**Tags**: `#AI`, `#code editor`, `#collaboration`, `#Zed`, `#developer tools`

---

<a id="item-5"></a>
## [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale published a detailed blog post revealing that a 16-year-old race condition in SQLite's WAL-reset logic caused database corruption in their control plane. They funded an open-source VFS shim that helped isolate the bug, which SQLite developers subsequently fixed. This incident highlights the subtlety of database reliability issues even in mature, widely-used software like SQLite, and demonstrates the value of investing in open-source debugging tools. The fix improves SQLite's robustness for all users, and Tailscale's approach serves as a model for companies contributing back to open-source projects. The bug occurs when a write transaction happens at a specific time during a checkpoint, causing the checkpoint to incorrectly assume pages have been copied from the WAL to the main database file. The VFS shim, named tmstmpvfs, added logging that allowed SQLite developers to identify and fix the race condition.

hackernews · ropbear · Aug 12, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49272832)

**Background**: SQLite is a widely-used embedded database that supports Write-Ahead Logging (WAL) mode for improved concurrency and performance. A VFS (Virtual File System) is an abstraction layer that allows SQLite to interact with different file systems; a VFS shim can intercept and log operations for debugging. The bug was disclosed by SQLite on March 5, 2026, and a fix was published shortly after.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL-Reset bug</a></li>
<li><a href="https://www.sqlite.org/howtocorrupt.html">How To Corrupt An SQLite Database File</a></li>
<li><a href="https://ubuntu.com/blog/hunting-a-16-year-old-sqlite-bug-with-tla-is-dqlite-affected">Hunting a 16-year-old SQLite bug with TLA+: is dqlite affected? | Ubuntu</a></li>

</ul>
</details>

**Discussion**: Community members praised Tailscale for their transparent write-up and for funding the open-source VFS shim, with some noting the value of supporting SQLite through support contracts. Others expressed curiosity about the specific checkpointing frequency that led to the bug, and one commenter highlighted the philosophical point that tests cannot prove the absence of bugs.

**Tags**: `#SQLite`, `#database`, `#bug`, `#Tailscale`, `#open-source`

---

<a id="item-6"></a>
## [Discovered Materials launches AI agents for semiconductor heat management](https://discoveredmaterials.com/research/) ⭐️ 8.0/10

Discovered Materials, a YC P26 startup, launched AI agents that discover new materials for semiconductor heat management, releasing hundreds of new materials and a benchmark for model evaluation. They claim their AI agents can discover materials in hours that would take a PhD student weeks, and they have synthesized thermal interface materials matching trade-secret performance. This addresses the escalating TDP of GPUs, which is a critical industry problem as heat dissipation drives datacenter power and water consumption. If successful, it could significantly reduce the timeline and cost of introducing new materials into semiconductor chips, impacting the entire semiconductor ecosystem. The company tested models from Anthropic, OpenAI, and Kimi, finding they can computationally discover dynamically stable materials. They acknowledge the 'lab-to-fab valley of death' and note that computational discovery is easier than synthesis; they are releasing a benchmark that measures model ability and documents strange behaviors like Claude's reward hacking and GPT-5.6 losing coherence after ~50M tokens.

hackernews · advaith08 · Aug 12, 07:51 · [Discussion](https://news.ycombinator.com/item?id=49269090)

**Background**: GPUs have a heat problem: Nvidia's H100 has a TDP of 700W, Blackwell 1.2kW, and Rubin 2.3kW. Heat dissipation is a major reason datacenters consume so much power and water. 3D packaging chips, such as placing HBM memory stacks on logic, could reduce energy per bit by 10-50x, but current dielectric materials like SiO2 are poor thermal conductors. The 'lab-to-fab valley of death' refers to the years and hundreds of millions of dollars needed to bring a new material into a fab.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Thermal_design_power">Thermal design power - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments are mixed: some find the approach promising but question novelty validation, noting models may have seen existing materials in training data. Others appreciate that they address feasibility, a step forward compared to previous AI-driven discovery efforts. There is also humor about model behaviors like GPT-5.6's mid-run relaxation summary.

**Tags**: `#AI`, `#materials science`, `#semiconductors`, `#startup`, `#YC`

---

<a id="item-7"></a>
## [xAI Releases Grok 4.6, a New Frontier Model](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI has released Grok 4.6, a new frontier model for coding, agentic tasks, and knowledge work, building on Grok 4.5 with improved instruction following and long-horizon agentic capabilities. The model is available via API with a 500k context window and pricing of $2 per million input tokens and $6 per million output tokens. Grok 4.6 returns xAI to the intelligence frontier, gaining 5 points over Grok 4.5 on the Intelligence Index and positioning it alongside OpenAI and behind only Anthropic. This intensifies competition in the AI model market, offering developers a cheaper and potentially more efficient alternative for coding and agentic tasks. Grok 4.6 is confirmed at 2T parameters with an early-August release window, and its performance numbers are distinct from Grok 4.5. The model is integrated into Cursor, and its API pricing is $2/$6 per million tokens, which is lower than the median for output tokens.

hackernews · iLuddite · Aug 12, 15:32 · [Discussion](https://news.ycombinator.com/item?id=49274027)

**Background**: Grok is xAI's series of large language models, designed to be maximally truthful and helpful. Frontier models are the most advanced AI models, often competing on benchmarks for coding, reasoning, and agentic tasks. The Intelligence Index is a metric used to compare such models, and xAI has been investing heavily in inference infrastructure to support its models.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.x.ai/developers/grok-4-6">Grok 4 . 6 | SpaceXAI Docs</a></li>
<li><a href="https://artificialanalysis.ai/models/grok-4-6">Grok 4 . 6 (high) - Intelligence, Performance & Price Analysis</a></li>
<li><a href="https://cursor.com/docs/models/grok-4-6">Grok 4 . 6 | Cursor Docs</a></li>

</ul>
</details>

**Discussion**: Community comments highlight API quirks, such as a default system prompt that can override user instructions, and speculate about how xAI achieved Fable-level performance so quickly, suggesting possible distillation or benchmark hacking. Some users find Grok 4.5/4.6 more pleasant to use than competitors, praising its conciseness and speed, while others note its polarizing reputation but acknowledge it as healthy competition.

**Tags**: `#AI`, `#Grok`, `#xAI`, `#LLM`, `#model release`

---

<a id="item-8"></a>
## [uBlock Origin Stops Blocking Facebook Ads](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 8.0/10

uBlock Origin has officially stopped filtering ads on Facebook, citing the increasing difficulty of keeping up with Facebook's ad-serving techniques. This decision was announced in a Reddit post and reported by Neowin. This marks a significant moment in the ongoing ad-blocking arms race, as one of the most popular ad blockers concedes defeat on a major platform. It highlights the challenges faced by ad blockers and raises questions about the future of user control over online advertising. The decision was made after years of back-and-forth with Facebook, where the social network continuously changed its ad delivery methods to evade blocking. uBlock Origin's move is seen as a practical acknowledgment that the effort required to keep up is no longer sustainable.

hackernews · Markoff · Aug 12, 11:28 · [Discussion](https://news.ycombinator.com/item?id=49270726)

**Background**: Ad blockers like uBlock Origin work by using filter lists to block requests to known ad servers. Facebook has been actively working to circumvent these blockers by obfuscating ad code and integrating ads more seamlessly into content, making them harder to detect. This has led to an ongoing arms race between ad blockers and platforms like Facebook.

<details><summary>References</summary>
<ul>
<li><a href="https://www.neowin.net/news/facebook-ads-are-so-hard-to-block-that-ublock-origin-stopped-filtering-them/">Facebook ads are so hard to block that uBlock Origin ... - Neowin</a></li>
<li><a href="https://www.linkedin.com/pulse/facebooks-ad-blocker-arm-race-escalates-hack-100-million-john-c-abell">Facebook 's ad - blocker arm race escalates; A hack for 100 million...</a></li>
<li><a href="https://arxiv.org/pdf/1811.03194">AdVersarial: Perceptual Ad Blocking meets Adversarial Machine...</a></li>

</ul>
</details>

**Discussion**: The community discussion reflects mixed sentiments, with some users supporting the decision as pragmatic, while others express frustration and speculate about future solutions like computer vision-based ad blocking. Some users also share personal experiences of leaving Facebook or using alternative tools to manage ads.

**Tags**: `#ad-blocking`, `#privacy`, `#Facebook`, `#uBlock Origin`, `#arms race`

---

<a id="item-9"></a>
## [Why Tiny JPEGs Look Different in Chrome](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 8.0/10

The article explains that Chrome's downscaling algorithm renders small JPEGs differently compared to Firefox, causing visual differences. It advises against using JPEGs for icons due to these artifacts. This matters because browser rendering differences can affect user experience and web design consistency. Developers need to be aware of these differences to ensure images display correctly across browsers. Chrome uses a specific downscaling algorithm that can produce blurrier or different results compared to Firefox's sharper but slightly ringing-prone scaling. The article highlights that using appropriately sized images is more important than the format.

hackernews · gutechh · Aug 12, 14:00 · [Discussion](https://news.ycombinator.com/item?id=49272549)

**Background**: JPEG is a lossy format primarily suited for photographs, while PNG is lossless and better for icons. Browsers use different image scaling algorithms, which can cause visual discrepancies when images are resized. Understanding these differences helps developers choose the right format and resolution.

<details><summary>References</summary>
<ul>
<li><a href="https://stackoverflow.com/questions/384991/what-is-the-best-image-downscaling-algorithm-quality-wise">What is the best image downscaling algorithm ... - Stack Overflow</a></li>
<li><a href="https://entropymine.com/resamplescope/notes/browsers/">How web browsers resize images</a></li>

</ul>
</details>

**Discussion**: Commenters noted that similar issues occur with PNGs, and that Chrome's optimization caused problems in Electron apps. Some pointed out that Firefox is working on a fix, and others debated the scaling algorithms, with some preferring Firefox's sharper output.

**Tags**: `#browser`, `#image processing`, `#JPEG`, `#Chrome`, `#Firefox`

---

<a id="item-10"></a>
## [Adam's Rotation Dependence Breaks Implicit Low-Rank Bias, Muon Retains It](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 8.0/10

A new study shows that Adam's per-coordinate second moment breaks rotation invariance, causing it to lose the implicit low-rank bias that gradient descent (GD) preserves, while the Muon optimizer surprisingly retains this bias. Experiments on underdetermined matrix sensing with nine update rules reveal two clean clusters of optimizers based on this property. This finding provides a mechanistic explanation for why adaptive optimizers like Adam often underperform GD on low-rank matrix factorization tasks, which are fundamental to many machine learning models. It could guide the design of new optimizers that combine the benefits of adaptivity with the implicit regularization of GD, impacting fields like deep learning and matrix sensing. The study introduces a one-parameter family that interpolates Adam's denominator from per-coordinate to a single shared scalar, showing recovery improves monotonically, pinpointing anisotropy as the culprit. Muon's behavior is nuanced: it is exact on truly low-rank targets but degrades fastest with spectral tail, crossing over with GD near 4% tail energy. A caveat: the 43-44% held-out error reduction on hyperspectral data uses a train-only learning rate rule that disadvantages Adam; with per-method tuning, the gap shrinks considerably.

reddit · r/MachineLearning · /u/EtherealGlyph · Aug 12, 16:39

**Background**: In factored models like W = UV^T, the loss is invariant to rotations (U,V) → (UQ, VQ), and gradient descent respects this symmetry. Adam's per-coordinate second moment depends on the basis, breaking this invariance. Implicit bias refers to the tendency of optimization algorithms to converge to solutions with certain properties (e.g., low rank) without explicit regularization. Matrix sensing is a problem of recovering a low-rank matrix from linear measurements, often used to study implicit bias.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/rotational-adam-optimizer">Rotational Adam Optimizer</a></li>
<li><a href="https://en.papernotes.org/NeurIPS2025/optimization/understanding_adam_requires_better_rotation_dependent_assumptions/">[Paper Note] Understanding Adam Requires Better Rotation ...</a></li>
<li><a href="https://arxiv.org/pdf/2011.13772">Gradient Descent for Deep Matrix Factorization</a></li>

</ul>
</details>

**Discussion**: The discussion likely includes debates over the fairness of the learning rate tuning, with the author preemptively addressing objections like 'you should have just tuned Adam harder.' Some may question the theoretical scope, as the theory covers only memoryless rules, while momentum is empirical. Others might discuss the surprising Muon results and the conflicting findings in recent literature.

**Tags**: `#optimization`, `#low-rank`, `#Adam`, `#matrix sensing`, `#implicit bias`

---

<a id="item-11"></a>
## [Decoupled Descent: Enforcing Exact Train-Test Error Tracking via AMP Onsager Corrections](https://www.reddit.com/r/MachineLearning/comments/1vlu1se/decoupled_descent_enforcing_exact_traintest_error/) ⭐️ 8.0/10

The paper introduces Decoupled Descent (DD), a novel training method that leverages Approximate Message Passing (AMP) with Onsager corrections to ensure the training error asymptotically equals the test error at each parameter iterate. This addresses the data reuse bias in full-batch gradient descent, as demonstrated on Gaussian mixture models. This work provides a theoretical framework to mitigate the common problem of overfitting, where training error decreases while test error stagnates or worsens. It opens avenues for principled optimal stopping and hyperparameter tuning, potentially impacting how neural networks are trained in practice. The method is validated on a stylized high-dimensional XOR model with a bespoke two-layer network, showing improved train-test error alignment over standard gradient descent. The paper is theoretical in nature, and the author plans to release a PyTorch-compatible package, inviting feature suggestions.

reddit · r/MachineLearning · /u/mlovik1 · Aug 11, 21:06

**Background**: Approximate Message Passing (AMP) is an iterative algorithm family that recovers signals from noisy observations, leveraging state evolution and Onsager corrections to maintain desirable statistical properties. The Onsager correction term is crucial for ensuring that iterates have independent Gaussian-like behavior, which is key to the theoretical guarantees in Decoupled Descent. Data reuse bias refers to the bias introduced when the same data is used multiple times during training, leading to overfitting and a gap between training and test performance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/approximate-message-passing-amp-algorithms">Approximate Message Passing Algorithms</a></li>
<li><a href="https://arxiv.org/abs/2201.07487">[2201.07487] A Concise Tutorial on Approximate Message Passing</a></li>
<li><a href="https://arxiv.org/pdf/2105.02180">A unifying tutorial on Approximate Message Passing</a></li>

</ul>
</details>

**Discussion**: The Reddit post includes the author's engagement with the community, inviting questions and feature suggestions for a future PyTorch package. The discussion sentiment appears positive, with interest in the theoretical approach and potential practical applications, though no specific comments are provided in the given content.

**Tags**: `#machine learning`, `#optimization`, `#approximate message passing`, `#generalization`, `#theory`

---

<a id="item-12"></a>
## [HTML over WebSockets: Real-Time SPAs with Minimal JavaScript](https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/) ⭐️ 7.0/10

The article explores the technique of serving HTML over WebSockets to build real-time single-page applications (SPAs) with minimal client-side JavaScript, comparing it to Server-Sent Events (SSE) and discussing its origins and trade-offs. 该技术为传统的基于 JSON 的 API 提供了一种替代方案，可能简化实时 Web 开发并降低客户端复杂性。它引发了关于针对不同用例选择合适工具的讨论，影响了构建协作或实时更新应用的开发者。 The article highlights that with HTML over WebSockets, requests travel over a persistent channel and responses are pre-assembled HTML, eliminating JSON in between. It also notes that SSE is simpler and cheaper for server-to-client push, while WebSockets are necessary for bidirectional, low-latency communication.

hackernews · redbell · Aug 12, 16:51 · [Discussion](https://news.ycombinator.com/item?id=49275335)

**Background**: Traditional SPAs use JavaScript to fetch JSON data from a server and render it in the browser. HTML over WebSockets flips this by sending ready-to-render HTML over a persistent WebSocket connection, reducing the need for client-side rendering logic. This approach is similar to server-side rendering but with real-time capabilities, and it has roots in frameworks like Phoenix LiveView and Rails' Sync.

<details><summary>References</summary>
<ul>
<li><a href="https://testdriven.io/blog/html-over-websockets/">HTML Over WebSockets | TestDriven.io</a></li>
<li><a href="https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/">HTML over WebSockets : real-time SPAs with... | Andros Fenollosa</a></li>
<li><a href="https://www.sabaoon.dev/blog/websockets-vs-sse-vs-long-polling">WebSockets vs Server - Sent Events vs Long Polling... | Sabaoon</a></li>

</ul>
</details>

**Discussion**: Commenters debated the trade-offs between WebSockets and SSE, with some advocating SSE for simpler server-to-client push and others noting the historical context of the technique, such as Chris McCord's earlier work on Rails' Sync. Some also compared it to Blazor and htmx, highlighting different approaches to achieving similar real-time SPA functionality.

**Tags**: `#WebSockets`, `#SPA`, `#real-time`, `#JavaScript`, `#SSE`

---

<a id="item-13"></a>
## [AI Coding Tools Risk Creating Unmaintainable Codebases](https://simonwillison.net/2026/Aug/12/florian-herrengt/) ⭐️ 7.0/10

Florian Herrengt's quote, highlighted by Simon Willison, illustrates a scenario where AI-assisted coding leads to a convoluted project that no team member understands, with developers relying on AI like Claude to explain their own code. This highlights a growing concern in software engineering: AI-generated code may accelerate development but also introduce cognitive debt and maintainability issues, potentially undermining long-term project health and developer expertise. The quote references 'Fable' (likely Claude Fable 5, Anthropic's coding model) and 'Claude' as AI tools used in the scenario. It underscores that even advanced AI cannot always resolve bugs in overly complex, AI-generated systems, leading to a loss of human understanding.

rss · Simon Willison · Aug 12, 15:08

**Background**: AI-assisted coding tools like GitHub Copilot and Claude Code are increasingly used to generate code quickly. However, without proper review, such code can introduce technical debt, lack documentation, and create architectures that are hard to maintain. This quote reflects a broader industry discussion about the trade-offs between AI productivity gains and code quality.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://blog.codacy.com/what-is-clean-code">What Is Clean Code ? A Guide to Principles and Best Practices</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/ai-generated-code-accelerate-defects-170600845.html">AI -Generated Code Can Accelerate Defects and Technical Debt...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#code maintainability`, `#developer productivity`

---

<a id="item-14"></a>
## [No Lossless Transformations of Natural-Language Text](https://simonwillison.net/2026/Aug/11/there-are-no-lossless-transformations-of-natural-language-text/) ⭐️ 7.0/10

Sophie Alpert published an internal policy for engineers on using AI writing tools, arguing that LLM transformations of text are inherently lossy and that engineers must stand behind every sentence. The post emphasizes that rewriting or rephrasing by an AI without full context inevitably loses information. This policy addresses a growing concern in software engineering and technical writing about accountability when using AI tools. It provides practical guidance that could influence how teams adopt AI writing assistance, emphasizing human responsibility and the preservation of authorial intent. The policy includes a rule that engineers must stand behind every idea and sentence in their docs, and it is not acceptable to dismiss AI-generated content as 'AI wrote that.' The post also explains that every rewrite or rephrase changes meaning, and information is lost when done by an entity without the author's detailed mental representation.

rss · Simon Willison · Aug 11, 23:48

**Background**: Large language models (LLMs) are increasingly used to assist with writing, including technical documentation. However, these models lack the author's original intent and context, so any transformation they perform can alter meaning. This has led to discussions about the ethical and practical implications of AI-assisted writing, particularly regarding accountability and accuracy.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48980425">There are no lossless transformations of natural - language text</a></li>
<li><a href="https://www.linkedin.com/posts/katie-miserany_there-are-no-lossless-transformations-of-activity-7491169182865293312-hLj8">There are no lossless transformations of natural - language text</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion highlights agreement with the core idea, with some commenters sharing personal experiences of AI rewriting losing nuance. Others debate the extent to which AI can ever preserve meaning, and some suggest that the policy is a good baseline for responsible AI use.

**Tags**: `#AI ethics`, `#technical writing`, `#LLM`, `#software engineering`, `#documentation`

---

<a id="item-15"></a>
## [New site ranks CS conferences by destination quality, not prestige](https://www.reddit.com/r/MachineLearning/comments/1vmbdk6/i_built_an_honest_cs_conference_ranking_sorted_by/) ⭐️ 7.0/10

A developer launched honestcsrankings.org, a website that ranks about 540 upcoming CORE-ranked computer science conferences by destination quality—including weather, safety, cost, and city vibe—rather than academic prestige. The tool also features an 'Upsets' tab highlighting A* venues in poor locations and allows filtering by field, rank, or deadlines. This tool addresses a practical need in the CS research community, where conference location often influences attendance and travel decisions. By combining academic rankings with travel considerations, it could help researchers balance career advancement with personal enjoyment, potentially influencing how conferences are chosen and attended. The ranking uses real climate data for weather, the Global Peace Index for safety, World Bank price levels for cost, and accessibility and city vibe metrics. ICML/ICLR 2027 are missing because they are not yet announced, and COLM is absent because CORE has not ranked it; smaller conferences are scraped from WikiCFP, so some errors may exist.

reddit · r/MachineLearning · /u/JohnAZoidberg77 · Aug 12, 11:23

**Background**: CORE ranking is a widely used system that categorizes computer science conferences into tiers (A*, A, B, C) based on academic prestige and impact. Researchers often consider both the conference's reputation and the travel experience when deciding where to submit and attend. The Global Peace Index, produced by the Institute for Economics and Peace, measures peacefulness using indicators like conflict deaths and safety, while World Bank price levels provide comparative cost-of-living data across countries.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Global_Peace_Index">Global Peace Index - Wikipedia</a></li>
<li><a href="https://www.economicsandpeace.org/global-peace-index/">Global Peace Index - Institute for Economics & Peace</a></li>
<li><a href="https://data.worldbank.org/">World Bank Open Data from The World Bank : Data</a></li>

</ul>
</details>

**Tags**: `#conference ranking`, `#CS research`, `#travel`, `#tool`, `#academia`

---

<a id="item-16"></a>
## [Seeking RL/Planning Advice for Stochastic Merge Puzzle with Afterstates](https://www.reddit.com/r/MachineLearning/comments/1vlfavg/planningrl_for_a_stochastic_singleplayer_merge/) ⭐️ 7.0/10

A developer is seeking advice on reinforcement learning and planning approaches for a stochastic single-player merge puzzle that features afterstates, previewed random events, and a long-horizon throughput objective. The puzzle has a 6x7 board, 30 possible actions, and a random tile drop every fourth action, with the upcoming drop revealed one move in advance. This problem is a niche but technically rich research area that combines afterstates, stochastic planning, and long-horizon optimization, which could inspire new algorithms or adaptations of existing ones. The insights gained could benefit similar games and broader RL/planning research on handling previewed chance events and throughput objectives. The game involves 6 vertical stacks with max height 7, and actions move complete runs of equal tiles, with cascading merges and a merge value of 9 disappearing for points. The state representation includes a 6x7x9 one-hot board, cycle phase, preview values, and history features, while the network is column-permutation equivariant with separate heads for actions and values.

reddit · r/MachineLearning · /u/CaiwenGong · Aug 11, 11:53

**Background**: Afterstates are states that occur immediately after an action but before the environment's random outcome, allowing value functions to be learned more efficiently by reducing state space complexity. In stochastic games, previewing random events can enable better planning by allowing the agent to condition its actions on known future information. The puzzle described resembles 2048 but with a larger action space and stack constraints, and the objective is to maximize throughput (number of 9s) over a fixed time horizon.

<details><summary>References</summary>
<ul>
<li><a href="https://stats.stackexchange.com/questions/411932/reinforcement-learning-afterstate-and-afterstate-value-functions">Reinforcement Learning : Afterstate and Afterstate value functions</a></li>
<li><a href="https://arxiv.org/pdf/2111.14375">Final Adaptation Reinforcement Learning</a></li>
<li><a href="https://arxiv.org/pdf/2603.18994">Evaluating Game Difficulty in Tetris Block Puzzle</a></li>

</ul>
</details>

**Discussion**: No comments were provided for this news item.

**Tags**: `#reinforcement learning`, `#planning`, `#stochastic games`, `#afterstates`, `#game AI`

---

<a id="item-17"></a>
## [Developer Shares 2026 Eclipse Webcam Aggregation Site](https://jonty.github.io/2026_eclipse_webcams/) ⭐️ 6.0/10

A developer, jonty, shared a webcam aggregation site for the 2026 solar eclipse, built initially for the 2024 US eclipse and updated for the current event. The site coordinates live webcams across Iceland and Spain, where the eclipse is visible. This project provides a practical, accessible way for people worldwide to experience a rare astronomical event in real time, fostering community engagement and shared experience. It highlights the value of simple, utility-driven side projects in bringing people together around natural phenomena. The site was built quickly in 2024 and finished minutes before totality started, and the developer forgot about it until a friend asked. It coordinates webcams across Iceland and Spain, and the developer notes that coordinating a 'DDOS' on cameras was not planned, hoping it doesn't break.

hackernews · zoenolan · Aug 12, 11:53 · [Discussion](https://news.ycombinator.com/item?id=49270953)

**Background**: Solar eclipses occur when the Moon passes between the Earth and the Sun, temporarily blocking sunlight. They are relatively rare events at any given location, making them significant for both scientific study and public interest. Webcam aggregation sites like this allow remote viewing, expanding access to those not in the path of totality.

**Discussion**: The community discussion includes personal anecdotes about traveling to view eclipses, with one user sharing their experience of driving hundreds of kilometers to escape clouds in 2024. Another user highlights the historical significance of eclipses, referencing Thales of Miletus's prediction in 585 BC as the 'Birth of Science'. Users also share additional resources like webcams and solar panel monitoring data.

**Tags**: `#eclipse`, `#webcams`, `#community`, `#astronomy`, `#side-project`

---

<a id="item-18"></a>
## [AmigaDOS Developer Tim King Passes Away](https://amiga-news.de/en/news/AN-2026-08-00070-EN.html) ⭐️ 6.0/10

Tim King, a key developer of AmigaDOS, has died, as reported by amiga-news.de. The community has responded with tributes and remembrances of his contributions. Tim King's work on AmigaDOS was foundational to the Amiga platform, which influenced many users and developers. His passing is significant to the retrocomputing community, which continues to value and preserve his legacy. AmigaDOS was the disk operating system of AmigaOS, initially based on a TRIPOS port written in BCPL, and later rewritten in C. Tim King was also known as the founder of UK Online, as mentioned in one community comment.

hackernews · doener · Aug 12, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49272655)

**Background**: AmigaOS, introduced with the Amiga 1000 in 1985, was a pioneering multitasking operating system. AmigaDOS handled file systems and the command-line interface, and its development involved contributions from MetaComCo and later rewrites. The Amiga platform has a dedicated retrocomputing community that continues to discuss and preserve its history.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AmigaDOS">AmigaDOS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amiga_Operating_System">Amiga Operating System</a></li>

</ul>
</details>

**Discussion**: Community comments express personal gratitude and nostalgia, with users crediting Tim King for their careers and fond memories of using AmigaDOS. One commenter mentions an interview from October 2021, and another recalls him as the founder of UK Online, describing him as friendly and helpful.

**Tags**: `#Amiga`, `#retrocomputing`, `#obituary`, `#AmigaDOS`, `#community`

---

<a id="item-19"></a>
## [Mass Scans Spoof AI Bots, But Experts Say It's Old News](https://knownagents.com/insights) ⭐️ 6.0/10

Recent reports indicate that someone is running mass vulnerability scans while spoofing AI bot user agents like ClaudeBot. This activity is similar to long-standing automated scanning, but with a new layer of deception. This matters because it highlights the evolving tactics of attackers who blend malicious activity with normal traffic, potentially evading detection. It also underscores the ongoing challenge of distinguishing legitimate AI crawlers from malicious scanners, affecting security teams and website administrators. The spoofed scans reportedly began around July 30 and ramped up significantly by August 6, with a 5x increase in volume. Attackers often fake user agents, and blocking VPS providers can eliminate many of these faked bots.

hackernews · gavinhking · Aug 12, 14:02 · [Discussion](https://news.ycombinator.com/item?id=49272569)

**Background**: AI bot user agents are strings that identify crawlers like GPTBot or ClaudeBot to websites. Mass vulnerability scanning has been common since the early 2000s, with tools like Code Red and masscan. Spoofing user agents is a known technique, but combining it with AI bot identities is a relatively new tactic.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49272569">Someone is running mass vulnerability scans , spoofing AI bots like...</a></li>
<li><a href="https://hacknjill.com/cybercrime-and-incidents/someone-is-running-mass-vulnerability-scans-spoofing-ai-bots-like-claudebot/">Someone Is Running Mass Vulnerability Scans , Spoofing AI Bots...</a></li>
<li><a href="https://llmscentral.com/blog/ai-bot-user-agents-complete-guide">Complete Guide to AI Bot User - Agents : GPTBot... | LLMS Central</a></li>

</ul>
</details>

**Discussion**: Community comments largely dismiss the novelty, noting that such scans are routine and have been happening for decades. Users share practical advice, such as checking ASN ownership and blocking VPS providers, and caution against trusting linked source code.

**Tags**: `#security`, `#vulnerability scanning`, `#bot detection`, `#AI bots`

---

<a id="item-20"></a>
## [Datasette Upload DBS 0.5a0 Adds Formalized API for Atomic Database Swaps](https://simonwillison.net/2026/Aug/11/datasette-upload-dbs/) ⭐️ 6.0/10

Datasette-upload-dbs 0.5a0 introduces a formalized API endpoint that allows users to upload and atomically swap SQLite databases via a simple curl command. This enables automated deployments, such as building databases in CI/CD pipelines and swapping them into production. This release significantly enhances the automation capabilities of Datasette, making it easier for developers to integrate database updates into their DevOps workflows. By providing a stable API, it reduces manual intervention and enables continuous deployment of database changes. The new API requires an authentication token and accepts a database file and a database name as multipart form data. The uploaded database is saved, verified, and then atomically swapped so that the specified endpoint serves the new version without downtime.

rss · Simon Willison · Aug 11, 20:35

**Background**: Datasette is a tool for exploring and publishing SQLite databases, and plugins extend its functionality. The datasette-upload-dbs plugin allows users to upload new databases to a running instance, and this update formalizes the process with a dedicated API endpoint, making it suitable for scripted and automated use.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/plugins/datasette-upload-dbs">datasette - upload - dbs - a plugin for Datasette</a></li>
<li><a href="https://github.com/simonw/datasette-upload-dbs">GitHub - simonw/ datasette - upload - dbs : Upload SQLite database files...</a></li>
<li><a href="https://simonwillison.net/2026/aug/11/datasette-upload-dbs/">Release: datasette - upload - dbs 0.5a0 | Simon Willison’s Weblog</a></li>

</ul>
</details>

**Tags**: `#Datasette`, `#SQLite`, `#API`, `#DevOps`, `#Plugin`

---

<a id="item-21"></a>
## [AAAI 2027 Reviewers Note Lack of Code Submissions](https://www.reddit.com/r/MachineLearning/comments/1vlqjby/aaai_2027_review_no_code_submission_d/) ⭐️ 6.0/10

A reviewer for AAAI 2027 reported that a surprisingly low number of submissions include code implementations, despite the conference's explicit emphasis on reproducibility. The reviewer is considering penalizing papers without code in their initial scores and seeks community input. This highlights a persistent gap between conference policies and actual practices in AI research, potentially undermining reproducibility efforts. If reviewers penalize missing code, it could pressure authors to share code more consistently, improving the reliability of published results. The reviewer notes that AI assistants can generate empirical papers with artificial results in hours, making code absence more suspicious. AAAI's review guidelines ask reviewers to assess reproducibility, but code submission is not mandatory, only encouraged.

reddit · r/MachineLearning · /u/wontonut · Aug 11, 18:58

**Background**: AAAI (Association for the Advancement of Artificial Intelligence) is a major AI conference that emphasizes reproducibility through guidelines and checklists. However, code sharing is often voluntary, and many authors cite concerns about idea theft or lack of time. The reproducibility crisis in AI has led to calls for mandatory code and data sharing, but implementation remains inconsistent.

<details><summary>References</summary>
<ul>
<li><a href="https://aaai.org/conference/aaai/aaai-25/submission-instructions/">AAAI -25 Submission Instructions - AAAI</a></li>
<li><a href="https://aaai.org/conference/aaai/aaai-27/main-technical-track-call/">AAAI -27 Main Technical Track Call - AAAI</a></li>
<li><a href="https://folk.idi.ntnu.no/odderik/reproducibility_guidelines_how_to.html">folk.idi.ntnu.no/odderik/ reproducibility _guidelines_how_to.html</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion likely includes mixed opinions: some agree that code should be required for reproducibility, while others argue that not all research requires code (e.g., theory papers) and that penalizing could disadvantage certain fields. Some may also share experiences with code review and the risk of idea theft.

**Tags**: `#AAAI`, `#reproducibility`, `#peer review`, `#machine learning`

---

<a id="item-22"></a>
## [Agentic World Cup: LLM Agents Compete in 1v1 Soccer](https://www.reddit.com/r/MachineLearning/comments/1vllvmn/we_built_the_agentic_world_cup_llms_that_compete/) ⭐️ 6.0/10

The Agentic World Cup platform has been launched, allowing users to sign in, select an LLM, coach it through prompting, and submit it to compete in 1v1 soccer matches against other agents. Rankings are published on the site by Friday. This platform addresses the embodiment gap in AI by providing a sports-based benchmark for embodied intelligence, which is a novel approach compared to traditional coding or math tasks. It could enable broader participation in embodied AI research and testing, potentially accelerating progress in this area. The platform is designed to let agents 'think on their feet,' requiring real-time decision-making in a dynamic environment. The long-term vision includes allowing anyone to test their latest algorithms on public embodied challenges, with sports as the apex of such challenges.

reddit · r/MachineLearning · /u/agenticworldcup · Aug 11, 16:12

**Background**: The embodiment gap refers to the limitation of current AI systems that lack physical bodies and thus cannot interact with the world as humans do. Embodied AI aims to bridge this gap by equipping agents with bodies or simulated environments. Sports provide a complex, dynamic testbed for embodied intelligence, requiring perception, decision-making, and motor control.

<details><summary>References</summary>
<ul>
<li><a href="https://agenticworldcup.ai/">Agentic World Cup</a></li>
<li><a href="https://theconsciousness.ai/posts/kadambi-embodiment-multimodal-llm-consciousness-2026/">The Body Gap : Why AI Still Can't Know What... | The Consciousness AI</a></li>

</ul>
</details>

**Tags**: `#embodied AI`, `#LLM agents`, `#benchmarking`, `#sports simulation`

---