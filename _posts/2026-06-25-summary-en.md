---
layout: default
title: "Horizon Summary: 2026-06-25 (EN)"
date: 2026-06-25
lang: en
---

> From 37 items, 22 important content pieces were selected

---

1. [OpenAI unveils first custom AI chip 'Jalapeno' with Broadcom](#item-1) ⭐️ 9.0/10
2. [Self-play RL agent tops Generals.io leaderboard](#item-2) ⭐️ 9.0/10
3. [Qualcomm Acquires AI Startup Modular for $4B](#item-3) ⭐️ 8.0/10
4. [HDD-RoPE: High-Dimensional Dynamic Rotary Positional Embedding](#item-4) ⭐️ 8.0/10
5. [DeepSWE: New Benchmark Tests Frontier Coding Models](#item-5) ⭐️ 8.0/10
6. [RubyLLM: A Ruby framework for all major AI providers](#item-6) ⭐️ 7.0/10
7. [Google Adds Computer Use to Gemini 3.5 Flash](#item-7) ⭐️ 7.0/10
8. [PR Spam Today Mirrors Early 2000s Email Spam](#item-8) ⭐️ 7.0/10
9. [NVIDIA's 45°C Cooling Cuts Data Center Water Use](#item-9) ⭐️ 7.0/10
10. [GLM-5.2: A Step Change for Open Agents](#item-10) ⭐️ 7.0/10
11. [Elastic Lays Off 7% of Workforce, Cites AI](#item-11) ⭐️ 7.0/10
12. [Nub: A Bun-like All-in-One Toolkit for Node.js](#item-12) ⭐️ 7.0/10
13. [Simon Willison Creates SQLite DB from MDN Browser Compat Data](#item-13) ⭐️ 7.0/10
14. [LLM-Generated Job Apps Obscure Candidate Authenticity](#item-14) ⭐️ 7.0/10
15. [Datasette 1.0a35 Adds Create/Alter Table APIs](#item-15) ⭐️ 7.0/10
16. [Curated Open-Source OCR Models Hub on Papers with Code](#item-16) ⭐️ 7.0/10
17. [MuJoFil: GPU-Native Simulator for Vision RL Training](#item-17) ⭐️ 7.0/10
18. [LLM Inference Pricing Comparison Reveals Surprising Caching Costs](#item-18) ⭐️ 7.0/10
19. [Are ML teams testing model security in production?](#item-19) ⭐️ 7.0/10
20. [uv 0.11.24 Adds CPython 3.15.0b3 and Relocatable Environments](#item-20) ⭐️ 6.0/10
21. [Xteink X4: Tiny Open E-Ink Reader with WiFi Transfer](#item-21) ⭐️ 6.0/10
22. [OPFS + Pyodide Test Harness for Datasette Lite](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI unveils first custom AI chip 'Jalapeno' with Broadcom](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI and Broadcom announced Jalapeno, a custom AI inference chip designed for large language models, manufactured by TSMC and developed in just nine months with AI-assisted design. This marks OpenAI's first foray into custom silicon, potentially reducing reliance on NVIDIA GPUs and improving inference efficiency and cost at scale. It could reshape the AI hardware landscape and intensify competition among hyperscalers. Jalapeno is a reticle-sized ASIC with a tiled architecture, using HBM3/HBM4 memory, and is optimized for LLM inference. OpenAI claims the chip was designed from scratch based on its deep understanding of LLM fundamentals and model roadmap.

hackernews · jamdesk · Jun 24, 17:47 · [Discussion](https://news.ycombinator.com/item?id=48663324)

**Background**: AI inference chips are specialized processors designed to run trained AI models efficiently, as opposed to training chips like NVIDIA's H100. OpenAI previously relied on NVIDIA GPUs and Microsoft's cloud infrastructure; custom chips could offer better performance per watt and lower total cost of ownership. Broadcom is a leading custom chip designer, and TSMC is the world's largest semiconductor foundry.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/broadcom-and-openai-unveil-custom-built-jalapeno-inference-processor-openais-first-chip-is-a-massive-reticle-sized-asic-built-in-an-ultra-fast-nine-month-development-cycle">Broadcom and OpenAI unveil custom-built Jalapeño inference processor — OpenAI's first chip is a massive reticle-sized ASIC built in an ultra-fast nine-month development cycle | Tom's Hardware</a></li>
<li><a href="https://www.nytimes.com/2026/06/24/technology/openai-broadcom-chip-jalapeno.html">OpenAI and Broadcom Unveil Custom A.I. Chip Design</a></li>

</ul>
</details>

**Discussion**: Commenters expressed curiosity about the AI-assisted design claims, with some skeptical that it's more than marketing. Others discussed the chip's architecture, noting the massive die size and potential for huge throughput, while also comparing it to other custom chips like Google's TPU and startups like Taalas.

**Tags**: `#AI hardware`, `#OpenAI`, `#custom chip`, `#inference`, `#semiconductors`

---

<a id="item-2"></a>
## [Self-play RL agent tops Generals.io leaderboard](https://www.reddit.com/r/MachineLearning/comments/1uei2yg/i_made_a_superhuman_generalsio_agent_with/) ⭐️ 9.0/10

A self-play reinforcement learning agent using JAX and Vision Transformer achieved #1 on the human 1v1 leaderboard of Generals.io, surpassing all prior algorithms and human players. The project is fully open-source, including a fast JAX simulator and the agent code. This demonstrates that scaling compute and model capacity (via JAX and ViT) can yield superhuman performance in complex imperfect-information games, without extensive human priors. The open-source release provides a valuable benchmark and toolkit for the RL community. The agent uses a Vision Transformer instead of a CNN, and the entire pipeline was reimplemented in JAX for speed and scalability. The blog details dead ends, decisions, and tricks, serving as a guide for building similar systems.

reddit · r/MachineLearning · /u/shrekofspeed · Jun 24, 16:18

**Background**: Generals.io is a fast-paced multiplayer strategy game with imperfect information, where players command armies to capture territory and defeat opponents. Self-play reinforcement learning trains an agent by playing against itself, gradually improving. JAX is a high-performance numerical computing library that accelerates machine learning on GPUs/TPUs, while Vision Transformer (ViT) adapts transformer architectures for image-like inputs, offering higher capacity than CNNs.

<details><summary>References</summary>
<ul>
<li><a href="https://generals.io/">generals.io</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vision_transformer">Vision transformer</a></li>
<li><a href="https://en.wikipedia.org/wiki/JAX_(software)">JAX (software) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Reddit community praised the work for its technical depth and open-source contribution, with discussions focusing on the scaling approach and the use of ViT over CNNs. Some users asked about training compute and the game's complexity, while others noted the potential for applying similar methods to other games.

**Tags**: `#reinforcement learning`, `#self-play`, `#game AI`, `#JAX`, `#vision transformer`

---

<a id="item-3"></a>
## [Qualcomm Acquires AI Startup Modular for $4B](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 8.0/10

Qualcomm announced the acquisition of AI infrastructure startup Modular for $4 billion, aiming to enhance its AI compute capabilities and expand beyond mobile chips. This acquisition signals Qualcomm's strategic push into high-performance AI compute, potentially challenging Nvidia's dominance in the AI hardware-software stack. Modular is known for its Mojo programming language and unified AI inference platform; the deal includes Modular's team and technology, with Chris Lattner continuing to lead the division.

hackernews · timmyd · Jun 24, 13:49 · [Discussion](https://news.ycombinator.com/item?id=48659798)

**Background**: Modular was founded in 2022 by former Apple and Google engineers, including Chris Lattner, creator of the LLVM compiler infrastructure. The startup raised $250 million to challenge Nvidia's CUDA software ecosystem. Qualcomm, traditionally a mobile chip leader, has been expanding into AI accelerators with its Dragonfly platform and NPU technology.

<details><summary>References</summary>
<ul>
<li><a href="https://www.qualcomm.com/">Qualcomm : Intelligent Computing Everywhere</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some see it as a bold strategic move by Qualcomm to compete in AI compute and RISC-V, while others question the fit given Qualcomm's limited presence in high-end inference/training. There is also debate about Mojo's direction and whether Chris Lattner's talents were optimally used.

**Tags**: `#acquisition`, `#AI`, `#hardware`, `#Qualcomm`, `#Modular`

---

<a id="item-4"></a>
## [HDD-RoPE: High-Dimensional Dynamic Rotary Positional Embedding](https://www.reddit.com/r/MachineLearning/comments/1uelcm9/high_dimensional_dynamic_rotary_positional/) ⭐️ 8.0/10

A new positional embedding method called HDD-RoPE (High-Dimensional Dynamic Rotary Positional Embedding) has been introduced, which uses data-dependent, multi-dimensional rotations instead of the fixed 2D rotations in standard RoPE. The method shows faster convergence on the TinyStories dataset compared to the xPos baseline. This advancement could improve the efficiency of transformer training by enabling faster convergence, potentially reducing computational costs. It also introduces a more flexible notion of position that may capture hierarchical structures like paragraphs or sentences, benefiting NLP models. HDD-RoPE breaks queries and keys into chunks of arbitrary size (e.g., 4) and rotates each chunk in a multi-dimensional space, with rotation rates learned from layer activations. The open-source repository provides code to replicate results on TinyStories using a GPT-2-like model with 4 blocks and 768-dimensional embeddings.

reddit · r/MachineLearning · /u/mikayahlevi · Jun 24, 18:16

**Background**: Rotary Positional Embedding (RoPE) encodes position by rotating pairs of query and key elements at fixed frequencies, enabling relative position learning. xPos is an enhancement to RoPE that addresses certain limitations. HDD-RoPE extends this idea by allowing higher-dimensional rotations that are dynamically adjusted based on the input data.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/jploski/RotaryEmbedding">jploski/RotaryEmbedding: Comparison of RoPE and xPos positional ...</a></li>

</ul>
</details>

**Discussion**: The community discussion on Reddit includes technical questions about the implementation and comparisons with other positional embeddings. The author actively engages, providing clarifications on the mathematical details and potential applications.

**Tags**: `#positional embedding`, `#transformer`, `#machine learning`, `#RoPE`, `#NLP`

---

<a id="item-5"></a>
## [DeepSWE: New Benchmark Tests Frontier Coding Models](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 8.0/10

DeepSWE is a new open-source benchmark for evaluating frontier coding agents, featuring contamination-free tasks written from scratch, high diversity across 91 repositories and 5 languages, and real-world complexity with prompts half the length of SWE-bench Pro but requiring 5.5x more code. This benchmark addresses key limitations of existing benchmarks like SWE-bench, such as data contamination and lack of diversity, providing a more reliable measure of how well AI models can handle real-world software engineering tasks. DeepSWE uses hand-written verifiers that test software behavior rather than implementation details, and its tasks are designed to be contamination-free so no model has seen the solutions during pretraining.

reddit · r/MachineLearning · /u/we_are_mammals · Jun 24, 02:03

**Background**: Benchmarks like SWE-bench evaluate AI models on software engineering tasks but often suffer from data contamination, where models may have seen similar tasks during training. DeepSWE aims to provide a more accurate assessment by creating entirely new tasks and using diverse repositories across multiple programming languages.

<details><summary>References</summary>
<ul>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE measures frontier coding agents on original, long-horizon...</a></li>
<li><a href="https://www.stork.ai/blog/ais-reality-check-the-benchmark-that-broke-llms">DeepSWE: The AI Coding Benchmark Exposing Real LLM... | Stork.AI</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is active, with users praising the benchmark's contamination-free design and diversity, though some question whether the hand-written verifiers might introduce bias. Overall sentiment is positive, with many seeing DeepSWE as a valuable addition to the evaluation landscape.

**Tags**: `#benchmark`, `#coding agents`, `#LLM evaluation`, `#software engineering`, `#open-source`

---

<a id="item-6"></a>
## [RubyLLM: A Ruby framework for all major AI providers](https://rubyllm.com/) ⭐️ 7.0/10

RubyLLM is a new Ruby framework that provides a unified API for interacting with major AI providers like OpenAI, Anthropic, and Google, enabling developers to build chatbots, AI agents, and RAG applications with minimal code. RubyLLM fills a gap in the Ruby ecosystem by offering a single, elegant interface for multiple AI providers, making AI integration more accessible to Ruby developers and potentially accelerating AI adoption in Ruby-based projects. The framework supports features like streaming, tool calling, and multimodal inputs, but community reports indicate cache issues with some providers (e.g., xAI) and limited maintainer responsiveness to pull requests.

hackernews · doener · Jun 24, 14:41 · [Discussion](https://news.ycombinator.com/item?id=48660711)

**Background**: Ruby is a dynamic, object-oriented programming language popular for web development, especially with the Rails framework. As AI services proliferate, developers need libraries that abstract away provider-specific APIs to reduce boilerplate and simplify maintenance. RubyLLM aims to be that abstraction layer for Ruby.

<details><summary>References</summary>
<ul>
<li><a href="https://rubyllm.com/">RubyLLM | One beautiful Ruby framework for all major AI providers. Chat ...</a></li>
<li><a href="https://github.com/crmne/ruby_llm">GitHub - crmne/ruby_llm: One delightful Ruby framework for every major ...</a></li>
<li><a href="https://cside.com/blog/ai-api-shared-cache-data-leaks">When an AI API returns another user's response: shared caches and cross-tenant leaks - cside Blog</a></li>

</ul>
</details>

**Discussion**: The community generally praises RubyLLM for its ease of use and clean API, with some users comparing it favorably to Vercel's AI SDK. However, concerns include cache reliability, lack of native support for certain APIs (e.g., responses API), and difficulty in engaging the maintainer for contributions.

**Tags**: `#Ruby`, `#AI`, `#framework`, `#LLM`, `#open-source`

---

<a id="item-7"></a>
## [Google Adds Computer Use to Gemini 3.5 Flash](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/) ⭐️ 7.0/10

Google has integrated computer use capabilities directly into Gemini 3.5 Flash, allowing the model to interact with desktop applications and web browsers autonomously. This feature was previously only available as a separate Gemini 2.5 model. This move brings agentic AI capabilities to a faster, more accessible model, potentially enabling more developers to build automation tools. However, community feedback highlights reliability issues and comparisons with competitors like Claude and GPT, suggesting the technology is still maturing. The computer use feature is now a built-in tool in Gemini 3.5 Flash, delivering Google's best performance for agentic computer use tasks. Google also introduced a 'Select from screen' tool in Chrome for Gemini, enhancing user interaction.

hackernews · swolpers · Jun 24, 17:21 · [Discussion](https://news.ycombinator.com/item?id=48662999)

**Background**: Large language models (LLMs) like Gemini are AI systems that understand and generate human language. When given agentic capabilities, they can perform tasks autonomously, such as controlling a computer interface. Computer use refers to an LLM's ability to interact with graphical user interfaces (GUIs) by moving the cursor, clicking buttons, and typing text, similar to a human user.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/">Introducing computer use in Gemini 3 . 5 Flash</a></li>
<li><a href="https://9to5google.com/2026/06/24/gemini-chrome-select-screen/">Gemini in Chrome adds ‘Select from screen’ tool</a></li>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3 . 5 Flash — Google DeepMind</a></li>

</ul>
</details>

**Discussion**: Community comments reveal mixed experiences: some users report Gemini giving up on tasks or performing unexpected actions like running 'git reset --hard', while others note the lack of MCP support and coding tools comparable to Codex or Claude Code. A user also pointed out that Google's own benchmark graph shows Gemini 3.5 Flash being outperformed by Opus 4.8 and GPT 5.5, despite the graph's presentation.

**Tags**: `#AI`, `#Gemini`, `#LLM`, `#computer-use`, `#Google`

---

<a id="item-8"></a>
## [PR Spam Today Mirrors Early 2000s Email Spam](https://www.greptile.com/blog/prs-on-openclaw) ⭐️ 7.0/10

A blog post on Greptile draws parallels between modern pull request spam and early 2000s email spam, arguing that open-source maintainers need better reputation systems and tools to combat it. As open-source projects grow, PR spam wastes maintainers' time and discourages contributions, threatening project health. Drawing lessons from email spam history could lead to effective solutions like reputation systems. The article highlights that PR spam often involves low-quality or automated submissions promoting products or services. GitHub recently added configurable PR limits for maintainers to help address the problem.

hackernews · dakshgupta · Jun 24, 14:32 · [Discussion](https://news.ycombinator.com/item?id=48660579)

**Background**: Email spam in the early 2000s overwhelmed inboxes until reputation systems (e.g., sender scores, blacklists) and filtering tools were developed. Similarly, open-source projects now face a surge of spam pull requests and issues, which lack robust reputation mechanisms. The comparison suggests that platform-level reputation systems for contributors could mitigate the problem.

<details><summary>References</summary>
<ul>
<li><a href="https://www.axiapr.com/blog/hagglers-complaint-pr-spam-work">The Haggler’s complaint – Does “ PR spam ” work?</a></li>

</ul>
</details>

**Discussion**: Commenters noted differences: email spam relied on server reputation, while PR spam involves individual users. Some suggested requiring non-textual verification (e.g., meeting maintainers) or donating token credits to projects. GitHub's new PR limits were seen as a partial solution.

**Tags**: `#open-source`, `#spam`, `#pull-requests`, `#maintainer-tools`, `#community`

---

<a id="item-9"></a>
## [NVIDIA's 45°C Cooling Cuts Data Center Water Use](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 7.0/10

NVIDIA announced a direct-to-chip liquid cooling architecture that operates at a coolant temperature of up to 45°C, enabling near-zero water consumption in data centers. This innovation significantly reduces water usage, a critical environmental concern for data centers, and opens the door to waste heat reuse for district heating, improving overall energy efficiency. The 45°C coolant temperature is higher than typical liquid cooling systems, which reduces or eliminates the need for water-intensive evaporative cooling; the design also enables potential integration with district heating networks that can utilize the waste heat.

hackernews · nitin_flanker · Jun 24, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48660178)

**Background**: Traditional data centers rely on air conditioning or water-intensive evaporative cooling to remove heat from servers. As AI workloads increase rack densities, liquid cooling becomes more efficient. NVIDIA's approach uses warmer coolant, reducing energy and water consumption while still maintaining safe operating temperatures for chips.

<details><summary>References</summary>
<ul>
<li><a href="https://www.guru3d.com/story/nvidia-unveils-liquid-cooling-design-for-ai-data-centers/">NVIDIA Unveils 45 ° C Liquid Cooling Design for AI Data Centers</a></li>
<li><a href="https://www.techbuzz.ai/articles/nvidia-s-45-c-liquid-cooling-redefines-ai-data-center-energy">NVIDIA's 45 ° C Liquid Cooling Redefines AI Data Center Energy</a></li>
<li><a href="https://www.araner.com/blog/data-center-and-district-heating-an-outstanding-combination">Data center and district heating : an outstanding combination</a></li>

</ul>
</details>

**Discussion**: Commenters questioned the novelty of the approach, noting that other facilities already use similar warm-water cooling. Some highlighted the potential for district heating synergy, while others asked for more details on climate dependency and implementation costs.

**Tags**: `#data center`, `#cooling`, `#energy efficiency`, `#NVIDIA`, `#liquid cooling`

---

<a id="item-10"></a>
## [GLM-5.2: A Step Change for Open Agents](https://www.interconnects.ai/p/glm-52-is-the-step-change-for-open) ⭐️ 7.0/10

Z.ai released GLM-5.2, an open-weight model with a 1M-token context, on June 13, 2026, claiming performance on par with proprietary models like Claude 4.8 Opus and GPT-5.5. GLM-5.2 significantly narrows the gap between open and proprietary models, offering a cost-effective alternative for users who cannot afford expensive subscriptions, potentially democratizing access to advanced AI agents. The model outperforms Opus 4.7 and GPT-5.5 on PostTrainBench, ranking second only to Opus 4.8, and supports dynamic 1-bit quantization achieving ~76.2% top-1 accuracy while being 86% smaller.

hackernews · vantareed · Jun 23, 03:23 · [Discussion](https://news.ycombinator.com/item?id=48639840)

**Background**: Open-weight models allow anyone to download and run the model parameters locally, offering transparency and flexibility. Chinese AI labs like Z.ai have been releasing competitive open-weight models at lower prices, challenging US-based proprietary models. GLM-5.2 is the latest in this trend, targeting long-horizon agent tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://registry.ollama.ai/library/glm-5.2">GLM - 5 . 2 is Z.ai’s flagship model for the era of long-horizon tasks.</a></li>
<li><a href="https://www.buildfastwithai.com/blogs/glm-5-2-review-2026">GLM - 5 . 2 Review 2026: Z.ai's 1M-Context AI Model</a></li>
<li><a href="https://unsloth.ai/docs/models/glm-5.2">Run the new GLM - 5 . 2 model by Z.ai on local hardware!</a></li>

</ul>
</details>

**Discussion**: Community members praise GLM-5.2's cost-effectiveness and competitive performance, with some finding it nearly indistinguishable from Codex or Claude Code for coding tasks. However, several users report excessive token consumption and quota issues, calling the pricing plan a 'scam' and noting that the model burns through tokens much faster than alternatives.

**Tags**: `#AI`, `#open-source`, `#LLM`, `#cost`, `#Chinese AI`

---

<a id="item-11"></a>
## [Elastic Lays Off 7% of Workforce, Cites AI](https://www.elastic.co/blog/ceo-ash-kulkarni-announcement-to-elastic-employees) ⭐️ 7.0/10

Elastic announced a 7% reduction in its workforce, citing advances in AI, automation, and technology as the reason for restructuring, while planning to hire more in go-to-market roles. This layoff reflects a broader trend where tech companies use AI to justify workforce reductions, raising concerns about job displacement and corporate communication transparency. The layoff affects approximately 7% of employees, and the company expects to grow headcount in go-to-market roles despite the reduction. The announcement focuses heavily on future optimism rather than the layoffs themselves.

hackernews · dakrone · Jun 24, 21:57 · [Discussion](https://news.ycombinator.com/item?id=48666100)

**Background**: Elastic is a major tech company known for its Elasticsearch and Kibana products. Layoffs in the tech industry have become common, often attributed to AI and automation, but critics argue they are sometimes used to mask mismanagement.

**Discussion**: Community comments express sadness and skepticism, with some calling the layoff a sign of mismanagement and others noting the disproportionate focus on future growth in the announcement. One commenter predicts that big companies will lose headcount to AI while small companies will leverage AI to grow.

**Tags**: `#layoffs`, `#AI`, `#tech industry`, `#Elastic`, `#corporate restructuring`

---

<a id="item-12"></a>
## [Nub: A Bun-like All-in-One Toolkit for Node.js](https://github.com/nubjs/nub) ⭐️ 7.0/10

Nub is a new open-source toolkit that enhances Node.js with Bun-like features such as transpilation, module resolution, and polyfills via a lightweight --require preload hook, without replacing the Node.js runtime. Nub improves developer experience by enabling modern JavaScript and TypeScript features on stock Node.js, bridging the gap between Node.js and Bun's all-in-one approach, and is created by Colin McDonnell, author of Zod and former Bun engineer, lending it credibility. Nub uses the oxc transpiler (packaged as a Node-API add-on) for fast TypeScript/JSX transformation, registers a module resolution hook, and injects polyfills for APIs like Worker and Temporal. It is purely additive, running code on Node's actual engine and stdlib.

hackernews · colinmcd · Jun 24, 14:14 · [Discussion](https://news.ycombinator.com/item?id=48660267)

**Background**: Bun is a fast all-in-one JavaScript runtime that includes a transpiler, bundler, and package manager, but it is not Node.js-compatible in all aspects. Node.js natively supports TypeScript stripping since v22, but lacks built-in transpilation for JSX and advanced module resolution. Nub fills this gap by adding these capabilities via hooks without changing the runtime.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/oxc-project/oxc">GitHub - oxc-project/oxc: ⚓ A collection of high-performance JavaScript tools.</a></li>
<li><a href="https://nodejs.org/api/module.html">Modules: `node:module` API | Node.js v26.3.1 Documentation</a></li>
<li><a href="https://nodejs.org/api/esm.html">Modules: ECMAScript modules | Node.js v26.3.1 Documentation</a></li>

</ul>
</details>

**Discussion**: The community reception is positive, with users praising the idea and execution. Some discussed ESM support nuances and the choice of --require over --import, while others reported successful migration with zero issues. The creator's background (Zod author, ex-Bun) adds trust.

**Tags**: `#Node.js`, `#Tooling`, `#TypeScript`, `#Developer Experience`, `#Bun`

---

<a id="item-13"></a>
## [Simon Willison Creates SQLite DB from MDN Browser Compat Data](https://simonwillison.net/2026/Jun/24/browser-compat-db/#atom-everything) ⭐️ 7.0/10

Simon Willison created a SQLite database from MDN's browser compatibility data, hosted on GitHub with open CORS headers, and built using AI-assisted scripts. This makes browser compatibility data easily queryable and accessible offline, benefiting developers who need to check feature support across browsers without relying on MDN's website or API. The ~66MB SQLite database is built via a GitHub Actions workflow that force-pushes to an orphan branch, enabling open CORS headers for direct use with tools like Datasette Lite.

rss · Simon Willison · Jun 24, 23:59

**Background**: MDN's browser compatibility data is a comprehensive JSON dataset tracking which web features are supported in which browser versions. Simon Willison's project repackages this data into SQLite format, making it more accessible for offline querying and integration with other tools.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/blog/introducing-mdn-mcp-server/">Introducing the MDN MCP server - MDN Web Docs</a></li>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library for manipulating SQLite databases · GitHub</a></li>

</ul>
</details>

**Tags**: `#browser-compat`, `#sqlite`, `#developer-tools`, `#data-engineering`

---

<a id="item-14"></a>
## [LLM-Generated Job Apps Obscure Candidate Authenticity](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 7.0/10

Tom MacWright observed that many recent job applications are clearly co-written by LLMs, linking to LLM-generated portfolios and GitHub projects with purely LLM-generated commit messages, making it impossible to assess the candidate's true abilities and personality. This trend threatens the integrity of the hiring process by eroding the signal that resumes and portfolios are meant to provide, making it harder for employers to distinguish genuine talent from generic, AI-generated content. MacWright's blog post titled 'Accidental anonymity' highlights that the perfected, generated resume is generic and impersonal, telling nothing about the person except their use of particular tools.

rss · Simon Willison · Jun 24, 18:13

**Background**: Large Language Models (LLMs) like GPT-4 are increasingly used to generate text, including resumes, cover letters, and code. While they can boost productivity, their misuse in job applications can produce content that lacks personal voice and genuine experience, making it difficult for recruiters to evaluate candidates.

**Tags**: `#AI`, `#careers`, `#hiring`, `#LLM`

---

<a id="item-15"></a>
## [Datasette 1.0a35 Adds Create/Alter Table APIs](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a35 introduces a new create table interface and JSON API for defining columns, primary keys, constraints, and foreign keys, as well as an alter table interface and JSON API for modifying existing tables, including adding, renaming, reordering, and dropping columns. These features mark a significant step toward the 1.0 release, enabling users to manage database schemas entirely through Datasette's UI and API without external tools, which greatly enhances its utility as a data publishing and exploration platform. The create table API supports custom column types, NOT NULL constraints, literal and expression defaults, and single-column foreign keys. The alter table API also includes a drop table button, and both APIs are backed by stable JSON endpoints documented in the official docs.

rss · Simon Willison · Jun 23, 21:34

**Background**: Datasette is an open-source tool for exploring and publishing data, especially SQLite databases. It provides a web interface and JSON API for querying and browsing data. Prior to this release, creating or altering tables required using SQLite command-line tools or other external methods.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/latest/json_api.html?highlight=pagination">JSON API - Datasette documentation</a></li>
<li><a href="https://simonwillison.net/2026/jun/23/datasette/">Release: datasette 1.0a35 | Simon Willison’s Weblog</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#open-source`, `#data tools`, `#release`

---

<a id="item-16"></a>
## [Curated Open-Source OCR Models Hub on Papers with Code](https://www.reddit.com/r/MachineLearning/comments/1ueiam6/find_the_best_opensource_ocr_models_in_one_place/) ⭐️ 7.0/10

A new curated page on Papers with Code lists top open-source OCR models with benchmarks, featuring Baidu's Unlimited OCR (3B parameters with Reference Sliding Window Attention) and Mistral OCR v4 via API. This centralized resource helps AI practitioners quickly select the best OCR model for document digitization and agentic RAG, accelerating adoption of open-source OCR in enterprise workflows. The page includes benchmarks like OlmOCRBench and OmniDocBench, and recommends Chandra OCR 2 (open-source, self-hostable) and Mistral OCR v4. Baidu's Unlimited OCR builds on DeepSeek OCR with R-SWA for efficient long-document processing.

reddit · r/MachineLearning · /u/NielsRogge · Jun 24, 16:26

**Background**: OCR (Optical Character Recognition) converts scanned documents and PDFs into machine-readable text, often Markdown. Agentic RAG uses such text to power AI agents that retrieve and generate answers from company data. Papers with Code is a platform that tracks research papers, code, and benchmarks for machine learning tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/reference-sliding-window-attention-r-swa">Reference Sliding Window Attention ( R - SWA )</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>
<li><a href="https://www.runlocalai.co/glossary/sliding-window-attention">Sliding Window Attention ( SWA ) — AI glossary | RunLocalAI</a></li>

</ul>
</details>

**Tags**: `#OCR`, `#open-source`, `#AI agents`, `#document digitization`, `#RAG`

---

<a id="item-17"></a>
## [MuJoFil: GPU-Native Simulator for Vision RL Training](https://www.reddit.com/r/MachineLearning/comments/1uemrch/mujoco_derived_simulator_for_high_fidelity_vision/) ⭐️ 7.0/10

MuJoFil, a new open-source simulator, combines NVIDIA Newton physics engine with Google Filament render engine to enable high-fidelity vision-based reinforcement learning training natively on GPU. It fills a gap by providing an accessible, GPU-accelerated alternative to MuJoCo and Isaac Sim for vision RL, potentially democratizing high-fidelity robot learning simulation. MuJoFil supports PBR textures and formats like GLB and OpenUSD, and is available via pip as mujofil (CPU) and mujofil-warp (GPU/CUDA). The project is early-stage with known bugs.

reddit · r/MachineLearning · /u/MT1699 · Jun 24, 19:07

**Background**: MuJoCo is a popular physics simulator but runs on CPU, limiting parallelization for vision RL. MJX offers GPU acceleration but lacks rendering for vision tasks. NVIDIA Isaac Sim provides high fidelity but requires powerful GPUs and a license. MuJoFil aims to combine GPU physics (Newton) and rendering (Filament) in an open-source package.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/newton-physics">Newton Physics Engine | NVIDIA Developer</a></li>
<li><a href="https://google.github.io/filament/dup/intro.html?trk=article-ssr-frontend-pulse_little-text-block">Introduction - Filament</a></li>
<li><a href="https://pypi.org/project/mujoco-mjx/">mujoco - mjx · PyPI</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#simulation`, `#GPU`, `#MuJoCo`, `#open-source`

---

<a id="item-18"></a>
## [LLM Inference Pricing Comparison Reveals Surprising Caching Costs](https://www.reddit.com/r/MachineLearning/comments/1ueavxn/i_compiled_llm_inference_pricing_across_7/) ⭐️ 7.0/10

A Reddit user compiled a spreadsheet comparing LLM inference pricing across 7 providers (OpenRouter, DeepSeek, Together AI, Fireworks, Groq, etc.), highlighting that cached input costs can be tens of times cheaper than uncached inputs for models like DeepSeek V4 Pro. This comparison matters because caching policies can dramatically affect total cost for applications with repeated prompts, such as agents, RAG pipelines, and multi-turn conversations, making caching a more important factor than headline token pricing. The spreadsheet tracks input/output token pricing, context windows, cached input pricing, and supported models, but does not include real throughput, cold-start times, or quantization details. The same model can vary multiple times in cost across providers.

reddit · r/MachineLearning · /u/Technomadlyf · Jun 24, 11:28

**Background**: LLM inference caching stores previously computed token representations (e.g., KV cache) so that repeated prompt prefixes can skip recomputation, reducing latency and cost. Providers like DeepSeek, OpenRouter, and Together AI offer prompt caching, but documentation and pricing transparency vary widely.

<details><summary>References</summary>
<ul>
<li><a href="https://www.knolli.ai/post/inference-caching-in-llms">Inference Caching in Large Language Models (LLMs) [Complete Guide]</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-pro">DeepSeek V4 Pro - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://api-docs.deepseek.com/quick_start/pricing">Models & Pricing | DeepSeek API Docs</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion praised the spreadsheet as a valuable resource and debated which metrics matter most beyond token pricing, such as throughput, reliability, and caching policies. Some users noted that caching costs are often hidden or poorly documented.

**Tags**: `#LLM`, `#pricing`, `#inference`, `#caching`, `#cloud providers`

---

<a id="item-19"></a>
## [Are ML teams testing model security in production?](https://www.reddit.com/r/MachineLearning/comments/1uddtws/are_model_security_risks_extraction_poisoning/) ⭐️ 7.0/10

A Reddit post highlights that many ML teams skip adversarial testing for model extraction and poisoning before deploying models, contrasting with standard security reviews in traditional software. This gap exposes deployed models to serious risks like intellectual property theft and behavioral manipulation, especially in critical sectors like healthcare and autonomous vehicles. Model extraction attacks steal model functionality via API queries, while poisoning attacks alter training data to corrupt model behavior; both are well-documented but rarely tested in production.

reddit · r/MachineLearning · /u/Xorphian · Jun 23, 10:52

**Background**: Adversarial machine learning studies attacks and defenses for ML models. Model extraction involves querying a model to build a replica, while poisoning injects malicious data during training. Traditional software security reviews are standard, but ML security testing lags behind.

<details><summary>References</summary>
<ul>
<li><a href="https://www.praetorian.com/blog/stealing-ai-models-through-the-api-a-practical-model-extraction-attack/">Stealing AI Models Through the API: A Practical Model Extraction Attack | Praetorian</a></li>
<li><a href="https://owasp.org/www-project-machine-learning-security-top-10/docs/ML10_2023-Model_Poisoning">OWASP Machine Learning Security Top Ten 2023 | ML10:2023 Model Poisoning | OWASP Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adversarial_machine_learning">Adversarial machine learning - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#ML security`, `#adversarial testing`, `#model extraction`, `#model poisoning`, `#production ML`

---

<a id="item-20"></a>
## [uv 0.11.24 Adds CPython 3.15.0b3 and Relocatable Environments](https://github.com/astral-sh/uv/releases/tag/0.11.24) ⭐️ 6.0/10

uv 0.11.24 adds support for CPython 3.15.0b3 and introduces relocatable project environments under the preview flag. It also includes performance improvements like a compact index for lazy version maps and several bug fixes. Relocatable environments allow users to move or share project environments without breaking paths, improving portability in CI/CD and team workflows. The addition of CPython 3.15.0b3 ensures uv stays compatible with the latest Python beta releases. The relocatable environment feature is currently under the preview flag, meaning it may change in future releases. The compact index for lazy version maps reduces memory usage and speeds up dependency resolution.

github · github-actions[bot] · Jun 23, 21:16

**Background**: uv is a fast, all-in-one Python package manager developed by Astral (now part of OpenAI), designed to replace pip, pyenv, pipx, and virtualenv. It creates virtual environments in milliseconds and installs packages significantly faster than pip. Relocatable environments allow the entire project environment directory to be moved to a different location without breaking references.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/python-uv">Python UV: The Ultimate Guide to the Fastest Python Package Manager | DataCamp</a></li>
<li><a href="https://tutorials.technology/tutorials/uv-python-package-manager-2026.html">uv: The Python Package Manager That Replaces pip, pyenv, and Poetry (2026) | Tech Tutorials</a></li>
<li><a href="https://pydevtools.com/handbook/explanation/uv-complete-guide/">uv: A Complete Guide to Python's Fastest Package Manager | pydevtools</a></li>

</ul>
</details>

**Tags**: `#python`, `#package-manager`, `#release`, `#uv`

---

<a id="item-21"></a>
## [Xteink X4: Tiny Open E-Ink Reader with WiFi Transfer](https://blog.omgmog.net/post/xteink-x4-e-ink-reader/) ⭐️ 6.0/10

The Xteink X4 is a small, open e-ink reader that has gained attention for its simplicity and WiFi-based book transfer, though it lacks a backlight and has a very small screen. This device highlights the growing interest in open hardware e-readers that prioritize user control and simplicity over locked ecosystems like Kindle, appealing to hobbyists and minimalists. The X4 features a microcontroller-based design, USB-C charging, and a magnetic cover for portability, but its screen is smaller than a typical smartphone, making it less suitable for extended reading.

hackernews · felixdoerp · Jun 24, 16:35 · [Discussion](https://news.ycombinator.com/item?id=48662381)

**Background**: E-ink displays use electrophoretic technology to mimic paper, consuming power only when the image changes, making them ideal for e-readers. Open hardware e-readers like the Xteink X4 allow users to modify software and avoid vendor lock-in, contrasting with proprietary devices like Amazon's Kindle.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/E_Ink">E Ink - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Electronic_paper">Electronic paper - Wikipedia</a></li>
<li><a href="https://www.youtube.com/watch?v=l4dE_cqiOQc">The Open Book: An Open Hardware E -Book Reader - YouTube</a></li>

</ul>
</details>

**Discussion**: Community members praised the X4's WiFi transfer and open nature, with some using it as a secondary device. However, many criticized the tiny screen size and lack of backlight, noting it's not suitable as a primary e-reader, especially for older eyes.

**Tags**: `#e-reader`, `#open hardware`, `#e-ink`, `#hobbyist`

---

<a id="item-22"></a>
## [OPFS + Pyodide Test Harness for Datasette Lite](https://simonwillison.net/2026/Jun/23/opfs-pyodide/#atom-everything) ⭐️ 6.0/10

Simon Willison built a test harness that combines the Origin Private File System (OPFS) with Pyodide to explore whether Datasette Lite can edit persistent SQLite files stored in the browser. If successful, this would enable Datasette Lite to offer persistent local data editing entirely in the browser, eliminating the need for a server and expanding its use cases for offline or privacy-sensitive data work. The test harness is a playground UI generated by Claude Code for web, allowing interactive testing of OPFS file operations across different browsers. OPFS provides low-level, byte-by-byte file access that is private to the page's origin and faster than the File System Access API.

rss · Simon Willison · Jun 23, 18:58

**Background**: Datasette Lite runs the full Datasette Python web application in the browser via Pyodide (Python compiled to WebAssembly). The Origin Private File System (OPFS) is a browser API that provides a sandboxed, origin-specific virtual filesystem for storing files that are not visible to the user's file manager. Combining them could allow Datasette Lite to persistently store and edit SQLite databases locally.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN</a></li>
<li><a href="https://github.com/simonw/datasette-lite">GitHub - simonw/ datasette - lite : Datasette running in your browser...</a></li>
<li><a href="https://simonwillison.net/2022/May/4/datasette-lite/">Datasette Lite : a server-side Python web application running in...</a></li>

</ul>
</details>

**Tags**: `#pyodide`, `#webassembly`, `#datasette-lite`, `#opfs`, `#browsers`

---