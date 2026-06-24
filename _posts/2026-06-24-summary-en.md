---
layout: default
title: "Horizon Summary: 2026-06-24 (EN)"
date: 2026-06-24
lang: en
---

> From 34 items, 18 important content pieces were selected

---

1. [WYSIWYG TikZ Editor Syncs Code and Graphics](#item-1) ⭐️ 8.0/10
2. [The Coming Loop: AI's Impact on Code Maintenance](#item-2) ⭐️ 8.0/10
3. [Unlimited OCR: One-Shot Long-Horizon Document Parsing](#item-3) ⭐️ 8.0/10
4. [Prompt Injection as Role Confusion](#item-4) ⭐️ 8.0/10
5. [Porting Moebius 0.2B Inpainting Model to Browser with WebGPU](#item-5) ⭐️ 8.0/10
6. [DeepSWE: A Contamination-Free Benchmark for Frontier Coding Models](#item-6) ⭐️ 8.0/10
7. [FUTO Swipe: A New Privacy-Focused Swipe Typing Model](#item-7) ⭐️ 7.0/10
8. [Apple Acquires Swift Package Index](#item-8) ⭐️ 7.0/10
9. [Extreme Heat Conference Canceled Due to Heat Warning](#item-9) ⭐️ 7.0/10
10. [Vitamin D Benefits Real but Overhyped](#item-10) ⭐️ 7.0/10
11. [Datasette 1.0a35 Adds Create/Alter Table Interfaces](#item-11) ⭐️ 7.0/10
12. [ML teams skip adversarial testing in production](#item-12) ⭐️ 7.0/10
13. [Non-deterministic Vulnerability Detection Benchmark](#item-13) ⭐️ 7.0/10
14. [Remembering the inventor of red and green squiggly underlines](#item-14) ⭐️ 6.0/10
15. [Simon Willison Tests OPFS with Pyodide for Datasette Lite](#item-15) ⭐️ 6.0/10
16. [Hugging Face Revives Papers with Code with New Features](#item-16) ⭐️ 6.0/10
17. [Seeking Syntax-Robust NLI for Diffusion LLM Outputs](#item-17) ⭐️ 6.0/10
18. [Potential Mistake Found in ICLR 2026 Blog Post](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [WYSIWYG TikZ Editor Syncs Code and Graphics](https://tikz.dev/editor/) ⭐️ 8.0/10

An open-source WYSIWYG TikZ editor has been released that allows users to edit TikZ source code visually by dragging and resizing elements, with the source and rendered figure staying in sync. The editor was built almost entirely using the AI coding agent Codex. This tool addresses a major pain point for academics and LaTeX users who manually tweak coordinates and recompile to create figures, potentially saving significant time. It also demonstrates how AI coding agents can enable building complex software that would otherwise be too tedious for humans. The editor parses TikZ code and tracks the exact source location of each object, allowing it to override only the numbers in coordinates when dragging without altering other code structure. It also includes converters from SVG, PPTX, and IPE to TikZ, and reimplements LaTeX hyphenation and line-breaking for multi-line nodes.

hackernews · DominikPeters · Jun 23, 14:24 · [Discussion](https://news.ycombinator.com/item?id=48645437)

**Background**: TikZ is a powerful LaTeX package for creating vector graphics using commands like \draw. Academics often code figures manually, requiring repeated recompilation to adjust positions. WYSIWYG (What You See Is What You Get) editors allow direct manipulation of the visual output, but existing TikZ editors typically lack simultaneous source and visual editing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.overleaf.com/learn/latex/TikZ_package">TikZ package - Overleaf, Online LaTeX Editor</a></li>
<li><a href="https://en.wikipedia.org/wiki/WYSIWYG_editor">WYSIWYG editor</a></li>
<li><a href="https://github.com/topics/tikz?l=tex&o=desc&s=updated">tikz · GitHub Topics · GitHub</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some praise the UI and concept, while others criticize the generated TikZ code for using absolute coordinates unnecessarily. One commenter notes that AI coding tools can already generate TikZ code effectively, and another points to a specialized alternative, quiver.app. The developer reveals the project cost about $500 in ChatGPT fees despite $15k API rates, using 700M tokens.

**Tags**: `#LaTeX`, `#TikZ`, `#editor`, `#academic tools`, `#open source`

---

<a id="item-2"></a>
## [The Coming Loop: AI's Impact on Code Maintenance](https://lucumr.pocoo.org/2026/6/23/the-coming-loop/) ⭐️ 8.0/10

Armin Ronacher's essay 'The Coming Loop' warns that reliance on AI assistants is creating codebases that assume machine participation, leading to a loss of human understanding and maintenance skills. This matters because it highlights a fundamental shift in software development where human comprehension is being replaced by AI-generated context, potentially making codebases unmaintainable without AI tools. The essay describes a 'loop' where developers merge code they cannot fully explain, and rely on AI to summarize or contextualize communications, eroding their ability to create issue reports or discuss technical details independently.

hackernews · ingve · Jun 23, 11:06 · [Discussion](https://news.ycombinator.com/item?id=48643180)

**Background**: Large Language Models (LLMs) like GPT-4 are increasingly used to generate code, but this essay argues that over-reliance on them can degrade human expertise. The author, Armin Ronacher, is a respected figure in the Python community, known for projects like Flask and Jinja2.

**Discussion**: Commenters debate the trade-offs: some argue that the 'loop' works when developers have clear specs, while others note that LLMs are good for goal-driven tasks but poor at aesthetics and taste. A key insight is that the bottleneck shifts to writing clear specifications, which still requires human effort.

**Tags**: `#AI-assisted development`, `#software engineering`, `#LLMs`, `#code maintenance`, `#human-AI collaboration`

---

<a id="item-3"></a>
## [Unlimited OCR: One-Shot Long-Horizon Document Parsing](https://github.com/baidu/Unlimited-OCR) ⭐️ 8.0/10

Baidu released Unlimited OCR, a one-shot long-horizon parsing method for multi-page documents using a vision-language model with a novel recurrent sliding-window attention (R-SWA) mechanism that reduces memory and computational costs. This approach enables parsing entire books in a single pass without running out of VRAM, overcoming a key limitation of existing OCR systems that require page-by-page processing or post-hoc correction. The R-SWA mechanism uses a sliding window for local context while always attending to the image/prefix, achieving linear memory growth instead of quadratic. The model surpasses DeepSeek OCR on popular document parsing benchmarks.

hackernews · ingve · Jun 23, 11:35 · [Discussion](https://news.ycombinator.com/item?id=48643426)

**Background**: Traditional OCR systems process documents page by page, which is inefficient for long documents and loses cross-page context. Vision-language models (VLMs) can understand both text and layout, but their attention mechanisms scale quadratically with input length, causing memory issues for long documents. Unlimited OCR addresses this with a recurrent sliding-window attention that keeps memory usage linear.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/baidu/Unlimited-OCR">GitHub - baidu/Unlimited-OCR: Unlimited OCR Works: Welcome the Era of One-shot Long-horizon Parsing. · GitHub</a></li>
<li><a href="https://arxiv.org/html/2606.23050v1">Unlimited OCR Works Welcome the Era of One-shot Long-horizon Parsing</a></li>
<li><a href="https://news.ycombinator.com/item?id=48643426">Unlimited OCR: One-Shot Long-Horizon Parsing | Hacker News</a></li>

</ul>
</details>

**Discussion**: The Hacker News community praised the architectural hack for reducing memory usage and noted its potential for sheet music OCR. Commenters also appreciated the acknowledgment of DeepSeek-OCR and PaddleOCR, and one pointed out the name references the Fate/stay night series.

**Tags**: `#OCR`, `#Vision-Language Model`, `#Document Parsing`, `#Machine Learning`, `#Open Source`

---

<a id="item-4"></a>
## [Prompt Injection as Role Confusion](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

A new research paper, 'Prompt Injection as Role Confusion,' reveals that LLMs cannot reliably distinguish privileged text (e.g., system prompts) from user input, and that models prioritize the writing style over the actual content of the text. This finding fundamentally undermines current prompt injection defenses, showing that style-based attacks can achieve up to 61% success rates, and suggests that without genuine role perception, injection defense will remain a perpetual whack-a-mole game. The researchers introduced 'destyling'—rewriting text to look less like the expected format in a role tag—which reduced attack success from 61% to 10%, despite being nearly invisible to human readers. They also developed novel role probes to capture how models internally identify 'who is speaking.'

rss · Simon Willison · Jun 22, 23:59

**Background**: Prompt injection is a cybersecurity exploit where innocuous-looking inputs cause unintended behavior in LLMs. It occurs because both system prompts and user inputs are natural-language strings, making it hard for models to distinguish them. Role confusion refers to the model's flawed inference of roles based on writing style rather than source.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://role-confusion.github.io/">Prompt Injection as Role Confusion</a></li>
<li><a href="https://arxiv.org/pdf/2603.12277v2">Prompt Injection as Role Confusion - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#prompt injection`, `#LLM security`, `#jailbreak`, `#role confusion`, `#AI safety`

---

<a id="item-5"></a>
## [Porting Moebius 0.2B Inpainting Model to Browser with WebGPU](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison successfully ported the Moebius 0.2B lightweight image inpainting model to run entirely in the browser using WebGPU, and released a live demo at simonw.github.io/moebius-web/. He used Claude Code to convert the PyTorch model to ONNX and build the web application. This port demonstrates that state-of-the-art image inpainting can run locally in a browser without server costs or GPU dependencies, making it accessible to a wider audience. It also showcases the growing capability of WebGPU for real-time AI inference and the potential of AI-assisted coding tools like Claude Code for rapid prototyping. The model was converted from PyTorch to ONNX and then run using ONNX Runtime Web with the WebGPU backend. The demo allows users to upload images, mark regions to inpaint, and run inference entirely on-device. The project was built in parallel with a major Datasette feature using Claude Code, completing the port in a few hours.

rss · Simon Willison · Jun 22, 23:43

**Background**: Image inpainting is the task of filling in missing or removed regions of an image with plausible content. Moebius is a 0.2B parameter model that claims performance comparable to 10B+ models like FLUX.1. WebGPU is a modern browser API that enables high-performance GPU compute and AI inference directly in the browser, supported by all major browsers as of 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.19195">[2606.19195] Moebius: 0.2B Lightweight Image Inpainting ...</a></li>
<li><a href="https://github.com/hustvl/Moebius">GitHub - hustvl/Moebius: [ECCV 2026] Moebius: 0.2B ...</a></li>
<li><a href="https://hustvl.github.io/Moebius/">Moebius: 0.2B Lightweight Image Inpainting Framework with 10B ...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (linked in the article) likely includes praise for the technical achievement and discussions about WebGPU's potential for on-device AI. Some commenters may question the model's quality compared to larger models or discuss the trade-offs of browser-based inference.

**Tags**: `#image inpainting`, `#WebGPU`, `#browser ML`, `#model porting`, `#AI`

---

<a id="item-6"></a>
## [DeepSWE: A Contamination-Free Benchmark for Frontier Coding Models](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 8.0/10

DeepSWE is a new open-source benchmark that evaluates frontier coding agents on original, long-horizon software engineering tasks, with hand-written verifiers to ensure contamination-free and reliable assessment. This benchmark addresses critical flaws in existing benchmarks like SWE-bench, such as data contamination and lack of task diversity, providing a more realistic measure of AI coding capabilities that could drive progress in autonomous software engineering. DeepSWE features 91 repositories across 5 languages, with prompts half the length of SWE-bench Pro's but requiring 5.5x more code and ~2x more output tokens, and uses hand-written verifiers that test software behavior rather than implementation details.

reddit · r/MachineLearning · /u/we_are_mammals · Jun 24, 02:03

**Background**: Existing benchmarks like SWE-bench often suffer from data contamination, where models may have seen solutions during pretraining, and lack task diversity. DeepSWE creates tasks from scratch and covers multiple languages and repositories to better reflect real-world software engineering complexity.

<details><summary>References</summary>
<ul>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE</a></li>
<li><a href="https://www.swebench.com/original.html">SWE-bench</a></li>

</ul>
</details>

**Discussion**: The Reddit community praised DeepSWE for its contamination-free design and real-world relevance, but some questioned the hand-written verifiers' scalability and whether the benchmark truly captures long-horizon tasks. Comparisons to SWE-bench Pro were common, with users noting DeepSWE's higher code complexity.

**Tags**: `#benchmark`, `#code generation`, `#AI`, `#machine learning`, `#software engineering`

---

<a id="item-7"></a>
## [FUTO Swipe: A New Privacy-Focused Swipe Typing Model](https://swipe.futo.tech/) ⭐️ 7.0/10

FUTO has released a new swipe typing model for its privacy-focused keyboard, aiming to rival Gboard's accuracy while keeping data fully offline. This development challenges the dominance of proprietary swipe keyboards like Gboard, offering a private, open-source alternative that could reshape mobile input standards. The model is available in the FUTO Keyboard app and can be downloaded separately for developers; it runs fully offline and uses a GPLv3-licensed library, though the Android keyboard app uses a different license.

hackernews · futohq · Jun 23, 17:50 · [Discussion](https://news.ycombinator.com/item?id=48648619)

**Background**: Swipe typing allows users to input words by sliding a finger across the keyboard, but most implementations rely on cloud-based processing, raising privacy concerns. FUTO Keyboard is a fully offline, open-source keyboard that prioritizes user privacy. The new swipe model was trained using community-contributed data collected through an opt-in program.

<details><summary>References</summary>
<ul>
<li><a href="https://swipe.futo.tech/">FUTO Swipe</a></li>
<li><a href="https://huggingface.co/futo-org/futo-swipe">futo -org/ futo - swipe · Hugging Face</a></li>
<li><a href="https://keyboard.futo.org/">FUTO Keyboard</a></li>

</ul>
</details>

**Discussion**: Users report that the new model is a significant improvement, with some switching from Gboard full-time, though issues like random capitalization and lack of context awareness remain. One commenter noted the licensing difference between the library (GPLv3) and the keyboard app (FUTO License) as a concern.

**Tags**: `#swipe typing`, `#keyboard`, `#privacy`, `#FUTO`, `#mobile input`

---

<a id="item-8"></a>
## [Apple Acquires Swift Package Index](https://swiftpackageindex.com/blog/swift-package-index-joins-apple) ⭐️ 7.0/10

Apple has acquired the Swift Package Index (SPI), a community-run package discovery and metadata search engine for Swift packages. The SPI team announced the acquisition on their blog, stating that the service will remain open source and free for developers. This acquisition signals Apple's strategic investment in the Swift ecosystem and package management, potentially improving the developer experience. However, it raises concerns about Apple's track record with open source and the possibility of future regulation on which packages are indexed. The Swift Package Index currently indexes metadata from over 11,000 packages. Apple explicitly mentioned developer identity as a future direction, which has caused unease among some community members.

hackernews · JDevlieghere · Jun 23, 18:00 · [Discussion](https://news.ycombinator.com/item?id=48648779)

**Background**: The Swift Package Index is a community-run website that helps developers discover Swift packages by providing metadata, compatibility information, and search functionality. It complements Apple's official Swift Package Manager (SPM), which handles dependency resolution but lacks a centralized discovery platform. The acquisition follows Apple's pattern of acquiring community tools to integrate into its ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://9to5mac.com/2026/06/23/swift-package-index-joins-apple-pledges-to-remain-open-source/">Swift Package Index joins Apple, pledges to remain open ...</a></li>
<li><a href="https://swiftpackageindex.com/">Swift Package Index</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed. Some are happy for the SPI team's success, while others express skepticism about Apple's open source commitment and fear that Apple may restrict package indexing. A few see an opportunity to build a competitor that supports non-GitHub repositories.

**Tags**: `#Swift`, `#Apple`, `#Package Management`, `#Open Source`, `#Acquisition`

---

<a id="item-9"></a>
## [Extreme Heat Conference Canceled Due to Heat Warning](https://www.lse.ac.uk/granthaminstitute/events/extreme-heat-improving-governance-and-strengthening-action-around-the-world/) ⭐️ 7.0/10

A conference titled 'Extreme Heat: Improving Governance and Strengthening Action Around the World' was canceled because an extreme heat warning was issued for the event's location. The cancellation highlights the irony and urgency of climate adaptation, sparking debate on air conditioning adoption, building infrastructure, and governance in the face of rising temperatures. The conference was hosted by the Grantham Research Institute at LSE in collaboration with the Zurich Climate Resilience Alliance, and was scheduled to include a fireside chat.

hackernews · rendx · Jun 23, 23:26 · [Discussion](https://news.ycombinator.com/item?id=48653060)

**Background**: Extreme heat events are becoming more frequent and severe due to climate change, posing significant risks to public health and infrastructure. Many regions, especially in Europe, have building designs and cultural norms that limit the use of air conditioning, leading to higher heat-related mortality.

**Discussion**: Commenters noted the irony of canceling a heat conference due to heat, with some pointing to cultural resistance to air conditioning in Europe as a factor in heat-related deaths. Others contrasted the moderate temperatures (37-40°C) with experiences in Australia, where such heat is considered normal, and highlighted differences in building design and adaptation.

**Tags**: `#climate change`, `#infrastructure`, `#public health`, `#governance`, `#irony`

---

<a id="item-10"></a>
## [Vitamin D Benefits Real but Overhyped](https://dynomight.net/vitamin-d/) ⭐️ 7.0/10

A critical review of Vitamin D research concludes that benefits are real but limited to those with severe deficiency, while health influencers often exaggerate the hype. This analysis helps clarify the conflicting messages about Vitamin D supplementation, guiding evidence-based decisions for the general public and healthcare providers. The strongest evidence for Vitamin D is in severely deficient individuals; bumping up to normal range can provide improvements, but benefits for others are minimal.

hackernews · surprisetalk · Jun 23, 16:30 · [Discussion](https://news.ycombinator.com/item?id=48647486)

**Background**: Vitamin D is a fat-soluble vitamin essential for bone health and immune function. Many people take supplements based on claims of broad health benefits, but large randomized trials have shown mixed results, leading to debate about its efficacy.

**Discussion**: Comments highlight methodological issues in Vitamin D studies, such as seasonal and latitude adjustments, and the importance of co-factors like Vitamin K2. Some users note that individual responses vary and that blood level monitoring is crucial.

**Tags**: `#nutrition`, `#vitamin D`, `#evidence-based medicine`, `#health research`

---

<a id="item-11"></a>
## [Datasette 1.0a35 Adds Create/Alter Table Interfaces](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a35 introduces a new 'Create table' interface and JSON API for defining columns, primary keys, and constraints, as well as an 'Alter table' interface and API for modifying existing tables including adding, renaming, and dropping columns. These features significantly enhance Datasette's utility as a database management tool, allowing users to perform schema changes directly through the UI or API without needing external SQLite tools. The create table API supports custom column types, NOT NULL constraints, literal and expression defaults, and single-column foreign keys. The alter table API also includes a 'Drop table' button and supports renaming the table itself.

rss · Simon Willison · Jun 23, 21:34

**Background**: Datasette is an open-source tool for exploring and publishing SQLite databases. It provides a web interface and a JSON API for querying and managing data. Prior to this release, creating or altering table schemas required using SQLite command-line tools or external scripts.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/latest/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="https://simonwillison.net/2026/Jun/23/datasette/">Release: datasette 1.0a35 - simonwillison.net</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#release`, `#database`, `#JSON API`

---

<a id="item-12"></a>
## [ML teams skip adversarial testing in production](https://www.reddit.com/r/MachineLearning/comments/1uddtws/are_model_security_risks_extraction_poisoning/) ⭐️ 7.0/10

A Reddit discussion highlights that many ML teams are not testing model security risks such as extraction and poisoning attacks before deploying models into production, contrasting with standard security reviews in traditional software. This gap exposes organizations to intellectual property theft, biased outputs, and backdoor vulnerabilities, undermining trust in AI systems and potentially leading to regulatory non-compliance. Model extraction attacks steal model behavior via repeated API queries, while model poisoning manipulates training data or parameters to introduce backdoors or biases; both are well-documented but rarely tested in production.

reddit · r/MachineLearning · /u/Xorphian · Jun 23, 10:52

**Background**: Adversarial machine learning studies attacks and defenses for ML models. Model extraction involves querying a model to build a replica, while model poisoning corrupts the model during training or fine-tuning. Traditional software security includes rigorous testing like penetration testing, but similar practices for ML models are not yet standard.

<details><summary>References</summary>
<ul>
<li><a href="https://www.praetorian.com/blog/stealing-ai-models-through-the-api-a-practical-model-extraction-attack/">Stealing AI Models Through the API: A Practical Model Extraction Attack | Praetorian</a></li>
<li><a href="https://owasp.org/www-project-machine-learning-security-top-10/docs/ML10_2023-Model_Poisoning">ML10:2023 Model Poisoning - OWASP Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adversarial_machine_learning">Adversarial machine learning - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#model security`, `#adversarial testing`, `#ML deployment`, `#AI safety`

---

<a id="item-13"></a>
## [Non-deterministic Vulnerability Detection Benchmark](https://www.reddit.com/r/MachineLearning/comments/1ud0rft/nondeterministic_vulnerability_detection/) ⭐️ 7.0/10

A work-in-progress benchmark for non-deterministic vulnerability detection has been released, which obfuscates known CWE patterns from the Juliet test suite and injects LLM-generated comments to test their effect on detection accuracy. This benchmark addresses a critical gap in evaluating LLMs for vulnerability detection by removing biases from known CWE patterns and studying the influence of natural language comments, which is essential for building reliable AI security tools. The benchmark uses Juliet code that has been 'hidden' to resemble a real codebase, preserving ground truth while removing LLMs' advantage of recognizing known CWEs. It includes hundreds of CWEs and fills most input contexts, with comments generated by an LLM in accurate, misleading, or neutral sentiments.

reddit · r/MachineLearning · /u/Psychological_Meat_6 · Jun 22, 23:34

**Background**: The Juliet Test Suite is a collection of over 81,000 synthetic C/C++ and Java programs with known flaws, commonly used for evaluating static analysis tools. LLMs have shown promise in vulnerability detection but are non-deterministic and can be biased by known patterns or comments. Recent advances like Claude Mythos have demonstrated autonomous vulnerability discovery, highlighting the need for robust benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/arichardson/juliet-test-suite-c">GitHub - arichardson/juliet-test-suite-c</a></li>
<li><a href="https://www.nist.gov/publications/juliet-11-cc-and-java-test-suite">The Juliet 1.1 C/C++ and Java Test Suite | NIST</a></li>
<li><a href="https://venturebeat.com/security/mythos-detection-ceiling-security-teams-new-playbook">Mythos autonomously exploited vulnerabilities that survived ...</a></li>

</ul>
</details>

**Tags**: `#vulnerability detection`, `#LLM benchmarking`, `#CWE`, `#security`, `#AI safety`

---

<a id="item-14"></a>
## [Remembering the inventor of red and green squiggly underlines](https://devblogs.microsoft.com/oldnewthing/20260622-00/?p=112451) ⭐️ 6.0/10

Raymond Chen's article pays tribute to Tony Krueger, the developer who introduced red and green squiggly underlines for spell-check in Microsoft Word, a feature that became a ubiquitous UI element. This minor UI feature revolutionized how users interact with text, making spelling and grammar errors instantly visible and setting a standard for real-time feedback in word processors. The squiggly underlines were first introduced in Microsoft Word for Windows, and Tony Krueger was responsible for porting the spell-check feature that included them.

hackernews · saikatsg · Jun 23, 18:10 · [Discussion](https://news.ycombinator.com/item?id=48648959)

**Background**: Before squiggly underlines, spell-check required manual initiation, often through a separate dialog. The red squiggle for misspellings and green for grammar errors provided instant, non-intrusive feedback, becoming a hallmark of modern word processing.

**Discussion**: Commenters expressed nostalgia for the feature, with some noting the irony of Wikipedia citing Chen's article as evidence for Krueger's role. Others wished such stories were shared before the developer passed away, and one user proposed an AI-powered auto-correct button triggered by squiggles.

**Tags**: `#history`, `#UI`, `#Microsoft`, `#spell-check`

---

<a id="item-15"></a>
## [Simon Willison Tests OPFS with Pyodide for Datasette Lite](https://simonwillison.net/2026/Jun/23/opfs-pyodide/#atom-everything) ⭐️ 6.0/10

Simon Willison built a test harness using the Origin Private File System (OPFS) and Pyodide to explore persistent SQLite file editing in the browser for Datasette Lite. This experiment could enable Datasette Lite to edit persistent SQLite files stored on the user's computer, bridging the gap between web apps and local file storage. The test harness is a playground UI built by Claude Code for web, allowing Willison to test OPFS support across different browsers.

rss · Simon Willison · Jun 23, 18:58

**Background**: Datasette Lite runs the full server-side Python Datasette application in the browser via Pyodide and WebAssembly. The Origin Private File System (OPFS) is a browser API that provides a private, sandboxed filesystem for web applications, optimized for performance.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN</a></li>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.0</a></li>
<li><a href="https://github.com/simonw/datasette-lite">GitHub - simonw/ datasette - lite : Datasette running in your browser...</a></li>

</ul>
</details>

**Tags**: `#webassembly`, `#pyodide`, `#datasette`, `#browsers`, `#sqlite`

---

<a id="item-16"></a>
## [Hugging Face Revives Papers with Code with New Features](https://www.reddit.com/r/MachineLearning/comments/1ucm508/some_new_updates_to_papers_with_code_p/) ⭐️ 6.0/10

Hugging Face has added SOTA badges, a new trending score combining GitHub stars and Hugging Face artifact popularity, support for external evaluations, and more benchmarks to Papers with Code. These updates make it easier for researchers to discover state-of-the-art papers and track their impact, fostering collaboration and reproducibility in the ML community. The trending score now incorporates Hugging Face model, dataset, and Space activity alongside GitHub stars. SOTA badges highlight top-3 benchmark performances, and external evals allow viewing third-party benchmark results not originally in the paper.

reddit · r/MachineLearning · /u/NielsRogge · Jun 22, 14:29

**Background**: Papers with Code was originally a popular platform for linking research papers to code and benchmarks, but was retired by Meta in July 2025. Hugging Face acquired the domain and is reviving it as an open-source community effort to help researchers discover and build upon each other's work.

<details><summary>References</summary>
<ul>
<li><a href="https://paperswithcode.co/">Papers with Code</a></li>
<li><a href="https://www.codesota.com/papers-with-code">Papers With Code Alternative: SOTA Leaderboards and Archived Data ...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#papers with code`, `#Hugging Face`, `#research tools`

---

<a id="item-17"></a>
## [Seeking Syntax-Robust NLI for Diffusion LLM Outputs](https://www.reddit.com/r/MachineLearning/comments/1ucy7p3/syntactically_robust_nli_for_semantics_of/) ⭐️ 6.0/10

A researcher on Reddit is asking about state-of-the-art syntax-robust Natural Language Inference (NLI) methods to evaluate semantic correctness of text generated by diffusion LLMs, which often contain syntactic noise. As diffusion LLMs emerge as alternatives to autoregressive models, their syntactic imperfections hinder the direct application of standard NLI for semantic evaluation, making syntax-robust NLI crucial for reliable assessment. The user notes that diffusion LLMs like LLaDA still struggle with syntactic correctness compared to autoregressive models, complicating NLI usage. They seek literature on NLI methods robust to such syntactic noise.

reddit · r/MachineLearning · /u/RepresentativeBee600 · Jun 22, 21:51

**Background**: Natural Language Inference (NLI) determines if a premise entails a hypothesis. Standard NLI models assume well-formed syntax, but diffusion LLMs generate text via iterative denoising, often producing syntactically imperfect outputs. Syntax-robust NLI aims to evaluate semantics despite such noise.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1ucy7p3/syntactically_robust_nli_for_semantics_of/">Syntactically robust NLI for semantics of imperfectly generated text? [R] - Reddit</a></li>
<li><a href="https://aclanthology.org/2023.iwcs-1.29.pdf">[PDF] AMR4NLI: Interpretable and robust NLI measures from semantic graph - ACL Anthology</a></li>
<li><a href="https://arxiv.org/abs/2502.09992">[2502.09992] Large Language Diffusion Models - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#NLI`, `#LLM`, `#syntax robustness`, `#diffusion models`, `#semantic evaluation`

---

<a id="item-18"></a>
## [Potential Mistake Found in ICLR 2026 Blog Post](https://www.reddit.com/r/MachineLearning/comments/1ud9i2g/found_a_potential_mistake_in_an_iclr_2026/) ⭐️ 6.0/10

A Reddit user has reported a potential mistake in an ICLR 2026 blog post and created a GitHub issue (#218) to document it, but has not received a response from the authors or organizers after several weeks. If confirmed, this could affect the credibility of the ICLR blog post track and highlight challenges in post-publication peer review. The incident underscores the need for responsive communication channels in academic publishing. The user is seeking community feedback on the issue via Reddit, as direct contact with the authors and organizers has been unsuccessful. The GitHub issue is part of the ICLR 2026 blog post repository, which uses a pull-request-based submission and review process.

reddit · r/MachineLearning · /u/metalwhaledev · Jun 23, 06:39

**Background**: ICLR (International Conference on Learning Representations) is a top-tier machine learning conference. Since 2022, it has hosted a blog post track where accepted submissions are published as blog posts rather than traditional papers. The track uses a GitHub-based workflow for submission, review, and publication, with issues used for discussion and errata.

<details><summary>References</summary>
<ul>
<li><a href="https://openreview.net/group?id=ICLR.cc/2026/BlogPosts">ICLR 2026 BlogPosts | OpenReview</a></li>
<li><a href="https://iclr-blog-track.github.io/submitting/">Submitting · The ICLR Blog Track</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#ICLR`, `#peer review`, `#bug report`, `#academic publishing`

---