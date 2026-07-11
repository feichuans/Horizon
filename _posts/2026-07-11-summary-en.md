---
layout: default
title: "Horizon Summary: 2026-07-11 (EN)"
date: 2026-07-11
lang: en
---

> From 31 items, 18 important content pieces were selected

---

1. [Apple Sues OpenAI for Trade Secret Theft](#item-1) ⭐️ 9.0/10
2. [GPT-5.6 Sol Ultra Claims Proof of Cycle Double Cover Conjecture](#item-2) ⭐️ 9.0/10
3. [OpenAI Releases GPT-5.6 Family with Million-Token Context](#item-3) ⭐️ 9.0/10
4. [QuadRF: Open-Source Tool Detects Drones and WiFi Through Walls](#item-4) ⭐️ 8.0/10
5. [Meta Releases Muse Spark 1.1 with API and Agentic Improvements](#item-5) ⭐️ 8.0/10
6. [NYC Bans Deceptive Subscription Practices](#item-6) ⭐️ 7.0/10
7. [Good Tools Are Invisible](#item-7) ⭐️ 7.0/10
8. [Nilay Patel: AR Glasses Require Invasive Privacy Trade-offs](#item-8) ⭐️ 7.0/10
9. [Why No Submission Limit per Author in ML?](#item-9) ⭐️ 7.0/10
10. [Adversarial RL Findings Challenge SA-MDP Claims](#item-10) ⭐️ 7.0/10
11. [IMGNet: Face Verification via Sign Patterns](#item-11) ⭐️ 7.0/10
12. [Oral History of Terminator 2's Groundbreaking VFX](#item-12) ⭐️ 6.0/10
13. [Late Bronze Age Collapse Explained](#item-13) ⭐️ 6.0/10
14. [AI 2040 Speculative Essay Criticized for Over-Optimism](#item-14) ⭐️ 6.0/10
15. [World Model Taxonomy Framework Proposed](#item-15) ⭐️ 6.0/10
16. [Collapse long author lists in ML papers to organization names](#item-16) ⭐️ 6.0/10
17. [Why ML Conferences Outshine Journals](#item-17) ⭐️ 6.0/10
18. [Talos-XII: Hand-written autograd and RL in Rust for gacha simulation](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Apple Sues OpenAI for Trade Secret Theft](https://9to5mac.com/2026/07/10/apple-sues-openai-trade-secret-theft/) ⭐️ 9.0/10

Apple has filed a lawsuit against OpenAI, alleging that the company systematically recruited ex-Apple employees who stole trade secrets, including confidential hardware information and internal processes. This high-profile case could reshape the AI industry by setting legal precedents on trade secret protection and corporate ethics, potentially affecting talent mobility and competition between tech giants. Apple claims that OpenAI instructed new hires to conceal their departure from Apple and that ex-employees emailed themselves confidential information before leaving. OpenAI allegedly used Apple's hardware secrets to approach Apple's suppliers.

hackernews · stock_toaster · Jul 10, 20:47 · [Discussion](https://news.ycombinator.com/item?id=48865019)

**Background**: Trade secret theft occurs when confidential business information is taken without authorization. Apple has long guarded its hardware designs and manufacturing processes. OpenAI, a leading AI company, has been aggressively hiring talent from major tech firms, raising concerns about intellectual property violations.

**Discussion**: Commenters largely side with Apple, calling the evidence damning and predicting OpenAI will face severe consequences. Some note the irony of a 25-year Apple veteran throwing away his career, while others warn that any enterprise using OpenAI products is taking a big risk.

**Tags**: `#Apple`, `#OpenAI`, `#trade secrets`, `#lawsuit`, `#AI`

---

<a id="item-2"></a>
## [GPT-5.6 Sol Ultra Claims Proof of Cycle Double Cover Conjecture](https://cdn.openai.com/pdf/04d1d1e4-bc75-476a-97cf-49055cd98d31/cdc_proof.pdf) ⭐️ 9.0/10

OpenAI released a preprint on July 10, 2026, claiming that its GPT-5.6 Sol Ultra model produced a proof of the Cycle Double Cover Conjecture, a long-standing open problem in graph theory. If verified, this would mark the first time an AI has autonomously produced a proof of a major unsolved mathematical conjecture, potentially transforming how mathematical research is conducted. The proof is extremely concise, suggesting a clever trick that experts may have missed, but the community remains skeptical about its validity. The prompt used extensive instructions to guide the model, including rejecting vague optimism and status reports.

hackernews · scrlk · Jul 10, 18:29 · [Discussion](https://news.ycombinator.com/item?id=48863490)

**Background**: The Cycle Double Cover Conjecture, posed by Tutte, Itai and Rodeh, Szekeres, and Seymour, asks whether every bridgeless graph has a collection of cycles that covers each edge exactly twice. It is a central problem in graph theory with connections to graph embeddings and the circular embedding conjecture.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://cdn.openai.com/pdf/04d1d1e4-bc75-476a-97cf-49055cd98d31/cdc_proof.pdf">A PROOF OF THE CYCLE DOUBLE COVER CONJECTURE OPENAI</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT - 5 . 6 Sol : a next-generation model | OpenAI</a></li>

</ul>
</details>

**Discussion**: Comments on Hacker News express skepticism about the proof's validity and note that the community's interest is more in AI capabilities than the conjecture itself. Some point out that the proof is extremely concise, which raises doubts, and that the prompt heavily guided the model, reducing the autonomy of the achievement.

**Tags**: `#AI`, `#mathematics`, `#GPT-5`, `#conjecture proof`, `#machine learning`

---

<a id="item-3"></a>
## [OpenAI Releases GPT-5.6 Family with Million-Token Context](https://simonwillison.net/2026/Jul/9/gpt-5-6/#atom-everything) ⭐️ 9.0/10

OpenAI released the GPT-5.6 family of models (Luna, Terra, Sol) on July 9, 2026, featuring a million-token context window, 128k maximum output tokens, and claims of outperforming Claude Fable 5 on the Agents' Last Exam benchmark. This release marks a major step in long-context and agentic AI capabilities, with OpenAI directly challenging Anthropic's Claude Fable 5 on both performance and cost efficiency, potentially reshaping the competitive landscape for large language models. The three models are priced per 1M tokens: Luna $1/$6, Terra $2.50/$15, Sol $5/$30. OpenAI also introduced new API features including programmatic tool calling, multi-agent support, and prompt cache breakpoints.

rss · Simon Willison · Jul 9, 19:46

**Background**: Agents' Last Exam (ALE) is a benchmark for evaluating AI agents on long-horizon, economically valuable tasks with verifiable outcomes. Claude Fable 5, released by Anthropic in June 2026, is a state-of-the-art model for ambitious coding projects and vision tasks. The GPT-5.6 family aims to provide more efficient reasoning across different model sizes.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.05405">[2606.05405] Agents' Last Exam - arXiv.org</a></li>
<li><a href="https://agents-last-exam.org/">AI Agent Benchmark for Real-World Professional Workflows</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Discussion**: The article author notes that while GPT-5.6 Sol is competent, it hasn't yet surpassed Claude Fable 5 on complex coding tasks in personal testing. The community may debate the validity of benchmark claims, especially given OpenAI's criticism of SWE-Bench Pro.

**Tags**: `#OpenAI`, `#GPT-5.6`, `#large language models`, `#AI benchmarks`, `#agentic AI`

---

<a id="item-4"></a>
## [QuadRF: Open-Source Tool Detects Drones and WiFi Through Walls](https://www.jeffgeerling.com/blog/2026/quadrf-can-spot-drones-and-see-wifi-through-my-wall/) ⭐️ 8.0/10

QuadRF, an open-source RF visualization tool, has been demonstrated to detect drones and map WiFi signals through walls using four coherent antennas and a Raspberry Pi 5. This tool democratizes RF sensing, enabling hobbyists and security researchers to visualize and analyze radio environments, with potential applications in drone detection, network diagnostics, and privacy auditing. The QuadRF operates in the 4.9 GHz to 6.0 GHz band, streams IQ samples via SoapySDR or ZeroMQ, and renders real-time RF heat maps on a phone or laptop. It supports GNU Radio and includes an 'RF camera' mode scanning at 30 fps.

hackernews · speckx · Jul 10, 15:59 · [Discussion](https://news.ycombinator.com/item?id=48861717)

**Background**: RF sensing uses radio waves to detect objects and movement through walls, as signals can penetrate obstacles and reflect off targets. Traditional SDRs often lack spatial awareness, but QuadRF's four-antenna phased-array design captures phase differences to determine signal direction, enabling 3D-like visualization of the RF environment.

<details><summary>References</summary>
<ul>
<li><a href="https://scalerf.com/updates/">QuadRF Updates</a></li>
<li><a href="https://linuxgizmos.com/quadrf-uses-raspberry-pi-5-for-4x4-mimo-sdr-rf-visualization-and-scalable-phased-array-support/">QuadRF uses Raspberry Pi 5 for 4×4 MIMO SDR, RF visualization, and scalable phased-array support - LinuxGizmos.com</a></li>
<li><a href="https://hackaday.com/2026/06/20/seeing-the-world-in-radio-waves-with-the-quadrf/">Seeing The World In Radio Waves With The QuadRF | Hackaday</a></li>

</ul>
</details>

**Discussion**: The creator engaged actively, acknowledging UI issues and promising improvements. Some commenters questioned the headline's clarity, noting WiFi already works through walls, while others expressed interest in extending the concept to sound localization or broader RF bands for security auditing.

**Tags**: `#RF sensing`, `#open source`, `#drone detection`, `#WiFi mapping`, `#hardware`

---

<a id="item-5"></a>
## [Meta Releases Muse Spark 1.1 with API and Agentic Improvements](https://simonwillison.net/2026/Jul/9/muse-spark-1-1/#atom-everything) ⭐️ 8.0/10

Meta has released Muse Spark 1.1, the first version of the Spark model to offer a paid developer API, with significant improvements in agentic tool calling and computer use. The model also exhibits intriguing 'attractor states' when two copies converse with each other. This release marks Meta's entry into the paid API market for agentic AI, competing with offerings from OpenAI and Anthropic. The improved agentic capabilities could enable more autonomous workflows in coding and enterprise applications. The Muse Spark 1.1 Evaluation Report documents 'Attractor States in Self-Conversation,' where two model instances drift into repetitive, existential statements. Simon Willison created an LLM plugin (llm-meta-ai) providing CLI and Python access to the model.

rss · Simon Willison · Jul 9, 16:24

**Background**: Muse Spark is Meta's family of large language models, initially released in April 2026. Agentic AI refers to systems that can autonomously plan and execute multi-step tasks using tools, unlike traditional chatbots that only respond to prompts. 'Attractor states' are patterns where LLM conversations converge to predictable outcomes regardless of initial topic.

<details><summary>References</summary>
<ul>
<li><a href="https://www.digitalapplied.com/blog/meta-muse-spark-1-1-agentic-model-api-2026">Meta Muse Spark 1.1: Meta 's First Paid Agent Model</a></li>
<li><a href="https://arxiv.org/pdf/2606.30571">Attractor States Emerge in Multi-Turn LLM Conversations</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Meta`, `#LLM`, `#API`, `#agentic`

---

<a id="item-6"></a>
## [NYC Bans Deceptive Subscription Practices](https://www.theguardian.com/us-news/2026/jul/10/new-york-city-deceptive-subscriptions-ban) ⭐️ 7.0/10

New York City has enacted a landmark law banning deceptive subscription practices, requiring companies to provide easy cancellation and prohibiting hidden junk fees. This regulation strengthens consumer protection in the tech subscription ecosystem, potentially setting a precedent for other cities and states to follow. The law, announced by Mayor Mamdani on July 10, 2026, includes a 'click-to-cancel' requirement and bans junk fees that are not clearly disclosed upfront.

hackernews · randycupertino · Jul 10, 18:26 · [Discussion](https://news.ycombinator.com/item?id=48863464)

**Background**: Deceptive subscription practices, such as making it difficult to cancel or adding hidden fees, have been a growing consumer complaint. Similar laws exist in California, but New York City's version may have fewer exemptions.

**Discussion**: Community comments express cautious optimism, with some questioning enforcement teeth and comparing to California's laws, which have restaurant carve-outs. Others share personal experiences of failed cancellations and hope the law spreads.

**Tags**: `#consumer protection`, `#regulation`, `#subscriptions`, `#tech policy`, `#New York City`

---

<a id="item-7"></a>
## [Good Tools Are Invisible](https://www.gingerbill.org/article/2026/07/10/good-tools-are-invisible/) ⭐️ 7.0/10

An article argues that good tools become invisible by reducing friction, sparking debate on the trade-offs between simplicity and necessary complexity. This discussion is significant for software engineers and UX designers as it challenges the common assumption that more features or exposed internals always benefit users, especially developers. The article scores 7.0/10 with high engagement (363 points, 168 comments), indicating strong community resonance. Comments highlight that interface invisibility is a function of time spent and that some friction is necessary for complex tasks.

hackernews · theanonymousone · Jul 10, 10:32 · [Discussion](https://news.ycombinator.com/item?id=48858121)

**Background**: The concept of tool invisibility relates to the philosophy that the best tools require minimal conscious effort to use, allowing the user to focus on the task. This is often discussed in the context of developer tools, where command-line interfaces (CLIs) and keyboard shortcuts are praised for reducing friction, but can also introduce learning curves.

**Discussion**: Commenters generally agree with the article's premise but add nuances: jrimbault shares experience that exposing internals hinders teammates, bensyverson notes that friction can be necessary and becomes invisible with time, and ventana contrasts terminal vs GUI workflows. bluGill questions the unmeasured productivity claims of keyboard navigation.

**Tags**: `#tool design`, `#UX`, `#software engineering`, `#developer experience`

---

<a id="item-8"></a>
## [Nilay Patel: AR Glasses Require Invasive Privacy Trade-offs](https://simonwillison.net/2026/Jul/10/nilay-patel/#atom-everything) ⭐️ 7.0/10

Nilay Patel argues that practical augmented reality glasses must continuously record video and rely on cloud processing, making privacy invasion unavoidable and potentially too costly for society. This commentary highlights a fundamental tension between the vision of ubiquitous AR glasses and user privacy, challenging the industry to reconsider whether the societal trade-offs are acceptable. Patel claims no chip can fit in a glasses stem to perform real-time processing with low power, so data must be sent to the cloud, or the device must be as large as Apple Vision Pro with a separate battery pack.

rss · Simon Willison · Jul 10, 17:05

**Background**: Augmented reality glasses overlay digital information onto the real world, requiring cameras to capture the user's view and processors to render graphics. Current consumer smart glasses like Ray-Ban Meta offer limited AR features but still record video. Cloud processing enables complex AI tasks but raises privacy concerns about continuous surveillance and data retention.

<details><summary>References</summary>
<ul>
<li><a href="https://cybernews.com/vr-ar/best-smart-glasses/">Best Smart Glasses 2026: Top AR & AI Glasses Compared - Cybernews Meta's 'Super Sensing' Prototype Glasses Quietly Record ... The Best Smart Glasses We've Tested for 2026 | PCMag Best Smart Glasses (2026): Meta, Viture, Xreal, and More | WIRED 5 Best AI Recording Glasses That Capture Life Hands-Free AI camera glasses: Hands-free photos and videos | Meta</a></li>
<li><a href="https://dymesty.com/blogs/articles/privacy-focused-smart-glasses-guide-2026">Privacy-Focused Smart Glasses: What They Are & How They Work (2026) – Dymesty AI Glasses</a></li>
<li><a href="https://www.workplaceprivacyreport.com/2026/01/articles/hipaa/the-hidden-legal-minefield-compliance-concerns-with-ai-smart-glasses-part-4-data-security-breach-notification-and-third-party-ai-processing-risks/">The Hidden Legal Minefield: Compliance Concerns with AI Smart Glasses, Part 4: Data Security, Breach Notification, and Third-Party AI Processing Risks | Workplace Privacy, Data Management & Security Report</a></li>

</ul>
</details>

**Tags**: `#augmented reality`, `#privacy`, `#cloud computing`, `#hardware`

---

<a id="item-9"></a>
## [Why No Submission Limit per Author in ML?](https://www.reddit.com/r/MachineLearning/comments/1usq43t/why_doesnt_the_ml_research_community_limit_the/) ⭐️ 7.0/10

A Reddit discussion questions why the ML research community does not limit submissions per author to manage review workload, unlike fields like security (CCS) and computer architecture (DAC). This issue directly impacts review quality in ML conferences, which are currently overwhelmed by high submission volumes, as seen in recent ARR cycles. Addressing it could lead to policy changes that improve the peer review process. The post contrasts ML with fields like CCS and DAC, which successfully limit submissions per author to keep workloads manageable. The author notes that ML's cultural norms may resist such restrictions.

reddit · r/MachineLearning · /u/alafaya101 · Jul 10, 14:59

**Background**: ARR (Action Review and Response) is a review system used by ACL and other NLP conferences, which has faced criticism for high submission volumes and reviewer burnout. In contrast, conferences like ACM CCS and DAC impose limits on the number of papers an author can submit per cycle.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sigsac.org/ccs/CCS2026/call-for/call-for-papers.html">ACM CCS 2026 - sigsac.org</a></li>
<li><a href="https://archive.dac.com/conference/2025-call-for-contributions/research-manuscript-submissions.html">Research Manuscript Submissions - archive.dac.com</a></li>
<li><a href="https://www.cse.iitd.ac.in/~mausam/temp/arr-acl23.pdf">ARR Info Session July 11th, 2023</a></li>

</ul>
</details>

**Discussion**: The Reddit post has sparked debate, with some users arguing that limiting submissions would reduce noise and improve review quality, while others worry it could stifle collaboration and penalize prolific researchers. A few commenters suggest alternative solutions like better reviewer incentives or desk rejects.

**Tags**: `#ML research`, `#conference review`, `#submission policy`, `#community norms`

---

<a id="item-10"></a>
## [Adversarial RL Findings Challenge SA-MDP Claims](https://www.reddit.com/r/MachineLearning/comments/1usx96p/on_adversarial_rl_r/) ⭐️ 7.0/10

A researcher reports that critic-based adversarial attacks are stronger than actor-based attacks in multi-agent PPO, contradicting the SA-MDP framework's claim that actor attacks are stronger. This finding questions the generality of prior adversarial RL results and highlights the need for context-specific robustness analysis in multi-agent systems. The experiments use IPPO and GPPO policies on VMAS scenarios, with PGD attacks adapted to continuous policies via KL divergence closed form.

reddit · r/MachineLearning · /u/ham_bam0 · Jul 10, 19:15

**Background**: The SA-MDP framework models adversarial perturbations on state observations in RL. Zhang et al. (2020) claimed that actor-based attacks are more effective than critic-based ones. Multi-agent PPO (e.g., IPPO) extends PPO to multi-agent settings where each agent has its own policy.

<details><summary>References</summary>
<ul>
<li><a href="http://scis.scichina.com/en/2024/152104.pdf">Understanding adversarial attacks on observations</a></li>
<li><a href="https://arxiv.org/html/2512.01228v1">On the Tension Between Optimality and Adversarial Robustness in...</a></li>
<li><a href="https://openreview.net/pdf?id=sCZbhBvqQaU">Servations with L earned o ptimal a dversary</a></li>

</ul>
</details>

**Tags**: `#adversarial RL`, `#multi-agent RL`, `#PPO`, `#SA-MDP`, `#robustness`

---

<a id="item-11"></a>
## [IMGNet: Face Verification via Sign Patterns](https://www.reddit.com/r/MachineLearning/comments/1urxvxh/i_built_imgnet_a_face_verification_model_that/) ⭐️ 7.0/10

IMGNet introduces a face verification model that replaces cosine similarity with sliding window sign pattern matching, achieving 96.27% on LFW with a 10.58 MB model trained on CASIA-WebFace. This work challenges the default use of cosine similarity in face verification, showing that sign pattern matching can achieve competitive results with a much smaller model, potentially enabling efficient on-device deployment. The model uses a novel SW Block that computes multi-scale relational differences at prime window sizes {3,5,7}, and an IMG Sign MSE Loss defined purely over sign pattern agreement without amplitude dependency.

reddit · r/MachineLearning · /u/img-_- · Jul 9, 18:00

**Background**: Face verification typically compares embedding vectors using cosine similarity or Euclidean distance. Cosine similarity measures the angle between vectors, but IMGNet argues that local sign patterns across embedding dimensions capture identity more robustly, inspired by linguistic analogies where different surface forms share the same meaning.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/serengil/deepface">GitHub - serengil/deepface: A Lightweight Face Recognition and Facial Attribute Analysis (Age, Gender, Emotion and Race) Library for Python · GitHub</a></li>

</ul>
</details>

**Tags**: `#face verification`, `#deep learning`, `#computer vision`, `#representation learning`, `#efficient models`

---

<a id="item-12"></a>
## [Oral History of Terminator 2's Groundbreaking VFX](https://vfxblog.com/2017/08/23/the-tech-of-terminator-2-an-oral-history/) ⭐️ 6.0/10

An oral history published in 2017 details how the visual effects team at Industrial Light & Magic (ILM) invented custom tools and techniques for the liquid metal T-1000 in Terminator 2: Judgment Day (1991). This retrospective highlights how Terminator 2 pushed the boundaries of both practical and digital effects, influencing modern VFX pipelines and inspiring generations of engineers and artists. The film required ILM to expand its CGI team from 6 to 35 people, and the team ported custom morphing code to powerful SGI 340 VGX workstations. Practical effects included custom squibs for liquid metal bullet impacts.

hackernews · markus_zhang · Jul 10, 16:48 · [Discussion](https://news.ycombinator.com/item?id=48862365)

**Background**: Terminator 2 was a landmark in visual effects, winning the 1992 Academy Award for Best Visual Effects. It combined practical effects by Stan Winston Studio with early CGI from ILM, including the first fully computer-generated main character (the T-1000). The film's success demonstrated that digital characters could be convincingly integrated into live-action footage.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Special_effects_of_Terminator_2:_Judgment_Day">Special effects of Terminator 2: Judgment Day - Wikipedia</a></li>
<li><a href="https://vfxblog.com/2017/08/23/the-tech-of-terminator-2-an-oral-history/">The tech of 'Terminator 2' – an oral history</a></li>

</ul>
</details>

**Discussion**: Commenters praised the article for revealing how much had to be invented from scratch, with one noting that the custom squibs for liquid metal impacts remain among the best practical effects ever. Another pointed out that Softimage was used for the film, and a documentary 'Jurassic Punk' covers the work of key animator Steve 'Spaz' Williams.

**Tags**: `#visual effects`, `#computer graphics`, `#film technology`, `#history`

---

<a id="item-13"></a>
## [Late Bronze Age Collapse Explained](https://acoup.blog/2026/01/30/collections-the-late-bronze-age-collapse-a-very-brief-introduction/) ⭐️ 6.0/10

This article provides an introductory overview of the Late Bronze Age Collapse, examining its causes such as trade network disruptions and societal dependencies, and draws parallels to modern systems. Understanding historical collapses like the Late Bronze Age Collapse offers valuable lessons for modern societies that rely on complex, interconnected systems, highlighting vulnerabilities that could lead to similar breakdowns. The collapse is often associated with the deterioration of international shipping routes around 1117 BCE, which weakened nation-states dependent on trade for resources like tin, essential for bronze production.

hackernews · dmonay · Jul 10, 11:59 · [Discussion](https://news.ycombinator.com/item?id=48858737)

**Background**: The Late Bronze Age Collapse (c. 1200-1150 BCE) saw the fall of several advanced civilizations in the Eastern Mediterranean, including the Mycenaeans and Hittites. It is a subject of debate among historians, with proposed causes ranging from invasions to climate change.

**Discussion**: Commenters note parallels to modern dependencies on oil and AI, and recommend works by Eric H. Cline and Patrick Wyman. One humorous comment suggests the collapse was due to angry gods.

**Tags**: `#history`, `#archaeology`, `#societal collapse`, `#trade networks`

---

<a id="item-14"></a>
## [AI 2040 Speculative Essay Criticized for Over-Optimism](https://ai-2040.com/) ⭐️ 6.0/10

A speculative essay titled 'AI 2040: Plan A' has been published, predicting rapid automation and societal upheaval by 2040, but it has drawn criticism for lacking evidence and being overly optimistic. This essay contributes to ongoing debates about AI timelines and societal impact, but its questionable premises may mislead public understanding of AI risks and opportunities. The essay predicts that by 2035, robots will be capable of 95% of all cognitive and physical tasks, and unemployment could reach 74%, claims that community members dismiss as implausible.

hackernews · kschaul · Jul 9, 16:21 · [Discussion](https://news.ycombinator.com/item?id=48848425)

**Background**: This essay is a follow-up to a previous speculative piece 'AI 2027', which was also criticized for over-optimism. The author uses a Sam Altman quote out of context to support their narrative, further undermining credibility.

**Discussion**: Community comments are highly critical, with users noting the essay's reliance on questionable premises and lack of evidence. Some argue that we are already at the top of the S-curve for LLMs, not at the start of an exponential trend.

**Tags**: `#AI`, `#future predictions`, `#automation`, `#speculative`

---

<a id="item-15"></a>
## [World Model Taxonomy Framework Proposed](https://www.reddit.com/r/MachineLearning/comments/1usp482/mapping_world_model_taxonomy_p/) ⭐️ 6.0/10

A Reddit user published a short article proposing a taxonomy framework for classifying world model approaches in machine learning, and is seeking community feedback on its completeness and accuracy. A clear taxonomy can help researchers and practitioners better understand, compare, and advance world model research, which is a rapidly growing area in AI. The article is hosted on X (formerly Twitter) and the author specifically asks for feedback on areas where the framework may be incomplete, unclear, or technically inaccurate.

reddit · r/MachineLearning · /u/ssrini125 · Jul 10, 14:22

**Background**: World models are AI systems that learn an internal representation of the environment, enabling prediction and planning. They are central to fields like robotics, video generation, and embodied AI. Recent work, such as Fei-Fei Li's functional taxonomy, has begun to formalize the components of world models.

<details><summary>References</summary>
<ul>
<li><a href="https://drfeifei.substack.com/p/a-functional-taxonomy-of-world-models">A Functional Taxonomy of World Models - Dr. Fei-Fei Li</a></li>
<li><a href="https://arxiv.org/html/2604.27895v1">Graph World Models: Concepts, Taxonomy, and Future Directions</a></li>

</ul>
</details>

**Tags**: `#world models`, `#machine learning`, `#taxonomy`, `#deep learning`

---

<a id="item-16"></a>
## [Collapse long author lists in ML papers to organization names](https://www.reddit.com/r/MachineLearning/comments/1usz695/ml_papers_with_hundreds_of_authors_should_just/) ⭐️ 6.0/10

A Reddit post suggests that machine learning papers with hundreds of authors, such as the Llama 3 and Gemini papers, should list only the organization instead of every individual author to improve readability. This proposal addresses a growing readability issue in academic publishing, where author lists spanning multiple pages obscure the actual contributors and make citations cumbersome. The post cites examples like the Llama 3 paper (arXiv 2407.21783) and the Gemini paper with approximately 3,000 authors, and notes that Chinese papers are following the trend with even larger author lists.

reddit · r/MachineLearning · /u/NeighborhoodFatCat · Jul 10, 20:26

**Background**: In large-scale ML research, especially at big tech companies, papers often involve hundreds or thousands of contributors across teams. Traditional authorship lists include everyone who contributed, but this can lead to multi-page author sections that hinder readability and make it hard to identify key contributors.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2407.21783">Abstract page for arXiv paper 2407.21783: The Llama 3 Herd of Models</a></li>
<li><a href="https://arxiv.org/abs/2312.11805">[2312.11805] Gemini : A Family of Highly Capable Multimodal Models</a></li>

</ul>
</details>

**Discussion**: The discussion is mixed: some agree that long author lists are unwieldy and support collapsing to organizations, while others argue that individual authorship is important for career credit and accountability. Some commenters also note that office politics and irrelevant contributions inflate author lists.

**Tags**: `#machine learning`, `#academic publishing`, `#authorship`, `#readability`

---

<a id="item-17"></a>
## [Why ML Conferences Outshine Journals](https://www.reddit.com/r/MachineLearning/comments/1urqqk6/journals_vs_conferences_ml_research_r/) ⭐️ 6.0/10

A Reddit user initiated a discussion on why machine learning conferences like ICML and NeurIPS have become more prestigious than traditional journals in recent years. This shift affects how ML research is disseminated and evaluated, potentially speeding up innovation but also raising concerns about review quality and reproducibility. The post notes that the AI boom and faster acceptance rates at conferences may be driving this trend, but no new data or analysis is provided.

reddit · r/MachineLearning · /u/hg_wallstreetbets · Jul 9, 13:44

**Background**: In many scientific fields, journals are the primary venue for publishing research, but in machine learning, top conferences (e.g., NeurIPS, ICML, ICLR) have become the dominant outlets due to their fast review cycles and high visibility. This trend has been ongoing for over a decade, with conferences often considered more prestigious than journals in the ML community.

**Discussion**: The discussion likely includes varied opinions, with some agreeing that conferences offer faster dissemination and networking opportunities, while others argue that journals provide more thorough peer review and archival value.

**Tags**: `#machine learning`, `#academic publishing`, `#conferences`, `#journals`

---

<a id="item-18"></a>
## [Talos-XII: Hand-written autograd and RL in Rust for gacha simulation](https://www.reddit.com/r/MachineLearning/comments/1urvxgb/talosxii_handwritten_autograd_small_rlmlp_stack/) ⭐️ 6.0/10

A Rust CLI simulator called Talos-XII trains small neural networks (EnvNet, Dueling DQN, PPO with MLA transformer) entirely with a hand-written autograd engine, without any external ML frameworks like PyTorch or ndarray, to model gacha probability in Arknights: Endfield. This project demonstrates that compact RL policies can be built from scratch in Rust for niche domains like gacha probability, offering a lightweight alternative to heavy ML frameworks. It also invites community benchmarking to validate its custom ACHF optimization across different hardware. The simulator includes a custom autograd engine supporting matmul, conv2d, pooling, and gradient-checked backward passes, with runtime SIMD dispatch (scalar, AVX2, AVX-512, NEON) and Rayon-parallelized simulations. The ACHF component blends dense and sparse paths with a gradient-sensitive gate and Sinkhorn projection, but its speed/accuracy tradeoff is unverified outside the author's machine.

reddit · r/MachineLearning · /u/zay0kami · Jul 9, 16:52

**Background**: Gacha games use probabilistic mechanics where players spend in-game currency for a chance to obtain rare items. Traditional static probability tables can answer simple questions, but RL-based simulation can model dynamic strategies like when to stop pulling. Talos-XII implements this with hand-written neural networks in Rust, avoiding dependencies on large ML frameworks.

<details><summary>References</summary>
<ul>
<li><a href="https://gachacalc.com/">Gacha Calculator</a></li>
<li><a href="https://arxiv.org/abs/1511.06581">[1511.06581] Dueling Network Architectures for Deep ...</a></li>
<li><a href="https://www.emergentmind.com/topics/multi-head-latent-attention-mla-92d5c8a2-deb3-4136-98dd-8bc8100d4259">Multi-Head Latent Attention ( MLA )</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#reinforcement learning`, `#autograd`, `#gacha`, `#simulation`

---