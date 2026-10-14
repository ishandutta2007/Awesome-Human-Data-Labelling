# Awesome-Human-Data-Labelling

## Top Human Data Labelling Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Expert Annotation, RLHF Preference Data & Workforce-Scale Labelling*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Human Data Labelling**. These tools enable AI labs, enterprises, and researchers to source expert annotations, collect RLHF preference data, and manage workforce-scale labelling operations—turning raw data into model-ready training signal.



**Examples** include Surge AI, Scale AI, Mercor, Appen, Sama, Labelbox, iMerit, Toloka, SuperAnnotate, and Turing (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, annotation workflows, and open RLHF pipelines—ideal for ML engineers, data teams, and developers seeking transparent, vendor-independent labelling infrastructure.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Surge AI](https://www.surgehq.ai/)**  

  Premium RLHF specialist with a curated expert network and multi-rater adjudication quality model. Competes head-on with Scale at sometimes lower headline cost. **The default when you need only RLHF preference data and want the strongest pure specialist** . Less generalist than Scale—if you need RLHF plus classical labelling plus multimodal, Scale fits better .



- **[Scale AI](https://scale.com/)**  

  The default for frontier-lab-adjacent projects. Outlier and SEAL workforce, mature RLHF pipeline, deepest customer evidence. **Tax: enterprise-only engagement, sales cycle measured in months, pricing disclosed only under NDA** . Broadest capability surface across RLHF, autonomous vehicles, multimodal, and classical labelling .



- **[Mercor](https://mercor.com/)**  

  Expert marketplace recruiting and vetting domain specialists (software engineering, medicine, law, finance) for AI labs. **Annualized revenue surpassed $2 billion with reported valuation around $20 billion** . Expanded by acquisition into expert-graded benchmarks (Sepal AI) and RL environments (Deeptune). **Rockier headlines include a reported early 2026 data breach and lawsuits from contract workers** .



- **[Appen](https://appen.com/)**  

  The veteran large-scale workforce labelling provider. Massive global workforce, broad capability surface, mature processes. **Tax: less differentiated than specialists; project management quality varies by engagement** .



- **[Sama](https://sama.com/)**  

  Differentiated on **ethical workforce practices** with roots in East Africa and expanded operations in Montreal and Europe. Strong managed-QA and Fortune-50 enterprise track record. **Tax: smaller crowd headcount than Appen; rush-project capacity ceiling at very high end** .



- **[Labelbox](https://labelbox.com/)**  

  Platform-led tooling supporting customer-owned workforces. **Self-service plus managed labeling**—three modes: Self-service (your team labels), Boost (Labelbox supplies labelers), Foundry (foundation models first pass, humans review). Publishes baseline pricing .



- **[iMerit](https://imerit.net/)**  

  **Strongest for regulated-industry expert work** (healthcare, finance, geospatial). Expert-domain depth where cost per label rises 5-20x against generalist tasks—right answer is often hybrid: synthetic for routine, expert for edge cases .



- **[Toloka](https://toloka.ai/)**  

  Strongest for **international and multilingual work** with public marketplace pricing making budgeting tractable. **Tax: open-marketplace model means QA setup falls more on the buyer** .



- **[SuperAnnotate](https://www.superannotate.com/)**  

  Platform supporting full lifecycle of AI data development. Annotation for images, video, text, audio, and documents with AI-assisted labeling, quality assurance workflows, and Python SDK/REST API.



- **[Turing](https://www.turing.com/)**  

  Expert network for AI training data and model evaluation. Connects domain specialists to AI labs for demonstrations, evaluations, and domain-specific training data.



## Open-Source GitHub Projects



- **[Label Studio](https://github.com/HumanSignal/label-studio)**  

  **The most comprehensive and active open-source annotation platform** (Apache-2.0) . Covers small-model (CV/NLP/audio) **and** large-model (RLHF, dialogue ranking, LLM evaluation) scenarios. Mature ML Backend mechanism for pre-labelling and active learning. Multi-user collaboration, review workflows, REST API/Python SDK. Exports to COCO, JSON, CSV, HuggingFace dataset formats. **The default choice for NLP+CV mixed projects, LLM fine-tuning datasets, and RAG Q&A annotation** .



- **[CVAT](https://github.com/cvat-ai/cvat)**  

  **The computer vision industrial-grade benchmark** (MIT, originally Intel) . Strongest for images, video, image sequences, 3D point clouds, 2D boxes, polygon segmentation, keypoints, skeletons, and video object tracking. **SAM3 and YOLO auto pre-labelling**; complete task assignment, multi-level quality inspection, annotation time tracking; native S3/object storage; 20+ export formats (COCO, YOLO, KITTI, MOT). Helm for large-scale K8s cluster deployment. **The default for autonomous driving, medical imaging, and video segmentation** .



- **[OpenRLHF](https://github.com/OpenRLHF/OpenRLHF)**  

  **Open-source RLHF framework built on Ray, vLLM, DeepSpeed, and HuggingFace Transformers** (Apache-2.0) . **1.22x–1.68x training efficiency speedups** vs. state-of-the-art frameworks across model sizes, with **significantly fewer lines of code** . **Single-turn agent execution** supports custom reward functions—rule-based (length, format, code execution, math verification), external API (judge models, compilers, test suites), and hybrid rewards . **Multi-turn agent execution** for reasoning chains, coding with feedback, and game playing via `AgentInstanceBase` with reset/step methods . Adopted by leading institutions to accelerate RLHF research .



- **[knowlyr-datalabel](https://pypi.org/project/knowlyr-datalabel/0.3.0/)**  

  **Offline-first, zero-dependency annotation platform generating standalone HTML interfaces** (PyPI) . **5 annotation types** (rating, single-choice, multi-choice, text, ranking), dark mode, undo support, statistics panel, and **large dataset support (1000+ tasks with pagination/search)** . **Multi-annotator merge with IAA computation** (Cohen's/Fleiss' Kappa, Krippendorff's Alpha). **LLM-powered pre-labelling, quality analysis, and guideline generation** via Kimi/Moonshot, OpenAI, or Anthropic. **MCP support** (11 tools, 6 resources, 3 prompts) for Claude Desktop/Code integration . **The most feature-complete lightweight open-source annotation quality tool available.**



- **[Recogito Studio](https://research-software.cceh.uni-koeln.de/software/recogito-studio)**  

  **Extensible platform for collaborative, standards-based annotation of TEI text, IIIF images, and PDFs** (open-source) . Two integrated components: **recogito-client** (Astro.js + Vite) and **recogito-server** (Supabase + PostgreSQL). **Plugin architecture** with SDK: GeoTagger (gazetteer references), Reconciliation Service API, NER Plugin (Named Entity Recognition on plain text and TEI), Revisions Plugin, TEI Inliner Plugin, Sandcastle3D Export . **The most standards-compliant open-source annotation platform** for scholarly and cultural heritage projects.



- **[Audino](https://github.com/midas-research/audino)**  

  **Open-source audio annotation tool for humans** (MIT) . **1,067 GitHub stars**. Purpose-built for audio labelling—segment annotation, transcription, and classification workflows. **The most focused open-source audio annotation platform available.**



- **[YEDDA](https://github.com/jiesutd/YEDDA)**  

  **Lightweight collaborative text span annotation tool** (ACL 2018 Best Demo Paper Nomination) . **1,036 GitHub stars**. Supports entity recognition and span annotation with keyboard shortcuts for rapid labelling. **The most efficient open-source tool for pure text span annotation.**



- **[INCEpTION](https://github.com/inception-project/inception)**  

  **Semantic annotation platform offering intelligent annotation assistance and knowledge management** (open-source) . **602 GitHub stars**. Java-based with recommendation, knowledge base, and multi-layer annotation support. **The most mature open-source platform for linguistic annotation** with knowledge management.



- **[Xtreme1](https://github.com/xtreme1-io/xtreme1)**  

  **All-in-one data labeling and annotation platform for multimodal data** (Apache-2.0, LF AI & Data Foundation project) . **743 GitHub stars**. Supports **3D LiDAR point cloud, image, and LLM** (RLHF beta). Features data management and quality monitoring, finding and fixing labeling errors, model results visualization, and image data curation. **The first open-source data labeling project hosted in LF AI & Data Foundation** .



- **[PixLint](https://pypi.org/project/pixlint/)**  

  **MCP server giving AI assistants direct access to computer-vision dataset toolkit** (PolyForm Strict License) . **103 operations — 67 tools, 23 resources, 13 prompts**. **Dataset Doctor** runs full diagnostic and returns prioritized fix plan. **Label-error detection** automatically surfaces mislabeled images. **Natural-language query** ("find blurry images with a person on the left"). **Weak-slice discovery** for under-represented slices. **Auto-labeling** with pretrained COCO-80 detector, and one-command Hugging Face publishing . Exports to PyTorch, TensorFlow, Ultralytics, FiftyOne, CVAT, LabelMe . **The most AI-agent-integrated open-source dataset curation tool.**



- **[Annotix](https://www.mdpi.com/2073-431X/15/8/496)**  

  **Comprehensive annotation platform with 11 export and 8 import formats** (open-source) . **7 annotation types** including video annotation, time-series support, and tabular data. **19 training backends** with integrated training pipeline. **Serverless peer-to-peer collaboration over QUIC** without cloud infrastructure. **Full offline operation** with data sovereignty . **The most feature-complete open-source annotation platform for complete ML data preparation pipelines.**



### Additional Strong Open-Source Options



- **[OpenRLHF Single-Turn & Multi-Turn](https://pypi.org/project/openrlhf/)** — RLHF framework with custom reward functions and agent environment interaction .

- **[clean-evals](https://pypi.org/project/clean-evals/)** — Open-source eval platform with blind review, golden answer locking, and LLM judge calibration .

- **[veltai-data-platform](https://github.com/Arts-HCS/veldai-data-platform)** — Flask-based platform connecting businesses with human labelers and data providers .

- **[Bob](https://github.com/YadlaMani/bob)** — Solana-powered data labeling marketplace with crypto rewards .

- Community **n8n** workflows for annotation task routing and quality alert automation.



**Frameworks for building custom systems**: Combine **Label Studio** for multimodal annotation with **CVAT** for vision-specific workflows, **OpenRLHF** for RLHF training pipelines, **knowlyr-datalabel** for offline HTML-based annotation with IAA computation, and **PostgreSQL** for persistence—creating a fully self-hosted, enterprise-grade human data labelling platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Human data labelling platforms handling training data must comply with data protection regulations (GDPR, CCPA, etc.) and ensure annotator workforce agreements are in place.

- **Open-source annotation platforms are mature and production-ready.** Label Studio is the most comprehensive and active open-source platform, covering small-model (CV/NLP/audio) and large-model (RLHF, dialogue ranking, LLM evaluation) scenarios . CVAT is the industrial-grade benchmark for computer vision . **These are genuine alternatives to commercial platforms.**

- **Vendor selection depends on lane.** Most production AI programmes run **two or three vendors in parallel** . The high-end-plus-large-scale combination: Scale or Surge for RLHF + Toloka or Appen for classical labelling. Premium spend on parts that drive quality; workforce-scale spend on volume work .

- **Expert work costs 5-20x more per label.** iMerit and Invisible Tech are strongest for expert-domain work. The right answer is often hybrid: synthetic data or programmatic generation for routine cases, expert annotators for edge cases that drive model performance .

- **RLHF frameworks are maturing.** OpenRLHF achieves 1.22x–1.68x training efficiency speedups with significantly fewer lines of code . Custom reward functions (rule-based, external API, hybrid) enable reinforced fine-tuning without a trained reward model .

- Self-hosted open-source solutions require proper security hardening, annotation workforce management, and ongoing maintenance. Training data is a strategic asset—access controls and versioning are essential.



---



**Made for ML engineers, data quality analysts, annotation managers, and developers building transparent human data labelling solutions.**  

Let's make Human Data Labelling more open, data-driven, and quality-verified.
