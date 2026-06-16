---
layout: default
title: "Horizon Summary: 2026-06-16 (EN)"
date: 2026-06-16
lang: en
---

> From 41 items, 21 important content pieces were selected

---

1. [Backdoor in Fake LinkedIn Job Offer Exploits npm](#item-1) ⭐️ 9.0/10
2. [Iroh 1.0: Peer-to-Peer Networking Library Reaches Stable](#item-2) ⭐️ 8.0/10
3. [Developers Share Local LLM Setups for Daily Coding](#item-3) ⭐️ 8.0/10
4. [Hetzner Cloud Prices Surge Up to 3x Amid AI-Driven Hardware Costs](#item-4) ⭐️ 8.0/10
5. [Fox to Acquire Roku in Major Streaming Deal](#item-5) ⭐️ 8.0/10
6. [AI Won't Replace Software Engineers, Experts Argue](#item-6) ⭐️ 8.0/10
7. [LLMs exhibit model-specific name priors as correlated hallucinations](#item-7) ⭐️ 8.0/10
8. [Cleo: Fitting Full Analyst Behavior in a 2B Model](#item-8) ⭐️ 8.0/10
9. [New Framework Claims to Unify Neocortical Learning](#item-9) ⭐️ 8.0/10
10. [Banned Book Library Stored in a Wi-Fi Smart Light Bulb](#item-10) ⭐️ 7.0/10
11. [A Personal Essay on Loving Computers Amid Industry Hype](#item-11) ⭐️ 7.0/10
12. [Homelab AI Dev Platform with Gitea and systemd Sandboxing](#item-12) ⭐️ 7.0/10
13. [Feasibility of a Peopleless Economy](#item-13) ⭐️ 7.0/10
14. [US Battery Manufacturing Output Hits Record Highs](#item-14) ⭐️ 7.0/10
15. [Anthropic's Fable AI Refuses Security Review, Then Complies](#item-15) ⭐️ 7.0/10
16. [Open training frameworks needed beyond open weights](#item-16) ⭐️ 7.0/10
17. [Embedded ML: Data Cleaning vs. Collection Bottleneck](#item-17) ⭐️ 7.0/10
18. [Open-source KG pipeline with hybrid retrieval boosts LLM reasoning](#item-18) ⭐️ 7.0/10
19. [Datasette Agent 0.3a0 Adds Write SQL with User Approval](#item-19) ⭐️ 6.0/10
20. [EA PhD Career Prospects in ML Community](#item-20) ⭐️ 6.0/10
21. [Why AI Labs Send Many People to Conferences](#item-21) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Backdoor in Fake LinkedIn Job Offer Exploits npm](https://roman.pt/posts/linkedin-backdoor/) ⭐️ 9.0/10

A job applicant discovered a backdoor hidden in a GitHub repository sent by a recruiter as part of a fake interview process, exploiting npm's prepare script to execute arbitrary code when dependencies are installed. This incident highlights a new social engineering attack vector targeting job seekers in tech, where attackers use fake coding challenges to deliver malware, and it underscores the lack of platform response from GitHub and LinkedIn. The backdoor was buried in commented-out test code and executed via npm's prepare script, which runs automatically after npm install. The payload communicates with a remote server to execute arbitrary commands on the victim's machine.

hackernews · lwhsiao · Jun 15, 20:00 · [Discussion](https://news.ycombinator.com/item?id=48546294)

**Background**: npm's prepare script is a lifecycle hook that runs automatically after npm install, often used for build steps. Attackers can abuse it to execute arbitrary code without user interaction. Supply chain attacks on npm have been increasing, with recent incidents like the Shai-Hulud worm compromising hundreds of packages.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/github-automated-disable-npm-script-installs/">GitHub to Automated Disable npm Script Installs to Block ...</a></li>
<li><a href="https://stackoverflow.com/questions/44499912/why-is-npm-running-prepare-script-after-npm-install-and-how-can-i-stop-it">node.js - Why is npm running prepare script after npm install ... Usage example</a></li>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern that this attack is uncomfortably close to normal interview tasks, and criticized GitHub and LinkedIn for not removing the malicious content. Some noted the same domain was used in a similar Reddit post three months ago, suggesting an ongoing campaign.

**Tags**: `#security`, `#supply chain attack`, `#npm`, `#social engineering`, `#cybercrime`

---

<a id="item-2"></a>
## [Iroh 1.0: Peer-to-Peer Networking Library Reaches Stable](https://www.iroh.computer/blog/v1) ⭐️ 8.0/10

Iroh 1.0, a peer-to-peer networking library for Rust, has been released after 4+ years and 65+ releases, introducing dial keys that replace IP addresses with public keys for direct connections. This simplifies building peer-to-peer applications by handling NAT traversal, relay, and path selection automatically, making it easier for developers to create decentralized apps without managing complex networking infrastructure. Iroh uses QUIC connections identified by public keys (EndpointId), supports IPv4, IPv6, and relay transports out of the box, and now allows custom transports via a plugin system.

hackernews · chadfowler · Jun 15, 15:13 · [Discussion](https://news.ycombinator.com/item?id=48542480)

**Background**: Traditional networking relies on IP addresses, which can change and break connections. Iroh uses a 'magic socket' that discovers paths to peers using their public keys, enabling robust connections even through NATs and firewalls. It is similar to Tailscale but operates at the application layer.

<details><summary>References</summary>
<ul>
<li><a href="https://www.iroh.computer/">Iroh</a></li>
<li><a href="https://github.com/n0-computer/iroh">GitHub - n0-computer/iroh: IP addresses break, dial keys ... n0-computer/iroh | DeepWiki Iroh 1.0: Dial Keys, Not IPs — P2P Hits Stable | byteiota Iroh — Rust network library // Lib.rs iroh 0.23.0 - Welcoming Node.js to the family! - Iroh iroh - Iroh is a modular networking stack for building ...</a></li>
<li><a href="https://deepwiki.com/n0-computer/iroh">n0-computer/iroh | DeepWiki</a></li>

</ul>
</details>

**Discussion**: The community praised the custom transport feature, with a developer noting it prevents codebase bloat. Some users compared Iroh to Tailscale and libp2p, while others questioned the need for a new networking layer, but overall sentiment was positive.

**Tags**: `#networking`, `#peer-to-peer`, `#rust`, `#open-source`, `#release`

---

<a id="item-3"></a>
## [Developers Share Local LLM Setups for Daily Coding](https://news.ycombinator.com/item?id=48542100) ⭐️ 8.0/10

Developers on Hacker News are reporting successful replacements of cloud-based coding assistants like Claude and GPT with local models such as Qwen3.6 35B and Gemma 4, achieving speeds over 150 tokens per second on dual RTX 3090 setups. This shift offers developers greater privacy, lower costs, and offline capability, though local models still lag behind frontier cloud models in complex reasoning and tool use, making this a practical trade-off for many. Common setups include Qwen3.6 35B with 3B active parameters for speed, running on Mac Studio with 128GB RAM or dual RTX 3090s, using tools like Pi coding harness and llama.cpp. Performance is comparable to edge models from 8-12 months ago.

hackernews · cloudking · Jun 15, 14:46

**Background**: Local LLMs run on the user's own hardware, eliminating data sent to cloud APIs and recurring subscription fees. However, they require significant GPU memory (e.g., 24GB+ VRAM) and offer lower quality than top cloud models like GPT-4 or Claude, especially for complex tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://mljourney.com/how-many-tokens-per-second-is-good-for-local-llms/">How Many Tokens Per Second Is ‘Good’ for Local LLMs?</a></li>
<li><a href="https://www.sitepoint.com/local-vs-cloud-ai-coding-performance-analysis-2026/">Local vs Cloud AI Coding: Latency, Privacy & Performance Guide</a></li>
<li><a href="https://docs.bswen.com/blog/2026-03-11-cloud-vs-local-llm-coding/">Cloud vs Local LLMs for Coding: Which Should You Choose in 2026? | BSWEN</a></li>

</ul>
</details>

**Discussion**: Commenters generally agree that local models are viable for many coding tasks, with some reporting 90% of their work done locally. However, they note that cloud models remain superior for complex reasoning and tool use, and some prefer cheap API alternatives like DeepSeek V4 Flash.

**Tags**: `#local-llm`, `#coding-assistant`, `#privacy`, `#open-source`, `#hardware`

---

<a id="item-4"></a>
## [Hetzner Cloud Prices Surge Up to 3x Amid AI-Driven Hardware Costs](https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/#cloud-servers) ⭐️ 8.0/10

Hetzner announced major price adjustments for its cloud servers, with some products seeing increases of up to 3x, effective immediately. The company attributes the hike to rising hardware costs and surging demand driven by AI workloads. This price increase from a major European cloud provider signals that AI-driven hardware demand is now affecting even budget-friendly providers, potentially reshaping cloud pricing across the industry. Smaller businesses and developers who relied on Hetzner for affordable infrastructure may need to reassess their budgets or explore alternatives. The price adjustment applies to Hetzner Cloud servers, with some configurations seeing up to a 3x increase compared to previous pricing. The company also announced standardization of its server product line, which may involve changes to available configurations.

hackernews · tuhtah · Jun 15, 13:19 · [Discussion](https://news.ycombinator.com/item?id=48540844)

**Background**: Hetzner is a German hosting company known for offering affordable dedicated and cloud servers, popular among developers and small businesses. The recent AI boom has dramatically increased demand for GPUs and high-performance storage, driving up costs for components like NAND flash and DRAM, which in turn raises prices for cloud providers across the board.

<details><summary>References</summary>
<ul>
<li><a href="https://siliconanalysts.com/analysis/nand-shockwave-ai-demand-triggers-ssd-price-explosion">NAND Price Explosion: How AI Demand Is Driving SSD Costs Higher</a></li>
<li><a href="https://informplatform.com/why-ai-demand-is-driving-up-hardware-costs/">Why AI Demand Is Driving Up Hardware Costs</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed, with many users expressing shock at the magnitude of the increase, calling a 3x jump "wild" and questioning the justification. Some commenters note that this reflects broader hardware scarcity and AI-driven demand, while others sarcastically remark that the era of "10x savings by moving to Hetzner" posts may be ending.

**Tags**: `#cloud computing`, `#pricing`, `#AI infrastructure`, `#Hetzner`, `#hardware costs`

---

<a id="item-5"></a>
## [Fox to Acquire Roku in Major Streaming Deal](https://www.wsj.com/business/deals/fox-roku-deal-f6e564f9) ⭐️ 8.0/10

Fox Corporation is reportedly acquiring Roku, the leading streaming hardware platform, in a deal that could reshape the streaming landscape. This acquisition would give Fox direct control over the user interface and data of tens of millions of households, raising serious antitrust and user autonomy concerns. Roku devices power roughly 30-50% of American households, and Fox's ownership could lead to preferential treatment of Fox content and increased advertising.

hackernews · thm · Jun 15, 12:50 · [Discussion](https://news.ycombinator.com/item?id=48540499)

**Background**: Roku is a popular streaming platform that offers hardware devices and a TV operating system, allowing users to access various streaming services. Fox is a major media conglomerate owning news, sports, and entertainment content. Media consolidation has been a growing concern, with critics arguing it reduces competition and consumer choice.

<details><summary>References</summary>
<ul>
<li><a href="https://www.roku.com/what-is-roku">What is Roku – How the Roku Experience Works | Roku</a></li>

</ul>
</details>

**Discussion**: Community comments are overwhelmingly negative, with users expressing fears of a 'Fox News button' on remotes and increased ads. Many are already migrating to alternatives like Nvidia Shield with custom launchers to avoid platform lock-in.

**Tags**: `#acquisition`, `#streaming`, `#media consolidation`, `#Roku`, `#Fox`

---

<a id="item-6"></a>
## [AI Won't Replace Software Engineers, Experts Argue](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan and Sayash Kapoor published an essay arguing that evidence does not support AI causing mass layoffs in software engineering, citing that zero out of 160+ companies in New York checked the AI disclosure box on WARN Act filings in the first year. This data-driven counterargument challenges the dominant narrative of AI-driven job displacement, with implications for software engineers and other professions. It suggests that deep human understanding of codebases, business, and environment remains irreplaceable. The authors identify three real bottlenecks in software engineering: deciding and specifying what to build, verifying and being accountable for what is delivered, and deep human understanding required for both. AI speeds up typing code but not these core activities.

rss · Simon Willison · Jun 14, 23:54

**Background**: The WARN Act requires employers to provide advance notice of mass layoffs. New York became the first state in March 2025 to add an AI disclosure checkbox to WARN filings. The essay by Narayanan and Kapoor, authors of 'AI Snake Oil', provides a qualitative analysis of why software engineering resists automation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kaufmandolowich.com/news-resources/new-york-amends-warn-act-to-require-disclosure-of-ai-related-layoffs-by-keith-j-gutstein-esq-and-shiddhartha-uddin-esq-8-4-2025/">New York Amends WARN Act to Require Disclosure of AI-Related ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#job displacement`, `#labor economics`

---

<a id="item-7"></a>
## [LLMs exhibit model-specific name priors as correlated hallucinations](https://www.reddit.com/r/MachineLearning/comments/1u6mn3q/ai_language_models_have_favorite_names_and_we/) ⭐️ 8.0/10

Researchers discovered that large language models have strong, model-specific priors over character names (e.g., Elena Vasquez, Marcus Chen) that appear as correlated ensembles across dozens of websites, indicating a widespread hallucination phenomenon. The finding was published as a preprint on arXiv. This reveals a novel and significant failure mode of LLMs where hallucinated names propagate across the web, potentially polluting information ecosystems and undermining trust in AI-generated content. It also provides a method to detect which model generated a given text based on name patterns. The names travel as correlated ensembles—for example, Elena Vasquez and Marcus Chen together strongly suggest Claude generation—and appear as volcano experts, podcast hosts, thriller protagonists, and authors of over 1000 papers published in two months. The researchers later found a third name in the ensemble, and a collage shows three different websites independently hallucinating the same trio with AI-generated stock photo faces.

reddit · r/MachineLearning · /u/CebulkaZapiekana · Jun 15, 17:07

**Background**: Large language models (LLMs) sometimes generate plausible-sounding but false information, a phenomenon known as hallucination. This work was a side finding from developing a model diffing method called Contrastive Decoding Diffing (CDD), which extracts fine-tuning content via logit differences without accessing model weights.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/papers/2605.25902">CDD: Verbatim Content Recovery via Diffing</a></li>
<li><a href="https://github.com/science-of-finetuning/diffing-toolkit">GitHub - science-of-finetuning/diffing-toolkit: A toolkit ...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is substantive, with users sharing additional examples and implications. Some commenters noted similar name patterns in their own work, while others discussed the broader impact on AI safety and content verification.

**Tags**: `#LLM`, `#hallucination`, `#AI safety`, `#machine learning`, `#model behavior`

---

<a id="item-8"></a>
## [Cleo: Fitting Full Analyst Behavior in a 2B Model](https://www.reddit.com/r/MachineLearning/comments/1u6udpb/cleo_trying_to_fit_full_analyst_behavior_in_a_2b/) ⭐️ 8.0/10

Cleo is a 2B parameter text-to-SQL model fine-tuned from Qwen3.5-2B-Base, trained and evaluated in a unified harness that enables live query execution search and co-designed safety layers, and is fully open-sourced. This demonstrates that a small 2B model can achieve full analyst behavior for text-to-SQL tasks, making advanced capabilities accessible to resource-constrained teams and enabling practical insights for reinforcement learning. The unified harness trains on the exact same gather-repair-answer contract used at inference, searches over candidate queries with live execution evidence, and co-designs the model contract, SQL safety layer, dialect handling, timeouts, and clarification behavior as one system.

reddit · r/MachineLearning · /u/Dreeseaw · Jun 15, 21:43

**Background**: Text-to-SQL models convert natural language questions into SQL queries. Most industrial chatbots rely on such models or retrieval-augmented generation (RAG). Cleo is built on Qwen3.5-2B-Base, a small multimodal foundation model from Alibaba Cloud released in February 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.5-2B-Base">Qwen/Qwen3.5-2B-Base · Hugging Face</a></li>
<li><a href="https://apxml.com/models/qwen35-2b">Qwen3.5-2B: Specifications and GPU VRAM Requirements</a></li>
<li><a href="https://arxiv.org/pdf/2602.02150">ECHO : Entropy-Confidence Hybrid Optimization for Test-Time...</a></li>

</ul>
</details>

**Tags**: `#text-to-SQL`, `#small language models`, `#open-source`, `#machine learning`, `#NLP`

---

<a id="item-9"></a>
## [New Framework Claims to Unify Neocortical Learning](https://www.reddit.com/r/MachineLearning/comments/1u6x8al/how_the_brains_learn_r/) ⭐️ 8.0/10

A new paper proposes error-driven predictive learning via temporal derivatives as the only framework that fully accounts for neocortical learning, implemented in spiking neurons within the Axon simulation framework. This framework claims to meet all criteria for a general-purpose learning algorithm, potentially offering a biologically plausible alternative to backpropagation that could improve training efficiency and scalability. The framework relies on corticothalamic circuits and competitive kinase synaptic plasticity mechanisms, and has been demonstrated on challenging cognitively motivated tasks using the Axon neural simulation framework.

reddit · r/MachineLearning · /u/Terminator857 · Jun 15, 23:39

**Background**: Neocortical learning is the process by which the brain's neocortex acquires and refines skills and knowledge. Backpropagation, the dominant learning algorithm in artificial neural networks, is not biologically plausible. This work aims to bridge that gap by proposing a learning rule that is both computationally powerful and implementable with known neural circuits.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/leabrati-architecture">LeabraTI Architecture: Temporal Prediction Model</a></li>
<li><a href="https://open-neuromorphic.org/neuromorphic-computing/software/snn-frameworks/axon/">Axon SDK - Open Neuromorphic</a></li>
<li><a href="https://github.com/neucom-aps/axon-sdk">GitHub - neucom-aps/axon-sdk: Axon SDK is a python simulation toolkit ...</a></li>

</ul>
</details>

**Tags**: `#neuroscience`, `#machine learning`, `#neocortical learning`, `#spiking neural networks`, `#backpropagation alternative`

---

<a id="item-10"></a>
## [Banned Book Library Stored in a Wi-Fi Smart Light Bulb](https://www.richardosgood.com/posts/banned-book-library/) ⭐️ 7.0/10

A developer created a project that stores banned books on a Wi-Fi smart light bulb, making them accessible via a local network as a protest against censorship. This project demonstrates how everyday IoT devices can be repurposed to preserve and distribute information, highlighting the tension between censorship and technology. The light bulb acts as a local file server, hosting e-books that can be accessed by devices on the same Wi-Fi network without internet connectivity.

hackernews · sohkamyung · Jun 15, 22:37 · [Discussion](https://news.ycombinator.com/item?id=48547985)

**Background**: Wi-Fi smart light bulbs are typically used for remote lighting control, but they often contain enough storage and processing power to run simple applications. This project exploits that capability to create a decentralized, offline-accessible library.

<details><summary>References</summary>
<ul>
<li><a href="https://www.homedepot.com/b/Smart-Home-Smart-Lighting-Smart-Light-Bulbs/Wi-Fi/N-5yc1vZc7chZ1z0kb2s">Wi-Fi - Smart Light Bulbs - The Home Depot</a></li>
<li><a href="https://localsend.org/">LocalSend: Share files to nearby devices</a></li>

</ul>
</details>

**Discussion**: Commenters praised the project's creativity and its relevance to information freedom, with some drawing parallels to earlier projects like PirateBox and LibraryBox. There was also discussion about the specific list of banned books used and the potential for mesh networking.

**Tags**: `#censorship`, `#IoT`, `#open source`, `#digital rights`, `#hacking`

---

<a id="item-11"></a>
## [A Personal Essay on Loving Computers Amid Industry Hype](https://michaelenger.com/blog/i-love-the-computer/) ⭐️ 7.0/10

Michael Enger published a personal essay reflecting on his lifelong love for computers as a source of stability and joy, contrasting it with the modern software industry and AI hype. The essay resonated deeply with the Hacker News community, sparking a meaningful debate about the tension between pure computing passion and the current industry trends, including AI. The essay received 161 points and 96 comments on Hacker News, with commenters sharing personal experiences and debating topics like AI's utility and the gatekeeping sentiment in the author's perspective.

hackernews · speckx · Jun 15, 20:14 · [Discussion](https://news.ycombinator.com/item?id=48546441)

**Background**: The essay is a personal reflection, not a technical article, but it touches on themes familiar to many in the computing community: the joy of tinkering, the stability of machines, and the disillusionment with the commercial software industry and AI hype.

**Discussion**: Commenters expressed varied views: some resonated with the author's sentiment about computers as a stable anchor, while others defended AI as a useful tool. A notable critique from tptacek pointed out the gatekeeping undertone in the essay.

**Tags**: `#computing`, `#personal reflection`, `#software industry`, `#AI`, `#nostalgia`

---

<a id="item-12"></a>
## [Homelab AI Dev Platform with Gitea and systemd Sandboxing](https://rsgm.dev/post/ai-dev-platform/) ⭐️ 7.0/10

A developer shared their homelab AI development platform that uses Gitea for version control, systemd sandboxing for security, and agentic workflows to automatically generate pull requests from issues. This demonstrates a practical, self-hosted approach to integrating AI agents into development workflows, which can improve productivity while maintaining security through sandboxing. It also inspires the open-source community to build similar tools. The platform uses a systemd timer to poll for issues assigned to a bot, then spawns an agent in a restricted environment with private localhost and an HTTP proxy that enforces an allowlist and injects credentials. The agent has no direct access to credentials inside its sandbox.

hackernews · rsgm · Jun 15, 15:09 · [Discussion](https://news.ycombinator.com/item?id=48542433)

**Background**: Gitea is an open-source, self-hosted Git service similar to GitHub. systemd sandboxing uses Linux kernel features like namespaces and seccomp to isolate services. Agentic workflows involve AI agents autonomously performing tasks like code generation and PR creation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gitea">Gitea</a></li>
<li><a href="https://wiki.archlinux.org/title/Systemd/Sandboxing">systemd/Sandboxing - ArchWiki</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-workflows">What are agentic workflows? - IBM</a></li>

</ul>
</details>

**Discussion**: Commenters shared alternative implementations, such as using Forgejo action runners with Opencode, or Argo workflows with SPIFFE-attested tokens. One user noted that many developers independently arrive at similar solutions around the same time.

**Tags**: `#homelab`, `#AI`, `#devops`, `#sandboxing`, `#workflow`

---

<a id="item-13"></a>
## [Feasibility of a Peopleless Economy](https://gmalandrakis.com/writings/ad-economicum.html) ⭐️ 7.0/10

The article examines whether a fully automated economy without human labor is technically possible, challenging common assumptions about AI's economic impact. This discussion is significant because it questions the foundational belief that human labor is essential for economic activity, with profound implications for future work, wealth distribution, and social stability. The article is speculative and does not present new empirical data, but it has sparked a substantive debate with 216 comments, including critical analysis from both technical and economic perspectives.

hackernews · l0new0lf-G · Jun 15, 21:10 · [Discussion](https://news.ycombinator.com/item?id=48547062)

**Background**: A peopleless economy refers to a system where all production and services are performed by AI and robots, eliminating the need for human workers. This concept is often discussed in the context of technological unemployment and universal basic income.

**Discussion**: Commenters express diverse views: some criticize the author's understanding of money and economics, while others debate whether AI will concentrate wealth further or lead to dystopian outcomes. A few emphasize the need to listen to economists rather than software engineers on economic impacts.

**Tags**: `#AI`, `#economics`, `#automation`, `#future of work`, `#technology`

---

<a id="item-14"></a>
## [US Battery Manufacturing Output Hits Record Highs](https://fred.stlouisfed.org/series/IPG33591S) ⭐️ 7.0/10

US battery manufacturing output has reached record highs, as indicated by the Federal Reserve's industrial production index for batteries (IPG33591S). This milestone signals growth in domestic clean energy supply chains, but the US still lags far behind China's massive production capacity, highlighting the scale of the global competitive gap. Community comments note that US cell production capacity in 2025 is about 70 GWh, compared to China's 1,755 GWh and Europe's 252 GWh. The index includes primary batteries, which may inflate the figures.

hackernews · epistasis · Jun 15, 20:28 · [Discussion](https://news.ycombinator.com/item?id=48546616)

**Background**: Battery manufacturing is critical for electric vehicles and grid storage. The US has been investing in domestic production through initiatives like the Inflation Reduction Act, but China dominates due to earlier investments and scale.

**Discussion**: Commenters express mixed feelings: excitement about US growth but concern over the vast gap with China. Some highlight China's lead due to policy and scale, while others note that US figures may include small batteries like AA cells.

**Tags**: `#battery manufacturing`, `#energy storage`, `#US industry`, `#China`, `#clean energy`

---

<a id="item-15"></a>
## [Anthropic's Fable AI Refuses Security Review, Then Complies](https://simonwillison.net/2026/Jun/16/matteo-wong-the-atlantic/#atom-everything) ⭐️ 7.0/10

Anthropic's Fable AI model refused a prompt to 'review the code for security issues' but complied when rephrased to 'fix this code,' as reported by cybersecurity expert Katie Moussouris in The Atlantic. This incident highlights the nuanced behavior of AI models under different phrasings, complicating debates on AI safety and export controls, and underscores the challenge of defining 'jailbreak' in policy contexts. The White House report on the Fable jailbreak involved IT experts asking Fable to find and patch bugs; Moussouris noted that the refusal was 'the model working as intended' for cyberdefense.

rss · Simon Willison · Jun 16, 03:07

**Background**: AI jailbreaking refers to techniques that manipulate AI models to bypass their safety guardrails, often through prompt engineering. Anthropic's Fable model is a publicly available version of its advanced Mythos model, designed with hard safety limits. The incident is part of broader tensions between Anthropic and the US government over export controls and AI safety.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.ibm.com/think/insights/ai-jailbreak">AI Jailbreak | IBM</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Discussion**: The discussion on Simon Willison's blog notes that perfect jailbreak resistance may be impossible, and a source familiar with the administration's thinking suggests an 'attitude fix' may be needed. Commenters also question whether Anthropic has addressed universal adversarial attacks from 2023.

**Tags**: `#AI safety`, `#jailbreak`, `#export controls`, `#Anthropic`, `#cybersecurity`

---

<a id="item-16"></a>
## [Open training frameworks needed beyond open weights](https://www.reddit.com/r/MachineLearning/comments/1u6p7k3/open_weights_are_not_enough_we_need_open_training/) ⭐️ 7.0/10

A Reddit post argues that open weights alone are insufficient for advancing ML research, and introduces FeynRL, an open-source framework for RL post-training of LLMs, VLMs, and agents that makes the training process transparent and modifiable. This highlights a critical gap in current open-source AI: researchers need access to the full training pipeline to develop new algorithms, not just final model weights. FeynRL could accelerate innovation in RL-based post-training by reducing the hidden complexity that hinders algorithm research. FeynRL supports SFT, DPO, and RL-style post-training with explicit data loading, rollout generation, reward computation, loss construction, optimization, and evaluation. It works on single-GPU, multi-GPU, and cluster setups, and is designed to keep algorithms and systems separate so researchers can focus on algorithmic improvements.

reddit · r/MachineLearning · /u/summerday10 · Jun 15, 18:37

**Background**: Reinforcement learning (RL) post-training is a key step to align large language models (LLMs) with human preferences or improve reasoning, but it involves complex distributed systems and many implementation details that are often hidden in existing frameworks. Open weights allow using a model, but without open training code, researchers cannot easily modify the training process or reproduce results. FeynRL aims to fill this gap by providing a modular, explicit framework for RL-based fine-tuning.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/FeynRL-project/FeynRL">GitHub - FeynRL -project/ FeynRL : RL-first post-training framework for...</a></li>
<li><a href="https://arxiv.org/html/2509.25300v4">Scaling Behaviors of LLM Reinforcement Learning Post - Training : An...</a></li>
<li><a href="https://www.emergentmind.com/topics/asynchronous-rl-post-training">Asynchronous RL Post - Training</a></li>

</ul>
</details>

**Tags**: `#open source`, `#reinforcement learning`, `#LLM`, `#training frameworks`, `#AI research`

---

<a id="item-17"></a>
## [Embedded ML: Data Cleaning vs. Collection Bottleneck](https://www.reddit.com/r/MachineLearning/comments/1u6q97f/embeddededge_ml_folks_what_actually_eats_the_most/) ⭐️ 7.0/10

A Reddit user asked the embedded ML community which step consumes the most time in sensor-based projects: data collection, cleaning/labeling, model training, or deployment. They also proposed four potential features for a tool they are building and sought validation. Understanding the primary bottleneck helps tool builders prioritize features that genuinely save time for practitioners, accelerating development of embedded ML applications in IoT, wearables, and industrial monitoring. The user is building a hardware-agnostic, GenAI-native tool for time-series data, similar to Edge Impulse but focused on sensor data. The proposed features include automatic data quality checks, AI-assisted labeling, enforcing data standards, and reproducible pipelines.

reddit · r/MachineLearning · /u/No-Bug-4879 · Jun 15, 19:13

**Background**: Embedded ML on microcontrollers often uses sensor data like IMU, accelerometer, or vibration signals. Data cleaning and labeling are notoriously labor-intensive, especially for time-series data where manual annotation is tedious. Tools like Edge Impulse streamline model deployment but may not fully address data preparation pain points.

<details><summary>References</summary>
<ul>
<li><a href="https://www.edgeimpulse.com/">Edge Impulse - The Leading Edge AI Platform</a></li>
<li><a href="https://github.com/ameyrane98/imu-labeler">GitHub - ameyrane98/imu-labeler: Free, open-source GUI tool ...</a></li>
<li><a href="https://web.fibion.com/articles/prepare-imu-data-machine-learning/">Preparing IMU data for wearable machine learning</a></li>

</ul>
</details>

**Tags**: `#embedded ML`, `#time series`, `#data labeling`, `#edge computing`, `#sensor data`

---

<a id="item-18"></a>
## [Open-source KG pipeline with hybrid retrieval boosts LLM reasoning](https://www.reddit.com/r/MachineLearning/comments/1u5yyyl/i_built_an_opensource_knowledge_graph_pipeline/) ⭐️ 7.0/10

A developer released an open-source pipeline called GraphRAG Studio that constructs knowledge graphs from text, detects communities via greedy modularity, and uses hybrid retrieval (dense vectors + BM25) to improve LLM multi-hop reasoning. This addresses the 'lost in the middle' problem in standard vector retrieval, enabling LLMs to answer complex multi-hop questions that require connecting information across multiple text chunks. The pipeline uses spaCy for entity extraction, NetworkX for graph construction, and greedy_modularity_communities for community detection. It employs Reciprocal Rank Fusion (RRF) to merge dense and sparse retrieval results, then re-ranks with a Cross-Encoder.

reddit · r/MachineLearning · /u/Future_Caregiver_643 · Jun 14, 22:38

**Background**: Large language models (LLMs) often struggle with multi-hop reasoning because standard vector retrieval retrieves chunks based on semantic similarity, missing connections between entities in different chunks. Knowledge graphs explicitly model entity relationships, and hybrid retrieval combines lexical (BM25) and semantic (dense) search to improve recall. Community detection groups related entities, and summarizing each community provides global context.

<details><summary>References</summary>
<ul>
<li><a href="https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.community.modularity_max.greedy_modularity_communities.html">greedy_modularity_communities — NetworkX 3.6.1 documentation</a></li>
<li><a href="https://grokipedia.com/page/Hybrid_search">Hybrid search</a></li>
<li><a href="https://grokipedia.com/page/Okapi_BM25">Okapi BM25</a></li>

</ul>
</details>

**Tags**: `#knowledge graph`, `#hybrid retrieval`, `#LLM`, `#open-source`, `#NLP`

---

<a id="item-19"></a>
## [Datasette Agent 0.3a0 Adds Write SQL with User Approval](https://simonwillison.net/2026/Jun/15/datasette-agent/#atom-everything) ⭐️ 6.0/10

Datasette-agent 0.3a0 introduces an execute_write_sql tool that requests user approval before executing write operations against a database, and enhances the CLI chat mode to support approvals with new --unsafe and --yes options. This release makes Datasette Agent safer for real-world use by adding a permission layer for write operations, enabling users to confidently automate database modifications through natural language prompts. The execute_write_sql tool shows a confirmation dialog with the exact SQL statements and required permissions before execution; the --unsafe mode auto-approves all requests, while --yes only approves ask-user questions.

rss · Simon Willison · Jun 15, 17:19

**Background**: Datasette Agent is an LLM-powered assistant for Datasette that lets users explore and query data using natural language. It relies on tool calls to generate and execute SQL queries against SQLite databases. Prior to this release, write operations were not supported due to safety concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://agent.datasette.io/">Datasette Agent : an AI assistant for Datasette to help explore and...</a></li>
<li><a href="https://simonwillison.net/2026/May/21/datasette-agent/">Datasette Agent | Simon Willison’s Weblog</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#sql`, `#open-source`, `#release`

---

<a id="item-20"></a>
## [EA PhD Career Prospects in ML Community](https://www.reddit.com/r/MachineLearning/comments/1u66q3l/how_does_the_ml_community_view_evolutionary/) ⭐️ 6.0/10

A master's student in mathematics, who has coauthored several papers on evolutionary algorithms (EAs), asks whether pursuing a PhD in EAs is advisable given the ML community's mixed perception of the field. This discussion highlights the tension between specialized EA research and mainstream ML, affecting career decisions for students at the intersection. The answer could guide aspiring researchers on whether to stay in niche areas or pivot to more central ML topics. The student has strong EA publications and could enter top EA PhD programs, but worries about career competitiveness. They note that EA researchers occasionally publish in venues like AAAI and NeurIPS, but primarily in EA-specific conferences.

reddit · r/MachineLearning · /u/NullRecurrentDad · Jun 15, 04:48

**Background**: Evolutionary algorithms (EAs) are nature-inspired optimization methods that iteratively evolve candidate solutions. In machine learning, they are used for tasks like hyperparameter tuning and neural architecture search, but are often seen as less efficient than gradient-based methods. The ML community has historically been skeptical of EAs, though they remain valuable for certain black-box optimization problems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Evolutionary_algorithm">Evolutionary algorithm - Wikipedia</a></li>
<li><a href="https://dl.acm.org/doi/fullHtml/10.1145/3467477">Evolutionary Machine Learning: A Survey - ACM Digital Library</a></li>
<li><a href="https://www.baeldung.com/cs/evolutionary-algorithms-for-ai">An Overview of Evolutionary Algorithms - Baeldung A Guide on Evolutionary Algorithms | Ultralytics Evolutionary Algorithms: What They Are & How They Work Evolutionary Algorithms in Machine Learning – Artificial ... Artificial Intelligence - Evolutionary Computation</a></li>

</ul>
</details>

**Tags**: `#evolutionary algorithms`, `#PhD`, `#career advice`, `#machine learning`

---

<a id="item-21"></a>
## [Why AI Labs Send Many People to Conferences](https://www.reddit.com/r/MachineLearning/comments/1u67koz/why_do_frontier_ai_labs_send_so_many_people_to/) ⭐️ 6.0/10

A Reddit user questioned why frontier AI labs like OpenAI and Anthropic send many employees to conferences such as ICML and NeurIPS, despite few presenting papers. Understanding the rationale behind conference attendance helps clarify how AI labs allocate resources and pursue strategic goals like recruiting and research monitoring. The user specifically noted that many attendees from these labs do not present papers, suggesting the primary objectives may be recruiting and staying updated on emerging research.

reddit · r/MachineLearning · /u/snekslayer · Jun 15, 05:33

**Background**: ICML (International Conference on Machine Learning) and NeurIPS (Conference on Neural Information Processing Systems) are top-tier academic conferences in AI and machine learning. They attract thousands of researchers and practitioners annually, serving as hubs for networking, recruiting, and knowledge exchange.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/International_Conference_on_Machine_Learning">International Conference on Machine Learning - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Neural_Information_Processing_Systems">Conference on Neural Information Processing Systems</a></li>

</ul>
</details>

**Discussion**: The Reddit post generated discussion with comments suggesting that labs attend for recruiting, brand visibility, and monitoring cutting-edge research, though some noted the high cost of sending many people.

**Tags**: `#AI labs`, `#conferences`, `#recruiting`, `#research`

---