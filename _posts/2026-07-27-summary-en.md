---
layout: default
title: "Horizon Summary: 2026-07-27 (EN)"
date: 2026-07-27
lang: en
---

> From 30 items, 13 important content pieces were selected

---

1. [US citizen charged after GrapheneOS phone wipes at border](#item-1) ⭐️ 8.0/10
2. [The relay market powering token resellers and fraud](#item-2) ⭐️ 8.0/10
3. [Ruff v0.16.0 Expands Default Rules from 59 to 413](#item-3) ⭐️ 8.0/10
4. [YOLO26n Inference from Scratch in ARM64 Assembly](#item-4) ⭐️ 8.0/10
5. [4B Open-Weight Models Match o3 on Swedish Medical QA](#item-5) ⭐️ 8.0/10
6. [LLMs Compared on IMO 2026 Problems](#item-6) ⭐️ 8.0/10
7. [PGSimCity: Interactive 3D Visualization of PostgreSQL Internals](#item-7) ⭐️ 7.0/10
8. [Decker Revives HyperCard with 1-Bit Retro Aesthetic](#item-8) ⭐️ 7.0/10
9. [Data-Oriented Design: A Performance Paradigm](#item-9) ⭐️ 7.0/10
10. [French Firefighters Face Pyrocumulonimbus Cloud for First Time](#item-10) ⭐️ 6.0/10
11. [Design is compromise](#item-11) ⭐️ 6.0/10
12. [Multi-Tenant RAG Architecture Advice Sought](#item-12) ⭐️ 6.0/10
13. [Theoretical ML papers face unfair review due to length limits](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [US citizen charged after GrapheneOS phone wipes at border](https://www.techspot.com/news/113236-us-prosecutors-charge-atlanta-man-after-grapheneos-phone.html) ⭐️ 8.0/10

A US citizen, identified as Tunick, was charged after his GrapheneOS phone automatically wiped during a border search by US Customs and Border Protection, allegedly due to entering a duress PIN. This case sets a precedent for legal consequences of using duress PINs at US borders, potentially chilling privacy-conscious travelers and testing the limits of digital security practices against government searches. The phone ran GrapheneOS, an open-source OS for Pixel devices that allows a duress PIN to trigger a factory reset. The prosecution argues the wipe was intentional obstruction, not an automatic feature.

hackernews · eecc · Jul 26, 22:21 · [Discussion](https://news.ycombinator.com/item?id=49063022)

**Background**: GrapheneOS is a security-focused Android-based OS that includes features like duress PINs, which wipe the device when entered under coercion. US border agents have broad authority to search electronic devices, but the legality of using such countermeasures is contested. The case highlights tension between privacy rights and border security.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techspot.com/news/113236-us-prosecutors-charge-atlanta-man-after-grapheneos-phone.html">US prosecutors charge Atlanta man after GrapheneOS phone ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Duress_PIN">Duress PIN</a></li>

</ul>
</details>

**Discussion**: Commenters debated the legal intent vs. technical action, with some arguing that using a duress PIN is akin to obstruction, while others suggested better practices like carrying a blank phone. The discussion also referenced VeraCrypt's hidden volume feature as a potential alternative.

**Tags**: `#privacy`, `#security`, `#legal`, `#GrapheneOS`, `#border search`

---

<a id="item-2"></a>
## [The relay market powering token resellers and fraud](https://vectoral.com/blog/token-relay-market) ⭐️ 8.0/10

A Vectoral blog post exposes a hidden relay market where token resellers exploit billing system loopholes, stolen accounts, and free cloud credits to resell AI API tokens at heavily discounted prices, enabling fraud and unfair competition. This practice undermines legitimate AI API pricing, distorts the market, and forces honest companies to compete with fraudsters who can offer tokens at 4% of the actual cost, threatening the sustainability of the AI ecosystem. The resale market mirrors earlier abuses in digital advertising, using stolen financial instruments, account takeovers, and free credit abuse. The article notes that fraud is a constant cat-and-mouse game with no clean fix.

hackernews · mlenhard · Jul 26, 15:17 · [Discussion](https://news.ycombinator.com/item?id=49058993)

**Background**: AI API tokens are units of computation used to access models like GPT-4. Cloud providers offer free credits to attract new customers, but these credits can be abused by resellers who create shell companies to obtain them and then resell the tokens at a discount.

<details><summary>References</summary>
<ul>
<li><a href="https://vectoral.com/blog/token-relay-market">An Inside Look at the Relay Market Powering Token Resellers and Fraud | Vectoral</a></li>
<li><a href="https://jinlow.substack.com/p/ai-token-resellers-are-selling-you">AI Token Resellers Are Selling You Fake Models - by Jin</a></li>
<li><a href="https://discuss.ai.google.dev/t/solved-how-to-stop-gemini-api-card-charges-and-use-your-300-google-cloud-credits-instead/142406">[SOLVED] How to stop Gemini API card charges and use your $300 Google Cloud Credits instead - Google AI Studio - Google AI Developers Forum</a></li>

</ul>
</details>

**Discussion**: Commenters note that this is not new, drawing parallels to ad fraud and ticket touting. Some highlight the abuse of free cloud credits as a key enabler, while others point to subscription model flaws as the root cause.

**Tags**: `#AI`, `#fraud`, `#token economy`, `#cloud credits`, `#subscription models`

---

<a id="item-3"></a>
## [Ruff v0.16.0 Expands Default Rules from 59 to 413](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0, released on July 23, 2026, dramatically expands its default rule set from 59 to 413 rules, catching more severe issues like syntax errors and runtime errors without any configuration. This change will cause CI failures for projects with unpinned Ruff dependencies, forcing developers to either pin their version or fix hundreds of new linting issues. It significantly raises the baseline code quality for Python projects using Ruff. The number of rules in Ruff grew from 708 to 968 since v0.1.0, and many previously disabled rules are now enabled by default. The new defaults include rules like DTZ005 (datetime without timezone), BLE001 (blind exception catch), and B018 (useless attribute access).

rss · Simon Willison · Jul 25, 22:44

**Background**: Ruff is an extremely fast Python linter written in Rust, designed to replace tools like Flake8 and pylint. It has gained widespread adoption due to its speed and comprehensive rule set. Astral, the company behind Ruff, was recently acquired by OpenAI.

<details><summary>References</summary>
<ul>
<li><a href="https://astral.sh/blog/ruff-v0.16.0">Ruff v0.16.0 - astral.sh</a></li>
<li><a href="https://byteiota.com/ruff-v0-16-default-rules/">Ruff v0.16.0: 413 Default Rules Break Unpinned Python ...</a></li>
<li><a href="https://rushcommerce.dev/blog/ruff-0-16-413-default-rules-your-python-ci-just-got-loud">Ruff 0.16 ships 413 default rules — pin before you upgrade</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights that many developers experienced CI breakage due to unpinned dependencies, with some praising the expanded defaults for catching real issues. Others noted the importance of pinning Ruff versions to avoid unexpected failures.

**Tags**: `#Python`, `#linting`, `#Ruff`, `#tooling`, `#release`

---

<a id="item-4"></a>
## [YOLO26n Inference from Scratch in ARM64 Assembly](https://www.reddit.com/r/MachineLearning/comments/1v6w394/i_implemented_the_yolo26n_model_inference_from/) ⭐️ 8.0/10

A bachelor's project implements YOLO26n inference entirely from scratch using ARM64 assembly and C, without any deep learning framework, on a Raspberry Pi 4. This demonstrates deep low-level understanding of neural network inference and optimization for edge AI, potentially inspiring more efficient implementations on resource-constrained devices. The implementation includes ARM NEON SIMD optimization, Winograd convolution, cache-aware tiling, operator fusion, and custom micro-kernels, but performance gains were modest compared to expectations.

reddit · r/MachineLearning · /u/Forward_Confusion902 · Jul 26, 06:43

**Background**: YOLO (You Only Look Once) is a popular real-time object detection model. ARM64 assembly is used for low-level hardware control, and NEON SIMD enables parallel data processing. Winograd convolution reduces multiplication operations in convolutional layers, and operator fusion combines multiple operations to reduce memory traffic.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2201.10369">[2201.10369] Winograd Convolution for Deep Neural Networks ... Winograd Convolution for Deep Neural Networks: Efficient ... Winograd's Convolution Theorem [Explained] - OpenGenus IQ Chapter 8: Fast Convolution - College of Science and Engineering The Winograd Convolution Method - DiVA Winograd Convolution for Deep Neural Networks: Efficient ... Winograd Convolution: A Perspective from Fault Tolerance</a></li>
<li><a href="https://www.arm.com/technologies/neon">Neon – Arm®</a></li>
<li><a href="https://ai-solutions.daviesmeyer.com/en/glossary/operator-fusion">Operator Fusion Explained: Definition, Examples & Use Cases ...</a></li>

</ul>
</details>

**Tags**: `#YOLO`, `#ARM64`, `#edge AI`, `#neural network optimization`, `#assembly`

---

<a id="item-5"></a>
## [4B Open-Weight Models Match o3 on Swedish Medical QA](https://www.reddit.com/r/MachineLearning/comments/1v71wds/openweight_4b_models_approach_o3level_medical/) ⭐️ 8.0/10

Open-weight 4B models, specifically Qwen3.5-4B with reasoning enabled, achieve 87% accuracy on the Swedish medical licensing exam dataset MedQA-SWE, approaching the 88% score of OpenAI's o3 model. The author also demonstrates that post-training (SFT) on earlier exam years boosts MedGemma-1.5-4B from a low baseline to 60% accuracy. This demonstrates that small, open-weight models can rival proprietary frontier models on specialized, low-resource language tasks, highlighting the potential for accessible, domain-specific AI in healthcare. The findings also provide practical insights into reasoning interventions like early exit to mitigate overthinking. Qwen3.5-4B achieves 87% accuracy with reasoning enabled and no length cap, but some reasoning traces spiral into repetitive loops; an early exit intervention from the S-GRPO paper helps by injecting a phrase to close the thinking trace at a predetermined length. The model performs all reasoning in English despite Swedish prompts, indicating language is not a barrier.

reddit · r/MachineLearning · /u/AccomplishedCat4770 · Jul 26, 11:58

**Background**: MedQA-SWE is a Swedish multiple-choice clinical question-answering dataset with 3,180 questions derived from medical licensing exams. Open-weight LLMs are models whose parameters are publicly released, allowing fine-tuning and customization. The S-GRPO method introduces reinforcement learning to enable early exit in chain-of-thought reasoning, reducing unnecessary computation.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/datasets/nicher92/medqa-swe">nicher92/ medqa - swe · Datasets at Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2505.07686">[2505.07686] S-GRPO: Early Exit via Reinforcement Learning in ... S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models S-GRPO: Early Exit via Reinforcement Learning - arXiv.org Images S-GRPO: Early Exit via Reinforcement Learning in Reasoning ... S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models [PDF] S-GRPO: Early Exit via Reinforcement Learning in ... (PDF) S-GRPO: Early Exit via Reinforcement Learning in ...</a></li>
<li><a href="https://aclanthology.org/2024.lrec-main.975.pdf">MedQA - SWE - a Clinical Question & Answer Dataset for Swedish</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#medical QA`, `#open-weight models`, `#reasoning`, `#SFT`

---

<a id="item-6"></a>
## [LLMs Compared on IMO 2026 Problems](https://www.reddit.com/r/MachineLearning/comments/1v6wskz/we_compared_different_llms_on_imo_2026_r/) ⭐️ 8.0/10

A systematic comparison of LLMs on new IMO 2026 problems shows frontier models achieve near-perfect scores, while the AutoFyn multi-agent harness significantly boosts performance of weaker models like Claude Sonnet and Opus. This benchmark demonstrates that mathematical reasoning remains a key differentiator for frontier models, and that harness engineering can substantially narrow the gap for weaker models, with implications for AI evaluation and agentic systems. Frontier models 'sol' and 'fable' scored perfectly or near-perfectly regardless of harness; AutoFyn improved Sonnet and Opus scores but could not match frontier performance. The hardest problem (P3) was unsolved by all sub-frontier models, even with a 20-hour run.

reddit · r/MachineLearning · /u/pequalnp92 · Jul 26, 07:21

**Background**: The International Mathematical Olympiad (IMO) is a prestigious competition with novel problems not in training data, making it a strong benchmark for reasoning. AutoFyn is a customizable multi-agent harness that orchestrates LLM agents with retrieval and verification to improve performance on complex tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/SignalPilot-Labs/AutoFyn">GitHub - SignalPilot-Labs/AutoFyn: Run Claude in self ...</a></li>
<li><a href="https://benchlm.ai/benchmarks/imo2026">IMO 2026 Leaderboard & Scores — July 2026 | BenchLM.ai</a></li>
<li><a href="https://www.imo-official.org/problems/2026/">IMO 2026 Problems - International Mathematical Olympiad</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion likely includes technical insights on harness design and model performance, with comments from the authors (former IMO medalists) about hallucination issues and the limitations of current harnesses on the hardest problem.

**Tags**: `#LLM`, `#benchmark`, `#mathematical reasoning`, `#multi-agent`, `#AI evaluation`

---

<a id="item-7"></a>
## [PGSimCity: Interactive 3D Visualization of PostgreSQL Internals](https://nikolays.github.io/PGSimCity/) ⭐️ 7.0/10

PGSimCity is an open-source interactive 3D visualization tool that animates PostgreSQL's internal processes, such as query execution and scheduling, in a city-building metaphor. This tool makes complex database internals accessible and engaging, helping developers and students understand PostgreSQL's architecture intuitively. It could inspire similar visualizations for other complex systems. The tool uses a 3D city metaphor where buildings represent processes and roads represent data flow, but some users report z-fighting issues and suggest making the tour interactive rather than automatic.

hackernews · jonbaer · Jul 27, 00:19 · [Discussion](https://news.ycombinator.com/item?id=49063754)

**Background**: PostgreSQL is a powerful open-source relational database with complex internals including a parser, planner, executor, and buffer manager. Understanding these components is crucial for performance tuning and debugging, but traditional documentation is text-heavy. PGSimCity aims to bridge this gap with a visual, exploratory interface.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/NikolayS/pgsimcity">GitHub - NikolayS/PGSimCity: An explorable 3D city that shows ...</a></li>
<li><a href="https://www.postgresql.org/docs/current/internals.html">PostgreSQL: Documentation: 18: Part VII. Internals</a></li>

</ul>
</details>

**Discussion**: The community praised the innovative approach but provided constructive feedback: some users experienced z-fighting when zooming out, others found the automatic tour overwhelming and suggested making it interactive. A user also expressed interest in entering custom queries to see the flow.

**Tags**: `#PostgreSQL`, `#visualization`, `#database internals`, `#interactive learning`

---

<a id="item-8"></a>
## [Decker Revives HyperCard with 1-Bit Retro Aesthetic](https://beyondloom.com/decker/) ⭐️ 7.0/10

Decker is a modern platform that reimagines Apple's classic HyperCard, enabling users to create interactive documents and applications using a visual, card-based interface with a distinctive 1-bit black-and-white aesthetic. By reviving HyperCard's accessible programming paradigm, Decker lowers the barrier for non-programmers to build interactive content, potentially inspiring a new generation of creators and preserving a key piece of computing history. Decker is open source and available on GitHub, featuring a built-in scripting language called DeckerScript. It runs on modern operating systems including Windows, macOS, and Linux, and outputs standalone HTML documents.

hackernews · tosh · Jul 26, 18:23 · [Discussion](https://news.ycombinator.com/item?id=49060856)

**Background**: HyperCard, released by Apple in 1987, was a groundbreaking hypermedia tool that combined a database with a graphical interface and a simple scripting language called HyperTalk. It allowed users to create 'stacks' of cards with text, images, and interactive elements, and was widely used for education, prototyping, and small business applications until its discontinuation in 2004. Decker aims to recapture that spirit by providing a similar authoring environment with a retro 1-bit visual style.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HyperCard">HyperCard</a></li>

</ul>
</details>

**Discussion**: Community comments express strong nostalgia for HyperCard and appreciation for Decker's faithful recreation, but some question its practical utility in 2026, noting that while it's a fun homage, it may not be suitable for real-world projects. Others highlight the historical significance of HyperCard's accessible programming model and hope Decker can introduce it to a new audience.

**Tags**: `#HyperCard`, `#retro computing`, `#visual programming`, `#interactive documents`, `#open source`

---

<a id="item-9"></a>
## [Data-Oriented Design: A Performance Paradigm](https://www.gamedevs.org/uploads/introduction-to-data-oriented-design.pdf) ⭐️ 7.0/10

Mike Acton's classic presentation on data-oriented design (DoD) has been shared, advocating for designing algorithms by first considering data layout to optimize CPU cache usage, especially in game engines. This approach challenges traditional object-oriented design, offering significant performance gains in data-intensive applications like games, where cache misses can bottleneck throughput. DoD focuses on transforming data into contiguous arrays (structure of arrays) to maximize cache locality, contrasting with object-oriented design's scattered memory access patterns.

hackernews · tosh · Jul 26, 18:11 · [Discussion](https://news.ycombinator.com/item?id=49060724)

**Background**: Data-oriented design is a software optimization technique that prioritizes efficient CPU cache usage by organizing data based on how it will be accessed. It is commonly used in high-performance computing and game development, where processing large datasets quickly is critical. Unlike object-oriented design, which groups data and behavior together, DoD separates data into flat structures to enable predictable memory access patterns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data-oriented_design">Data - oriented design - Wikipedia</a></li>
<li><a href="https://stackoverflow.com/questions/1641580/what-is-data-oriented-design">What is data oriented design? - Stack Overflow Code sample</a></li>
<li><a href="https://dataorienteddesign.com/dodbook.pdf">Data - Oriented Design</a></li>

</ul>
</details>

**Discussion**: Commenters generally appreciate DoD's principles but note practical challenges: ghosty141 points out that rapidly changing requirements can undermine DoD's upfront analysis, while PessimalDecimal and inigyou question whether DoD is just cache-aware array programming. dustbunny emphasizes the core idea of putting data first in algorithm design.

**Tags**: `#data-oriented design`, `#performance optimization`, `#game development`, `#software engineering`

---

<a id="item-10"></a>
## [French Firefighters Face Pyrocumulonimbus Cloud for First Time](https://www.france24.com/en/live-news/20260726-french-firefighters-face-pyrocumulonimbus-for-first-time) ⭐️ 6.0/10

French firefighters in the Bordeaux region encountered a pyrocumulonimbus cloud for the first time amid devastating wildfires, marking a new extreme in fire behavior. This event highlights how climate change is intensifying wildfires, creating dangerous fire-generated weather that can spread fires faster and pose new risks to firefighters and communities. Pyrocumulonimbus clouds can reach the upper troposphere, produce lightning, hail, and extreme winds, and inject smoke into the stratosphere, affecting air quality and climate.

hackernews · saaaaaam · Jul 26, 17:49 · [Discussion](https://news.ycombinator.com/item?id=49060495)

**Background**: A pyrocumulonimbus (PyroCb) is a fire-generated thunderstorm cloud that forms when intense heat from a wildfire causes air to rise rapidly, condensing into a cumulonimbus cloud. It is the most extreme form of a flammagenitus cloud and can create its own weather, including fire tornadoes. These clouds were first identified in 1998 and have become more common with increasing wildfire severity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pyrocumulonimbus">Pyrocumulonimbus</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cumulonimbus_flammagenitus">Cumulonimbus flammagenitus - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Flammagenitus_cloud">Flammagenitus cloud - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the Landes and Médoc regions are artificial pine monocultures planted in the 19th century, making them exceptionally flammable. Others shared personal accounts of evacuations and compared the event to similar fire clouds in Washington state and Spain.

**Tags**: `#wildfires`, `#climate change`, `#environment`, `#France`

---

<a id="item-11"></a>
## [Design is compromise](https://stephango.com/design-is-compromise) ⭐️ 6.0/10

An essay argues that compromise is essential in design, sparking community discussion on its nuances and limitations. This perspective challenges the common view that compromise indicates weakness, offering a pragmatic approach to design trade-offs. The essay emphasizes that compromise is not a failure but a necessary tool for balancing constraints, though some commenters argue it should be a last resort.

hackernews · ankitg12 · Jul 26, 15:51 · [Discussion](https://news.ycombinator.com/item?id=49059367)

**Background**: In design and software engineering, trade-offs are inevitable due to limited resources, time, and conflicting requirements. Compromise involves making decisions that satisfy multiple constraints imperfectly but practically.

**Discussion**: Commenters express mixed views: some agree that compromise is a valuable skill, while others argue that it should be avoided by better scoping problems or making strong decisions that alienate some users.

**Tags**: `#design`, `#compromise`, `#software engineering`, `#philosophy`

---

<a id="item-12"></a>
## [Multi-Tenant RAG Architecture Advice Sought](https://www.reddit.com/r/MachineLearning/comments/1v794kw/multitenant_saas_which_architecture_would_you/) ⭐️ 6.0/10

A developer building a SaaS platform in Sri Lanka is seeking advice on choosing between a global RAG with base LLM and a fine-tuned open-source LLM with user-specific RAG for handling sensitive documents. This decision highlights a common trade-off in multi-tenant RAG systems: the cost and complexity of fine-tuning versus the simplicity and scalability of a shared knowledge base with retrieval augmentation. The developer leans toward Option 1 (base LLM + global RAG + user-specific RAG) due to lack of fine-tuning experience and concerns about cost and time, but seeks validation from experienced practitioners.

reddit · r/MachineLearning · /u/Fickle_Degree_2728 · Jul 26, 16:47

**Background**: Multi-tenant RAG architectures serve multiple customers from one system while maintaining strict data isolation. Option 1 uses a curated global knowledge base for domain knowledge and a separate user-specific RAG for private documents, while Option 2 fine-tunes an open-source LLM on domain data and adds user-specific RAG. Fine-tuning can improve accuracy on domain-specific tasks but requires significant data, compute, and expertise.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/azure/architecture/ai-ml/guide/secure-multitenant-rag">Design a secure multitenant RAG inferencing solution</a></li>
<li><a href="https://www.linkedin.com/pulse/building-multi-tenant-rag-architecture-scalable-enterprise-sachin-p-hgqsf">Building Multi-Tenant RAG Architecture for Scalable ...</a></li>
<li><a href="https://www.maviklabs.com/blog/multi-tenant-rag-2026/">Multi-Tenant RAG in 2026: Building Secure Retrieval-Augmented ...</a></li>

</ul>
</details>

**Tags**: `#RAG`, `#multi-tenant`, `#SaaS`, `#LLM`, `#architecture`

---

<a id="item-13"></a>
## [Theoretical ML papers face unfair review due to length limits](https://www.reddit.com/r/MachineLearning/comments/1v6gh43/paper_lengths_and_reasonable_assumptions_in_ml/) ⭐️ 6.0/10

A researcher argues that fixed paper lengths and reviewer expectations at ML conferences like NeurIPS and ICML unfairly penalize theoretical papers, with rejections often citing difficulty rather than lack of impact. This highlights a systemic bias in ML conference reviewing that could discourage theoretical contributions, potentially narrowing the field's intellectual diversity and slowing progress on foundational problems. Conferences allow unlimited appendices but state that reviewers are not expected to read them, creating a tension for theory papers that need extra space for prerequisites. The author notes a shift from earlier rejections based on novelty to recent ones based on perceived difficulty.

reddit · r/MachineLearning · /u/OutsideSimple4854 · Jul 25, 18:48

**Background**: ML conferences like NeurIPS and ICML have long used fixed page limits (e.g., 8 pages) to manage reviewer workload and printing costs, with unlimited appendices for additional details. Theoretical ML papers often require substantial background knowledge and careful exposition, which can be hard to fit within strict length constraints. The review process relies on volunteer reviewers who may lack deep expertise in theory, leading to rejections based on readability rather than scientific merit.

<details><summary>References</summary>
<ul>
<li><a href="https://neurips.cc/">2026 Conference</a></li>
<li><a href="https://github.com/serre-ai/research/blob/main/docs/submission-guides/icml-2025.md">research/docs/submission-guides/ icml -2025.md at main...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion shows mixed sentiment: some agree that theoretical papers are disadvantaged, while others argue that clear writing is a skill authors must develop. A few commenters suggest that reviewers should be more honest about their expertise, and that conferences could adopt separate tracks for theory papers.

**Tags**: `#ML conferences`, `#paper review`, `#theoretical ML`, `#academic publishing`

---