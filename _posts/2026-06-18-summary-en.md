---
layout: default
title: "Horizon Summary: 2026-06-18 (EN)"
date: 2026-06-18
lang: en
---

> From 49 items, 29 important content pieces were selected

---

1. [GLM-5.2: Most Powerful Open-Weight Text LLM Released](#item-1) ⭐️ 9.0/10
2. [Epic Games Open-Sources Lore VCS for Large Binary Files](#item-2) ⭐️ 8.0/10
3. [US delays blacklisting DeepSeek, designates over 100 Chinese firms](#item-3) ⭐️ 8.0/10
4. [U.S. Science in Crisis: Broken Compact Drives Researchers Abroad](#item-4) ⭐️ 8.0/10
5. [Running Firecracker VMs in EC2 for Sub-Second Browser Launch](#item-5) ⭐️ 8.0/10
6. [RFC 10008 Defines New HTTP QUERY Method](#item-6) ⭐️ 8.0/10
7. [Tesco moves 40,000 workloads off VMware over Broadcom pricing](#item-7) ⭐️ 8.0/10
8. [Charity Majors: AI Flips Code Economics, Demands More Discipline](#item-8) ⭐️ 8.0/10
9. [Export Controls on AI Models Undermine US Cyber Defense](#item-9) ⭐️ 8.0/10
10. [Microsoft's NextLat: Transformers Predict Own Latent States](#item-10) ⭐️ 8.0/10
11. [Speculative Decoding: Fast LLM Inference](#item-11) ⭐️ 8.0/10
12. [Contrastive Targeted SFT for Causal Circuit Mapping in LLMs](#item-12) ⭐️ 8.0/10
13. [Leakage-Clean Verifier for Robot Manipulation](#item-13) ⭐️ 8.0/10
14. [Midjourney Pivots to Medical Imaging, Experts Skeptical](#item-14) ⭐️ 7.0/10
15. [Adam (YC W25) Launches Open-Source AI CAD Platform](#item-15) ⭐️ 7.0/10
16. [Volkswagen blocks GrapheneOS users via API lock](#item-16) ⭐️ 7.0/10
17. [Datasette 1.0a34 Adds CRUD UI for Rows](#item-17) ⭐️ 7.0/10
18. [Georgi Gerganov Endorses Qwen3.6-27B for Local Coding](#item-18) ⭐️ 7.0/10
19. [Anthropic's Fable jailbreak: expected cyberdefense behavior](#item-19) ⭐️ 7.0/10
20. [Can foundational AI research be done without HPC?](#item-20) ⭐️ 7.0/10
21. [Probe Strength Analysis in Mechanistic Interpretability](#item-21) ⭐️ 7.0/10
22. [8-bit Live Baseball Gamecast from MLB Data](#item-22) ⭐️ 6.0/10
23. [Why Talking Through Problems Beats Thinking Alone](#item-23) ⭐️ 6.0/10
24. [Robot Sprint Game Compares Claude, Grok, and DeepSeek](#item-24) ⭐️ 6.0/10
25. [Click-to-Play Web Component Defers GIF Loading](#item-25) ⭐️ 6.0/10
26. [Datasette-Tailscale Plugin Exposes Local DB Securely](#item-26) ⭐️ 6.0/10
27. [Open-Source ML Pipeline for Hong Kong Horse Racing](#item-27) ⭐️ 6.0/10
28. [ECCV 2026 Final Decisions Expected June 17](#item-28) ⭐️ 6.0/10
29. [GAN on Raspberry Pi 4 Powers Physical NFT Minting Device](#item-29) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [GLM-5.2: Most Powerful Open-Weight Text LLM Released](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai released GLM-5.2, a 753B-parameter open-weight LLM under MIT license with a 1M-token context window, achieving top scores on the Artificial Analysis Intelligence Index. GLM-5.2 is likely the most powerful text-only open-weight LLM, surpassing models like DeepSeek V4 Pro and Kimi K2.6, which could accelerate open-source AI research and applications. The model uses a Mixture-of-Experts architecture with 40 active parameters, but consumes more output tokens per task (43k) compared to peers. It also ranks 2nd on Code Arena WebDev leaderboard despite lacking image input.

rss · Simon Willison · Jun 17, 23:58

**Background**: Large language models (LLMs) like GLM-5.2 are trained on vast text data to generate human-like text. Mixture-of-Experts (MoE) architectures activate only a subset of parameters per token, improving efficiency. A 1M-token context window allows the model to process very long documents or conversations in one go.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/zai-org/GLM-5.2">zai-org/GLM-5.2 · Hugging Face</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM-5.2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.buildfastwithai.com/blogs/glm-5-2-review-2026">GLM-5.2 Review 2026: Z.ai's 1M-Context AI Model</a></li>

</ul>
</details>

**Discussion**: The community is excited about GLM-5.2's benchmark performance and open license, but some note its high token usage and lack of vision capabilities. The model's strong SVG generation is praised, though results can be inconsistent.

**Tags**: `#LLM`, `#open-source`, `#AI`, `#GLM-5.2`, `#benchmark`

---

<a id="item-2"></a>
## [Epic Games Open-Sources Lore VCS for Large Binary Files](https://lore.org/) ⭐️ 8.0/10

Epic Games has open-sourced Lore, a new version control system built from scratch in Rust, designed for scalability with large binary files and exclusive file locking, announced at State of Unreal 2026 alongside Unreal Engine 5.8. Lore directly addresses the pain points of game development where Git fails, offering a modern, open-source alternative to Perforce for managing large binary assets and enabling exclusive locks, which could reshape version control workflows in the game industry. Lore is MIT-licensed, written in Rust, and optimized for projects combining code with large binary assets like textures, 3D models, and audio files, supporting exclusive file locking essential for artists.

hackernews · regnerba · Jun 17, 14:30 · [Discussion](https://news.ycombinator.com/item?id=48571081)

**Background**: Version control systems like Git are excellent for text-based code but struggle with large binary files common in game development, leading to the industry's reliance on Perforce. Git LFS attempts to address this but adds complexity and lacks native exclusive locking. Lore aims to provide a purpose-built solution from the ground up.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/EpicGames/lore">Lore is a next-generation, open source revision control system</a></li>
<li><a href="https://www.phoronix.com/news/Epic-Games-Lore-VCS">Epic Games Announces Lore Open-Source Version Control System</a></li>
<li><a href="https://byteiota.com/epic-games-open-sources-lore-a-vcs-built-for-binary-files/">Epic Games Open-Sources Lore: A VCS Built for Binary Files</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights that Lore is seen as a promising challenger to Perforce, especially for Unreal Engine development, with users noting Perforce's complexity and Git's inadequacy for binary files. Some commenters express hope for a simpler alternative, while others caution that Lore is still early and needs to prove itself.

**Tags**: `#version control`, `#game development`, `#open source`, `#scalability`, `#Perforce`

---

<a id="item-3"></a>
## [US delays blacklisting DeepSeek, designates over 100 Chinese firms](https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/) ⭐️ 8.0/10

The US government has decided to delay blacklisting Chinese AI startup DeepSeek, but has designated over 100 other Chinese companies as security risks, according to a Reuters report. This move comes amid ongoing debates about tech decoupling and AI export controls between the US and China. This decision highlights the complex geopolitical tensions in the AI industry, potentially affecting global supply chains and the competitive landscape for AI models. The delay for DeepSeek, known for its cost-effective open-weight models, suggests a nuanced approach, but the broader list signals continued pressure on Chinese tech firms. DeepSeek, founded in 2023, has gained attention for its R1 model, which rivals GPT-4 at a fraction of the training cost. The company's models are open-weight and available under the MIT License, and it has successfully trained on weaker AI chips due to export restrictions.

hackernews · giuliomagnifico · Jun 17, 03:55 · [Discussion](https://news.ycombinator.com/item?id=48565498)

**Background**: DeepSeek is a Chinese AI company that develops large language models, known for its cost-efficient training methods and open-weight releases. The US has imposed export controls on advanced AI chips to China, aiming to limit China's AI capabilities, but DeepSeek's success with restricted hardware has challenged these assumptions. The Entity List restricts US companies from selling goods and services to listed firms, but does not prohibit purchases from them.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://www.fdd.org/analysis/2026/06/02/commerce-department-admits-failure-to-enforce-ai-export-controls-on-china/">Commerce Department Admits Failure To Enforce AI Export ...</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed views: some users appreciate DeepSeek's affordability and performance, while others criticize US export controls as hypocritical or difficult to enforce. There is also curiosity about the actual list of 100 firms and debate over the effectiveness of such measures.

**Tags**: `#AI`, `#geopolitics`, `#export controls`, `#DeepSeek`, `#US-China`

---

<a id="item-4"></a>
## [U.S. Science in Crisis: Broken Compact Drives Researchers Abroad](https://www.scientificamerican.com/article/americas-compact-between-science-and-politics-is-broken/) ⭐️ 8.0/10

A Scientific American article reports that the U.S. scientific enterprise is in chaos due to a broken political compact, funding cuts, and visa restrictions, prompting many researchers to leave the country. This crisis threatens U.S. leadership in science and innovation, as talent and funding drain away, potentially weakening national competitiveness and public trust in science. The article highlights arbitrary grant cancellations, delayed disbursements, and political interference in research topics like DEI, alongside visa restrictions that block foreign talent.

hackernews · presspot · Jun 17, 09:54 · [Discussion](https://news.ycombinator.com/item?id=48568058)

**Background**: The U.S. has long relied on a compact where science receives stable funding and political autonomy in exchange for societal benefits. Recent political shifts have eroded this compact, leading to funding instability and politicization of research.

**Discussion**: Commenters share personal stories of leaving the U.S. due to funding and visa issues, with many expressing despair and noting a pervasive sense of crisis in academic labs.

**Tags**: `#science policy`, `#research funding`, `#U.S. politics`, `#academia`, `#immigration`

---

<a id="item-5"></a>
## [Running Firecracker VMs in EC2 for Sub-Second Browser Launch](https://browser-use.com/posts/firecracker-browser-infra) ⭐️ 8.0/10

Browser-use.com describes how to run Firecracker microVMs on EC2 to launch browsers in under one second, achieving 81% stealth benchmark success against bot detection. This approach enables high-speed, stealthy browser automation for web scraping and testing, potentially reducing detection by anti-bot systems and improving efficiency for automated tasks. Nested virtualization on regular EC2 instances (non-metal) has only been supported since February 2026, previously requiring bare-metal instances to run Firecracker VMs.

hackernews · gregpr07 · Jun 16, 15:15 · [Discussion](https://news.ycombinator.com/item?id=48556561)

**Background**: Firecracker is an open-source virtualization technology by AWS that creates lightweight microVMs, combining security of hardware virtualization with speed of containers. The AWS Nitro hypervisor offloads I/O to dedicated hardware, enabling nested virtualization on EC2. Anti-bot measures detect headless browsers through automation signals, making stealthy browser automation challenging.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Firecracker_(software)">Firecracker (software) - Wikipedia</a></li>
<li><a href="https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/amazon-ec2-nested-virtualization.html">Use nested virtualization to run hypervisors in Amazon EC2 instances - Amazon Elastic Compute Cloud</a></li>
<li><a href="https://aws.amazon.com/ec2/nitro/">Lightweight Hypervisor - AWS Nitro System - AWS</a></li>

</ul>
</details>

**Discussion**: Commenters raised ethical concerns about bypassing anti-bot measures, noted the recent availability of nested virtualization on non-metal EC2 instances, and suggested alternatives like Lightpanda for better performance. Some also compared the approach to using AWS Lambda for simpler architecture.

**Tags**: `#Firecracker`, `#EC2`, `#browser automation`, `#virtualization`, `#anti-bot`

---

<a id="item-6"></a>
## [RFC 10008 Defines New HTTP QUERY Method](https://www.rfc-editor.org/info/rfc10008/) ⭐️ 8.0/10

RFC 10008 introduces a new HTTP QUERY method that allows safe, idempotent requests with a request body, filling a gap left by GET (which has no body) and POST (which is not safe or idempotent). This standardizes a common pattern for complex queries (e.g., GraphQL, search APIs) where a body is needed but the operation should be safe and cacheable, potentially improving API design and web interoperability. The QUERY method is defined as safe and idempotent, and it supports caching based on the request body. It also introduces an Accept-Query header for content negotiation.

hackernews · schappim · Jun 17, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48568502)

**Background**: HTTP methods like GET are safe and idempotent but cannot carry a body, while POST can carry a body but is neither safe nor idempotent. This created a gap for operations like complex searches that need a body but should be safe and cacheable. RFC 10008 fills this gap with the QUERY method.

<details><summary>References</summary>
<ul>
<li><a href="https://www.rfc-editor.org/info/rfc10008/">RFC 10008 : The HTTP QUERY Method | RFC Editor</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods">HTTP request methods - HTTP | MDN</a></li>
<li><a href="https://zenn.dev/catatsuy/scraps/73c262be2e4145">RFC 10008 : HTTP QUERY Method</a></li>

</ul>
</details>

**Discussion**: Commenters discussed caching challenges with request bodies, potential HTML form support for QUERY to avoid POST refresh warnings, and noted that the RFC number has reached five digits. Some expressed surprise that GET with a body was rejected in favor of a new method.

**Tags**: `#HTTP`, `#RFC`, `#web standards`, `#API design`

---

<a id="item-7"></a>
## [Tesco moves 40,000 workloads off VMware over Broadcom pricing](https://arstechnica.com/information-technology/2026/06/tesco-moving-40000-server-workloads-off-vmware-amid-broadcoms-abusive-conduct/) ⭐️ 8.0/10

Tesco, the UK's largest supermarket chain, is migrating 40,000 server workloads away from VMware to an unnamed open-source alternative, citing Broadcom's abusive pricing and support cuts. This major enterprise migration signals a growing backlash against Broadcom's post-acquisition strategy of aggressive price hikes and reduced support, potentially accelerating industry-wide shifts to open-source virtualization. Tesco faces migration challenges because its new virtualization software is incompatible with Veeam and Zerto backup products it currently uses. The company is also dealing with data security concerns during the transition.

hackernews · Bender · Jun 17, 21:00 · [Discussion](https://news.ycombinator.com/item?id=48576838)

**Background**: VMware is a leading virtualization platform that allows multiple virtual servers to run on a single physical machine. Broadcom acquired VMware in November 2023 and subsequently introduced per-core subscription licensing, leading to price increases of 150-1000% for many customers. This has prompted many organizations to explore alternatives like Proxmox or Nutanix.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/information-technology/2024/10/a-year-after-broadcoms-vmware-buy-customers-eye-exit-strategies/">Disgruntled customers discuss quitting VMware - Ars Technica</a></li>
<li><a href="https://us.ovhcloud.com/resources/blog/navigating-broadcom-new-licensing-model/">VMware Pricing Changes : A Practical Path for SMBs Navigating...</a></li>
<li><a href="https://www.softwareseni.com/broadcom-vmware-pricing-changes-understanding-the-licensing-crisis-driving-migration/">Broadcom VMware Pricing Changes - Understanding... - SoftwareSeni</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong criticism of Broadcom's business model, describing it as 'tech bottom feeding' that buys declining companies with moats and squeezes them. One noted that Broadcom's marketing for Proxmox is 'extremely effective' as customers flee VMware.

**Tags**: `#VMware`, `#Broadcom`, `#enterprise migration`, `#virtualization`, `#open source`

---

<a id="item-8"></a>
## [Charity Majors: AI Flips Code Economics, Demands More Discipline](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors argues that in 2025, AI made code generation effectively free and instant, turning code from a treasured asset into a disposable commodity, which paradoxically requires more engineering discipline, not less. This insight challenges the common assumption that AI reduces the need for rigorous engineering practices, highlighting a paradigm shift where the ease of generating code increases the importance of system design, testing, and maintainability. Majors specifically notes that lines of code went from being 'treasured, reused, cared for and carefully curated' to 'disposable and regenerable' practically overnight, emphasizing the economic inversion in code production.

rss · Simon Willison · Jun 17, 17:12

**Background**: Historically, writing code was labor-intensive and expensive, leading developers to carefully craft and reuse code. With generative AI, code can be produced rapidly at low cost, but this abundance introduces new challenges in managing complexity, ensuring correctness, and maintaining systems over time.

**Tags**: `#ai-assisted-programming`, `#software-engineering`, `#generative-ai`, `#economics-of-code`

---

<a id="item-9"></a>
## [Export Controls on AI Models Undermine US Cyber Defense](https://simonwillison.net/2026/Jun/16/fable-5-export-controls/#atom-everything) ⭐️ 8.0/10

The US government imposed export controls on Anthropic's Claude Fable 5 and Mythos 5 models, citing concerns about cyber attack capabilities. However, researchers found that the 'jailbreak' that triggered the ban was actually a defensive request to fix security vulnerabilities in code. This policy inadvertently harms US cyber defense by preventing defenders from using AI to find and fix security bugs, which is the most valuable application of AI for cybersecurity. It highlights a dangerous disconnect between non-technical policymakers and the practical needs of security researchers. The models were asked to review code with known CVEs and deliberately planted vulnerabilities, then to 'fix this code' — a standard defensive task. The export controls, issued via a BIS 'Is Informed' letter, require Anthropic to obtain a license before sharing the models with any foreign national.

rss · Simon Willison · Jun 16, 05:20

**Background**: Export controls on AI models aim to prevent adversaries from using advanced AI for offensive cyber operations. However, the same capabilities that enable offensive use — such as generating exploit code — are also essential for defensive security tasks like vulnerability detection and patch verification. The CVE system catalogs known security vulnerabilities, and fixing them is a core part of cyber defense.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aimadetools.com/blog/claude-fable-5-banned-us-export-controls">Claude Fable 5 Banned — US Government Export Controls ...</a></li>
<li><a href="https://cybersecuritynews.com/claude-mythos-5-and-fable-5-export/">U.S. Commerce Dept Imposes Export Controls on Anthropic's ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerabilities_and_Exposures">Common Vulnerabilities and Exposures - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#export controls`, `#cybersecurity`, `#AI safety`, `#open source`

---

<a id="item-10"></a>
## [Microsoft's NextLat: Transformers Predict Own Latent States](https://www.reddit.com/r/MachineLearning/comments/1u84mio/nextlatent_prediction_transformers_r/) ⭐️ 8.0/10

Microsoft Research proposes Next-Latent Prediction (NextLat), a self-supervised method that trains transformers to predict their own next latent state in addition to the next token, enabling compact world models and up to 3.3x faster inference via self-speculative decoding. NextLat addresses the myopia of next-token prediction by providing denser supervision in latent space, improving representation learning and data efficiency. The self-speculative decoding capability offers a practical speedup for transformer inference without an auxiliary model. The method extends standard next-token prediction with an auxiliary loss that predicts the next latent state given the current latent state and next token. After training on TinyStories, linear probes on hidden states can predict 1–20 tokens ahead, indicating compact world model formation.

reddit · r/MachineLearning · /u/jayden_teoh_ · Jun 17, 08:44

**Background**: Standard autoregressive transformers predict tokens one by one, which can be inefficient and myopic. Self-supervised learning aims to learn useful representations without labeled data. Self-speculative decoding accelerates inference by using a cheaper approximation of the same model to draft tokens, then verifying them in a single forward pass.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2511.05963v1">Next - Latent Prediction Transformers Learn Compact World Models</a></li>
<li><a href="https://github.com/JaydenTeoh/NextLat">GitHub - JaydenTeoh/NextLat: Codebase for " Next - Latent Prediction ..."</a></li>

</ul>
</details>

**Tags**: `#transformers`, `#self-supervised learning`, `#representation learning`, `#inference acceleration`, `#world models`

---

<a id="item-11"></a>
## [Speculative Decoding: Fast LLM Inference](https://www.reddit.com/r/MachineLearning/comments/1u83kzt/what_is_speculative_decoding_trending_on/) ⭐️ 8.0/10

Speculative decoding is trending on Papers with Code, with SGLang releasing a blog post on achieving state-of-the-art latencies using Modal and Z.ai's DFlash speculative decoding models. This technique can speed up LLM inference by 2-3x without sacrificing output quality, making it crucial for reducing serving costs and improving user experience in real-time applications. Speculative decoding uses a fast draft model to propose multiple tokens, which are then verified in parallel by a larger target model. SGLang's implementation supports multiple draft methods including EAGLE-2/3, MTP, DFLASH, and NGRAM variants.

reddit · r/MachineLearning · /u/NielsRogge · Jun 17, 07:41

**Background**: Large language models generate tokens one by one, which is slow. Speculative decoding accelerates this by having a small model draft several tokens at once, then the large model checks them all in parallel, accepting correct ones and discarding incorrect ones. This allows generating multiple tokens per step while maintaining quality.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-speculative-decoding-for-reducing-latency-in-ai-inference/">An Introduction to Speculative Decoding for Reducing Latency ...</a></li>
<li><a href="https://research.google/blog/looking-back-at-speculative-decoding/">Looking back at speculative decoding - Google Research</a></li>
<li><a href="https://docs.sglang.io/docs/advanced_features/speculative_decoding">Speculative Decoding - SGLang Documentation</a></li>

</ul>
</details>

**Tags**: `#speculative decoding`, `#LLM inference`, `#optimization`, `#SGLang`, `#machine learning`

---

<a id="item-12"></a>
## [Contrastive Targeted SFT for Causal Circuit Mapping in LLMs](https://www.reddit.com/r/MachineLearning/comments/1u8if6l/contrastive_targeted_sft_as_a_mechinterp_method/) ⭐️ 8.0/10

A self-taught researcher proposes using contrastive targeted supervised fine-tuning (SFT) to locate circuits for specific capabilities in a 31B model and build causal dependency graphs between dimensions by ablating discovered circuits and measuring degradation in other dimensions. This approach could enable a closed-loop training strategy where mechanistic interpretability findings guide subsequent training rounds, potentially leading to more efficient and controllable LLM training by understanding how capabilities interact causally. The method involves training contrastive variants from the same checkpoint—examples with a dimension deep vs shallow—and then finding the difference between checkpoints to locate the circuit. The researcher also plans to test dimension composition via prompts requiring causal chaining and use activation steering as a diagnostic.

reddit · r/MachineLearning · /u/Substantial_Diver469 · Jun 17, 18:31

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks by identifying circuits—subnetworks responsible for specific behaviors. Supervised fine-tuning (SFT) adapts a pretrained model on labeled data. Contrastive SFT uses pairs of examples to emphasize differences. Causal dependency graphs map how changes in one part of the model affect others.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2404.14082">arXiv:2404.14082v3 [cs.AI] 23 Aug 2024 Mechanistic</a></li>
<li><a href="https://www.emergentmind.com/papers/2605.11426">Mechanistic Analysis of SFT-Induced Drift</a></li>
<li><a href="https://transformer-circuits.pub/2025/attribution-graphs/methods.html">Circuit Tracing: Revealing Computational Graphs in Language Models</a></li>

</ul>
</details>

**Discussion**: The community discussion is substantive, with the author asking for methodological advice on distinguishing direct from indirect effects in ablation studies and on combining activation steering with fine-tuning diagnostics. No comments are provided in the input, so the summary is based on the post's questions.

**Tags**: `#mechanistic interpretability`, `#SFT`, `#causal inference`, `#LLM capabilities`, `#circuit discovery`

---

<a id="item-13"></a>
## [Leakage-Clean Verifier for Robot Manipulation](https://www.reddit.com/r/MachineLearning/comments/1u7hxem/i_built_a_leakageclean_verifier_for_robot/) ⭐️ 8.0/10

A researcher built a leakage-clean verifier that uses object-centric graphs to independently verify robot task completion, preventing the policy author's success metrics from leaking into evaluation. This addresses a critical conflict of interest in robot manipulation evaluation, where policy authors define both behavior and success metrics, potentially enabling more reliable and scalable reward signals for training foundation models. The verifier compiles a human demonstration into an object-centric graph (relations, contacts, event order), then independently extracts a graph from the robot rollout and checks for a match; a no-op baseline fails with named failure classes while a scripted arm passes.

reddit · r/MachineLearning · /u/Alexpplay · Jun 16, 16:10

**Background**: In robot manipulation, success metrics are often hand-coded predicates written by the same person training the policy, creating a conflict of interest. Object-centric graphs represent the state of objects and their relations, enabling symbolic reasoning about task completion. Current evaluation methods struggle with scalability and honesty, especially for training large vision-language-action models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/object-centric-task-and-motion-planning">Object - Centric Task & Motion Planning</a></li>
<li><a href="https://hal.science/hal-05062028v1/document">Is an object - centric representation beneficial for robotic manipulation?</a></li>
<li><a href="https://www.uml.edu/news/stories/2024/compare-robot-manipulation.aspx">Funded by $1.5M NSF Grant, Researchers Look to Advance Robot ...</a></li>

</ul>
</details>

**Discussion**: The community discussion is substantive, with diverse viewpoints on whether this is a real problem or a non-problem. Some argue that task-specific success checks are sufficient in practice, while others see the need for a general verifier. Concerns are raised about the difficulty of perception (video-to-graph under occlusion) and the representation's limitations for deformable or force-profile tasks.

**Tags**: `#robot manipulation`, `#benchmarking`, `#evaluation`, `#object-centric`, `#ML`

---

<a id="item-14"></a>
## [Midjourney Pivots to Medical Imaging, Experts Skeptical](https://www.midjourney.com/medical/blogpost) ⭐️ 7.0/10

Midjourney announced a pivot into medical imaging with a concept video, but provided no technical details or validation data. If successful, this could reduce radiation exposure from CT scans and lower costs, but the lack of substantiation raises doubts about feasibility. The announcement includes only a render of a hypothetical device; no peer-reviewed studies or technical specifications were released.

hackernews · ricochet11 · Jun 18, 01:59 · [Discussion](https://news.ycombinator.com/item?id=48579650)

**Background**: AI has been increasingly used in medical imaging to improve diagnostic accuracy and efficiency, with deep learning models aiding in tumor detection and other tasks. However, regulatory approval and clinical validation are critical hurdles. Midjourney is known for its text-to-image generative AI, but medical imaging requires rigorous testing and domain expertise.

<details><summary>References</summary>
<ul>
<li><a href="https://healthcare.boardofinnovation.com/midjourney/">Midjourney - Generative AI tools for Healthcare providers</a></li>
<li><a href="https://www.ghostmedical.com/news/is-midjourney-ai-smart-enough-to-make-medical-art">"Is Midjourney AI Smart enough to make Medical Art?"</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC10740686/">How Artificial Intelligence Is Shaping Medical Imaging Technology: A Survey of Innovations and Applications - PMC</a></li>

</ul>
</details>

**Discussion**: Comments from doctors and engineers express skepticism, noting the example images look poor and the video lacks substance. Some see potential in reducing CT radiation but demand more details.

**Tags**: `#AI`, `#medical imaging`, `#Midjourney`, `#healthcare`, `#deep learning`

---

<a id="item-15"></a>
## [Adam (YC W25) Launches Open-Source AI CAD Platform](https://github.com/Adam-CAD/CADAM) ⭐️ 7.0/10

Adam (YC W25) launched CADAM, an open-source AI platform that generates parametric 3D CAD models from text prompts or image references, outputting OpenSCAD code with interactive sliders for dimension tweaking. This represents a novel code-based paradigm for CAD generation, potentially lowering the barrier for mechanical design by allowing natural language input. As a YC-backed open-source project, it could accelerate adoption of AI in engineering workflows. CADAM uses a model-agnostic backend via the Vercel AI SDK, supporting Claude, Gemini, and OpenAI models, with Gemini 3.1 Pro performing best in evaluations. It compiles OpenSCAD to WebAssembly for in-browser rendering and supports BOSL, BOSL2, and MCAD libraries.

hackernews · zachdive · Jun 17, 16:14 · [Discussion](https://news.ycombinator.com/item?id=48572553)

**Background**: Traditional CAD software like Fusion 360 requires manual modeling, which can be time-consuming. Code-based CAD tools such as OpenSCAD allow parametric designs but require programming knowledge. AI text-to-CAD tools aim to combine the flexibility of code with the ease of natural language.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tinkercad.com/users/07Lo2eg3KjZ-ai">.A.I. - Tinkercad</a></li>
<li><a href="https://zoo.dev/zookeeper">ML CAD Model Generator | Create CAD Files With Text | Zoo</a></li>

</ul>
</details>

**Discussion**: Some engineers expressed skepticism, arguing that manual modeling is faster and more reliable for precise mechanical parts. However, others praised the parametric slider feature and noted that the tool handled complex prompts well, suggesting potential for rapid prototyping.

**Tags**: `#AI`, `#CAD`, `#open-source`, `#YC`, `#mechanical-design`

---

<a id="item-16"></a>
## [Volkswagen blocks GrapheneOS users via API lock](https://discuss.grapheneos.org/d/35949-volkswagen-app?page=3) ⭐️ 7.0/10

Volkswagen has locked its automotive API to only accept requests from Play Protect certified devices, effectively blocking users of GrapheneOS and other custom ROMs from accessing vehicle features via community integrations. This move undermines user choice and privacy by forcing GrapheneOS users to either use Google's proprietary services or lose access to their vehicle's digital features, highlighting a growing conflict between automakers and privacy-focused open-source communities. The API lock affects all community-driven projects like Home Assistant integrations, which many users preferred over Volkswagen's official app due to its heavy advertising and limited features. GrapheneOS is an open-source Android-based OS that can run Google services in a sandbox, but it is not Play Protect certified.

hackernews · microtonal · Jun 17, 15:04 · [Discussion](https://news.ycombinator.com/item?id=48571526)

**Background**: Play Protect certification is Google's program that ensures devices pass compatibility tests and include proprietary Google apps. GrapheneOS prioritizes privacy and security by removing Google services by default, though users can optionally install them sandboxed. Volkswagen's API previously allowed third-party integrations for features like preheating the car, which are now blocked for non-certified devices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://support.google.com/googleplay/answer/7165974?hl=en">Check & fix Play Protect certification status - Google Play Help</a></li>
<li><a href="https://grapheneos.org/">GrapheneOS: the private and secure mobile OS</a></li>

</ul>
</details>

**Discussion**: Community members expressed frustration, with one user delaying a car purchase due to the API change and another criticizing Volkswagen's app as 60% ads and 30% features. Some linked the move to broader EU mandates for intrusive driving aids, while others speculated about future implications for GrapheneOS if VPNs are banned.

**Tags**: `#GrapheneOS`, `#Volkswagen`, `#API`, `#privacy`, `#automotive`

---

<a id="item-17"></a>
## [Datasette 1.0a34 Adds CRUD UI for Rows](https://simonwillison.net/2026/Jun/16/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a34 introduces insert, edit, and delete row capabilities directly in the user interface, available on table pages and row pages. This feature was inspired by the SQL write support recently added to Datasette Agent. This release brings long-awaited CRUD (Create, Read, Update, Delete) functionality to Datasette, making it a more complete data management tool. Users can now perform basic data operations without needing to write SQL queries, lowering the barrier for non-technical users. The insert, edit, and delete tools are available on table pages, while edit and delete are also accessible as action items on the row page. The feature is permission-gated, meaning only users with the necessary permissions can perform these operations.

rss · Simon Willison · Jun 16, 21:31

**Background**: Datasette is an open-source tool for exploring and publishing data, primarily used with SQLite databases. Previously, Datasette only supported read-only operations in its UI; write operations required using the SQL API or external tools. Datasette Agent is an AI assistant that can generate and execute SQL queries, including write queries, which highlighted the gap in the main Datasette interface.

<details><summary>References</summary>
<ul>
<li><a href="https://agent.datasette.io/">Datasette Agent : an AI assistant for Datasette to help explore and...</a></li>
<li><a href="https://simonwillison.net/2026/Jun/15/datasette-agent/">Release: datasette-agent 0.3a0 - simonwillison.net</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#release`, `#database`, `#CRUD`, `#open source`

---

<a id="item-18"></a>
## [Georgi Gerganov Endorses Qwen3.6-27B for Local Coding](https://simonwillison.net/2026/Jun/16/georgi-gerganov/#atom-everything) ⭐️ 7.0/10

Georgi Gerganov, creator of llama.cpp, publicly endorsed Qwen3.6-27B as a highly capable local model for coding tasks, stating he uses it daily on his M2 Ultra or RTX 5090. He shared his lightweight setup using the pi agent with a custom system prompt. This endorsement from a key figure in local LLM development validates Qwen3.6-27B's practical utility for coding, potentially encouraging wider adoption of local AI coding assistants. It highlights the growing viability of running capable models on consumer hardware. Gerganov uses the pi agent with the `-nc --offline` flags and a short system prompt from the llama.cpp repository to align the model with his coding style. He noted that he would use it more if not for time spent on PR reviews.

rss · Simon Willison · Jun 16, 16:04

**Background**: Qwen3.6-27B is a dense 27-billion-parameter multimodal model open-sourced by Alibaba's Qwen team, optimized for coding and tool calling. The pi agent is a minimal, MIT-licensed terminal coding agent that works with local models via Ollama or LM Studio. llama.cpp is the foundational inference engine for running LLMs locally on various hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-27B">Qwen/Qwen3.6-27B · Hugging Face</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp">GitHub - ggml - org / llama . cpp : LLM inference in C/C++ · GitHub</a></li>
<li><a href="https://insiderllm.com/guides/pi-agent-local-models-ollama/">Best Local Models for PI Agent: Qwen 3.6, Gemma 4 (2026 Setup)</a></li>

</ul>
</details>

**Discussion**: The Hacker News comment from Gerganov received positive attention, with users noting the credibility of his endorsement given his role in local LLM development. The discussion reinforced the trend of local coding agents becoming practical for everyday tasks.

**Tags**: `#local LLM`, `#coding assistant`, `#Qwen`, `#llama.cpp`, `#AI tools`

---

<a id="item-19"></a>
## [Anthropic's Fable jailbreak: expected cyberdefense behavior](https://simonwillison.net/2026/Jun/16/matteo-wong-the-atlantic/#atom-everything) ⭐️ 7.0/10

Cybersecurity expert Katie Moussouris reviewed a White House report on the Fable jailbreak and concluded that Claude Fable's refusal to review insecure code but compliance with 'fix this code' was the model working as intended for cyberdefense. This expert assessment reframes the Fable jailbreak from a safety failure to a demonstration of proper AI cyberdefense behavior, influencing how policymakers and developers view AI safety incidents. The Fable jailbreak involved IT experts asking the model to find and patch bugs; the model refused to 'review the code for security issues' but complied when asked to 'fix this code' with manual steps, which Moussouris said was expected for cyberdefense.

rss · Simon Willison · Jun 16, 03:07

**Background**: AI jailbreaks are techniques to trick models into bypassing safety training. The Fable model is Anthropic's most capable coding model, but its access was suspended shortly after launch due to safety concerns. The White House report investigated the Fable jailbreak as part of broader AI safety and export control discussions.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/0xSufi/fable-jailbreak/">GitHub - 0xSufi/ fable - jailbreak : Anthropic's Fable jailbreak for Claude...</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#jailbreak`, `#Anthropic`, `#cybersecurity`

---

<a id="item-20"></a>
## [Can foundational AI research be done without HPC?](https://www.reddit.com/r/MachineLearning/comments/1u8jyat/is_foundational_ai_research_still_something_that/) ⭐️ 7.0/10

A Reddit user asks whether foundational AI research is still possible without access to high-performance computing (HPC), noting that the seminal 'Attention is all you need' paper was trained on just eight GPUs. This question highlights a growing barrier to entry in AI research, where large-scale models increasingly require massive compute, potentially excluding individual researchers or small labs from making foundational contributions. The original Transformer paper used 8 GPUs for 3.5 days, costing a fraction of modern training runs. Today, state-of-the-art models often require thousands of GPUs or TPUs, making HPC access critical for reproducing or advancing such work.

reddit · r/MachineLearning · /u/Proof-Bed-6928 · Jun 17, 19:26

**Background**: Foundational AI research refers to work that introduces new architectures, algorithms, or theoretical insights, rather than incremental improvements. High-performance computing (HPC) encompasses supercomputers and large clusters of GPUs/TPUs used for training large models. The Transformer architecture, introduced in 2017, revolutionized natural language processing and remains the basis for models like GPT-4.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/1706.03762">[1706.03762] Attention Is All You Need - arXiv.org Attention is All You Need - Google Research Attention is All You Need - Google Search Attention Is All You Need — Full Paper Breakdown Paper page - Attention Is All You Need - Hugging Face</a></li>

</ul>
</details>

**Discussion**: The Reddit thread likely contains diverse opinions, with some arguing that algorithmic innovations can still come from small-scale experiments, while others contend that the field's trajectory demands HPC for meaningful contributions. No specific comments are provided.

**Tags**: `#AI research`, `#HPC`, `#foundational models`, `#machine learning`, `#hardware requirements`

---

<a id="item-21"></a>
## [Probe Strength Analysis in Mechanistic Interpretability](https://www.reddit.com/r/MachineLearning/comments/1u8lo60/how_do_you_analyze_the_relative_strength_of/) ⭐️ 7.0/10

A researcher raises a nuanced question about balancing probe capacity and network complexity in mechanistic interpretability, specifically seeking theoretical grounding for provable guarantees and sampling theory akin to the Nyquist-Shannon theorem. This question highlights a critical gap in mechanistic interpretability research: the lack of rigorous theory to determine whether a probe's findings reflect genuine model knowledge or artifacts of probe capacity, which is essential for reliable circuit analysis and factuality guarantees. The post references a specific example of probing whether a transformer knows which word a token belongs to, and notes that even simple probes can yield misleading results due to small vocabulary size or spurious correlations. The author also mentions a real-world failure of Gemini in counting letters, suggesting limitations in token decomposition.

reddit · r/MachineLearning · /u/RepresentativeBee600 · Jun 17, 20:29

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks into human-understandable algorithms, often using probes (simple classifiers) to detect internal representations. However, the field lacks formal guarantees about probe reliability, and questions about overfitting, sample complexity, and capacity trade-offs remain open.

<details><summary>References</summary>
<ul>
<li><a href="https://www.neelnanda.io/mechanistic-interpretability/glossary">A Comprehensive Mechanistic Interpretability ... — Neel Nanda</a></li>
<li><a href="https://leonardbereska.github.io/blog/2024/mechinterpreview/">Mechanistic Interpretability for AI Safety — A Review</a></li>

</ul>
</details>

**Tags**: `#mechanistic interpretability`, `#probing`, `#circuit analysis`, `#machine learning theory`, `#transformers`

---

<a id="item-22"></a>
## [8-bit Live Baseball Gamecast from MLB Data](https://ribbie.tv/watch) ⭐️ 6.0/10

A developer launched ribbie.tv, a website that converts live MLB data streams into near real-time 8-bit pixel art gamecasts, complete with stadiums, day/night modes, and between-inning graphics. This project offers a novel, nostalgic way to follow baseball games, potentially appealing to fans who enjoy retro aesthetics or want a data-driven, low-bandwidth alternative to video broadcasts. The site uses live MLB data feeds to animate pixel art representations of players and game events, but some community members noted that the pixel art appears AI-generated rather than hand-crafted, which may reduce authenticity.

hackernews · brownrout · Jun 17, 16:44 · [Discussion](https://news.ycombinator.com/item?id=48573012)

**Background**: MLB provides official data streams that include play-by-play events, player positions, and scores, which third-party developers can access via APIs. Pixel art gamecasts are a type of visualization that recreates the game in a retro 8-bit style, similar to classic video games.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48573012">Show HN: An 8-bit live gamecast for baseball | Hacker News</a></li>
<li><a href="https://hn.nuxt.dev/item/48573012">Nuxt HN | Show HN: An 8-bit live gamecast for baseball</a></li>
<li><a href="https://ideaverse.ai/blog/show-hn-8-bit-live-baseball-gamecasts-from-mlb-streaming-data-mqif7eci">Show HN: 8-bit live baseball gamecasts from MLB streaming ...</a></li>

</ul>
</details>

**Discussion**: Commenters generally praised the creativity but offered constructive criticism: some suggested using a real pixel font and deterministic downsampling instead of AI art, while others requested features like a play-by-play log, clickable inning tabs, and sound effects for key events.

**Tags**: `#baseball`, `#visualization`, `#pixel art`, `#data streaming`, `#web development`

---

<a id="item-23"></a>
## [Why Talking Through Problems Beats Thinking Alone](https://www.thesignalist.io/s/the-dialogue-dividend/) ⭐️ 6.0/10

An article on The Signalist argues that articulating thoughts to another person improves clarity and problem-solving, drawing parallels to rubber duck debugging in software engineering. 这一概念强化了协作思考和口头表达在技术与非技术领域中的价值，可能改善团队处理复杂问题的方式。 The article highlights that the act of forming vague impressions into structured sentences forces deeper understanding, similar to how writing improves thinking. The technique is widely known but often underutilized.

hackernews · kodesko · Jun 17, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48569894)

**Background**: Rubber duck debugging is a common practice where programmers explain code line by line to an inanimate object (like a rubber duck) to find errors. The underlying principle is that verbalizing forces explicit reasoning, revealing gaps in understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rubber_duck_debugging">Rubber duck debugging</a></li>
<li><a href="https://rubberduckdebugging.com/">Rubber Duck Debugging – Rubber Duck Debugging – Debugging ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with the premise, with some noting that the key is the act of structuring thoughts rather than the presence of a listener. One commenter shared a personal anecdote about using doodles as a similar technique, while another pointed out cultural differences in thinking styles.

**Tags**: `#cognition`, `#communication`, `#problem-solving`, `#rubber-duck-debugging`

---

<a id="item-24"></a>
## [Robot Sprint Game Compares Claude, Grok, and DeepSeek](https://openrouter.ai/blog/insights/royale-last-agent-standing/) ⭐️ 6.0/10

A blog post on OpenRouter describes a game where a robot sprints toward the player, and compares how different AI models (Claude, Grok, DeepSeek V4 Flash) control the robot, with DeepSeek V4 Flash winning on cost efficiency. This comparison highlights the trade-offs between model performance and cost in a novel, real-time task, offering insights for developers choosing AI models for interactive applications. The experiment ran 30 games per model, costing $482 total; frontier models like Opus 4.7 or GPT-5.5 would have cost around $3,000. DeepSeek V4 Flash, a Mixture-of-Experts model with 284B total parameters and 13B activated, proved highly cost-effective.

hackernews · Usu · Jun 17, 21:00 · [Discussion](https://news.ycombinator.com/item?id=48576824)

**Background**: Large language models (LLMs) like Claude, Grok, and DeepSeek are typically benchmarked on coding or reasoning tasks, but this game tests them in a dynamic, real-time environment. The blog uses a custom game to evaluate how well each model handles a simple but reactive scenario, emphasizing cost as a key factor.

<details><summary>References</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/news/news260424">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>
<li><a href="https://news.ycombinator.com/item?id=48576824">A robot is sprinting towards you. Do you want it running on Claude or...</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Grok is more likely to bring a taco without export restrictions, and that DeepSeek V4 Flash's cost efficiency is unsurprising given its coding prowess. One user criticized the silent rerouting of grok-4.1-fast to 4.3 with higher pricing as bad practice.

**Tags**: `#AI`, `#LLM`, `#benchmarking`, `#cost analysis`

---

<a id="item-25"></a>
## [Click-to-Play Web Component Defers GIF Loading](https://simonwillison.net/2026/Jun/17/click-to-play-component/#atom-everything) ⭐️ 6.0/10

Simon Willison introduced a progressive enhancement web component called <click-to-play> that defers loading GIFs until the user clicks a play button, improving page performance. This component helps reduce initial page load times and bandwidth usage by avoiding automatic loading of large GIFs, which is especially beneficial for content-heavy sites and users on slow connections. The component uses standard HTML markup with a fallback <a> and <img> tag, ensuring content is accessible even without JavaScript. It was built for a Datasette blog post demonstrating new row editing tools.

rss · Simon Willison · Jun 17, 03:56

**Background**: Progressive enhancement is a web development strategy that ensures basic content and functionality are available to all users, while advanced features are layered on for browsers that support them. Web Components are reusable custom HTML elements that encapsulate functionality. Lazy-loading GIFs on demand can significantly improve Core Web Vitals like Largest Contentful Paint (LCP).

<details><summary>References</summary>
<ul>
<li><a href="https://griffadev.medium.com/using-web-components-with-11ty-6187427fc3fb">Using Web Components With 11ty. I took a progressive enhancement</a></li>
<li><a href="https://www.30secondsofcode.org/js/s/progressive-enhancement-web-components/">JavaScript - Progressive enhancement with Web Components</a></li>
<li><a href="https://codepen.io/jjmartucci/pen/ExNQVdZ">Progressive enhancement with Web Components</a></li>

</ul>
</details>

**Tags**: `#web components`, `#javascript`, `#performance`, `#progressive enhancement`

---

<a id="item-26"></a>
## [Datasette-Tailscale Plugin Exposes Local DB Securely](https://simonwillison.net/2026/Jun/16/datasette-tailscale/#atom-everything) ⭐️ 6.0/10

The experimental alpha plugin datasette-tailscale 0.1a0 allows users to run a Datasette instance on localhost and expose it to a Tailscale tailnet via a single command, using Tailscale's sidecar and Python bindings for tailscale-rs. This plugin simplifies secure sharing of local Datasette databases over a Tailscale mesh VPN, making it easier for teams to collaborate on data without exposing it to the public internet. It demonstrates a practical integration of Tailscale's networking capabilities with data exploration tools. The plugin uses the ts_python crate from tailscale-rs to connect to a tailnet and bind network sockets. It requires a Tailscale auth key and hostname, and currently relies on an experimental proxy mechanism that the author has filed an issue about for improvement.

rss · Simon Willison · Jun 16, 16:18

**Background**: Datasette is an open-source tool for exploring and publishing SQLite databases. Tailscale provides a zero-config VPN that creates a secure mesh network called a tailnet. The tailscale-rs library offers Rust-based bindings for Python, enabling applications to interact with a tailnet programmatically.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/docs/concepts/tailnet">What is a tailnet? - Tailscale Docs</a></li>
<li><a href="https://github.com/tailscale/tailscale-rs/tree/main/ts_python">tailscale-rs/ts_python at main - GitHub</a></li>
<li><a href="https://deepwiki.com/tailscale/tailscale-rs/6.1-python-bindings-(ts_python)">Python Bindings (ts_python) | tailscale/tailscale-rs | DeepWiki</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#tailscale`, `#plugin`, `#networking`, `#alpha`

---

<a id="item-27"></a>
## [Open-Source ML Pipeline for Hong Kong Horse Racing](https://www.reddit.com/r/MachineLearning/comments/1u8twkz/opensource_hong_kong_horse_racing_ml_pipeline/) ⭐️ 6.0/10

A developer released an open-source ML pipeline for Hong Kong horse racing prediction using LightGBM and XGBoost, including feature engineering, ensemble models, and betting simulations with Kelly criterion. This project provides a reproducible benchmark for sports betting ML research, and its finding that a no-odds model outperforms for quinella ROI challenges common assumptions about incorporating public odds. The pipeline includes unit tests for betting math and database schema, and the dashboard shows out-of-sample validation results. The no-odds model's superior quinella ROI suggests public odds already price favorites efficiently.

reddit · r/MachineLearning · /u/Marshallmatta · Jun 18, 02:21

**Background**: Quinella is a bet where you pick two horses to finish in the top two in any order. The Kelly criterion is a formula for optimal bet sizing to maximize long-term growth. The Hong Kong Jockey Club (HKJC) is the sole legal horse racing operator in Hong Kong.

<details><summary>References</summary>
<ul>
<li><a href="https://www.americasbookie.com/what-is-a-quinella/">What is a Quinella Bet ? - America’s Bookie | CBS Sports Picks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kelly_criterion">Kelly criterion - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hong_Kong_Jockey_Club">Hong Kong Jockey Club - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#open source`, `#sports betting`, `#feature engineering`, `#pipeline`

---

<a id="item-28"></a>
## [ECCV 2026 Final Decisions Expected June 17](https://www.reddit.com/r/MachineLearning/comments/1u7gouq/eccv_2026_final_decisions_d/) ⭐️ 6.0/10

ECCV 2026 final decisions are expected to be released on June 17, 2026, with results likely rolling out within 48 hours. A Reddit thread has been created for the community to share updates and discuss outcomes. This announcement marks a key milestone for researchers and practitioners submitting to ECCV, one of the top conferences in computer vision. The outcome will influence future research directions and career opportunities for many in the field. No exact release time was specified, so results may appear throughout June 17-18. The conference itself will take place from September 8-12, 2026 in Malmö, Sweden.

reddit · r/MachineLearning · /u/mclovingho · Jun 16, 15:25

**Background**: ECCV (European Conference on Computer Vision) is a biennial conference considered one of the top venues in computer vision, alongside CVPR and ICCV. The final decision phase follows a review and rebuttal process, where authors respond to reviewer comments before acceptance decisions are made.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/European_Conference_on_Computer_Vision">European Conference on Computer Vision - Wikipedia</a></li>
<li><a href="https://eccv.ecva.net/Conferences/2026/Dates">2026 Dates and Deadlines</a></li>
<li><a href="https://huggingface.co/spaces/huggingface/ai-deadlines/commit/3bccf2b883c17d4536b469411fa413dc8711fdbb">Update ECCV 2026 with complete deadline information...</a></li>

</ul>
</details>

**Discussion**: The Reddit thread is primarily a place for sharing updates and offering mutual support; no specific comments or sentiment analysis are available from the provided content.

**Tags**: `#ECCV`, `#conference`, `#machine learning`, `#community`

---

<a id="item-29"></a>
## [GAN on Raspberry Pi 4 Powers Physical NFT Minting Device](https://www.reddit.com/r/MachineLearning/comments/1u8cqan/i_deployed_a_gan_on_a_raspberry_pi_4_and_built_a/) ⭐️ 6.0/10

A hobbyist trained a 128×128 DCGAN on a MacBook M3, deployed it on a Raspberry Pi 4, and built a physical device that generates hybrid face images and prints them as physical NFTs at the press of a button. This project demonstrates that running GAN inference on low-cost edge hardware like a Raspberry Pi 4 is feasible, opening up possibilities for interactive art installations and decentralized NFT minting without cloud dependencies. The DCGAN uses a 6-block generator and discriminator, trained for 800 epochs on 2480 images (11 subjects) with one dominant anchor class to produce hybrids. Inference takes 3 seconds per face on the Pi 4, and the model was exported from PyTorch to ONNX (float32, 53MB).

reddit · r/MachineLearning · /u/Numerous-Dentist-882 · Jun 17, 15:05

**Background**: DCGAN (Deep Convolutional Generative Adversarial Network) is a class of GAN that uses convolutional layers for image generation. ONNX (Open Neural Network Exchange) is an open format for model interoperability. The LILYGO TTGO T-Display ESP32 is a microcontroller board with an integrated display, used here to show the generated face and title.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html">DCGAN Tutorial — PyTorch Tutorials 2.12.0+cu130 documentation</a></li>
<li><a href="https://docs.pytorch.org/tutorials/beginner/onnx/export_simple_model_to_onnx_tutorial.html">Export a PyTorch model to ONNX</a></li>
<li><a href="https://lilygo.cc/products/t-display">T - Display – LILYGO</a></li>

</ul>
</details>

**Tags**: `#GAN`, `#Edge AI`, `#Raspberry Pi`, `#NFT`, `#DIY`

---