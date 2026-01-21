# Industry Work Experience

## Huawei – Munich, Bavaria, Germany
(Senior Research Engineer, Jul 2023 – Present)

### AI4Sec Team
(Senior Research Engineer, Aug 2024 - Present)

Working on Next-Generation Firewall Systems in the Applied Networking Technologies Laboratory, Munich Research Center.

> Primary project 1: NGFW System Understanding & Prototype Planning

* Conducted several weeks of deep code review, debugging, and system analysis to document key components, execution flows, dependencies, and integration points across a complex C-based next-generation firewall (NGFW) system.
* Acted as the technical point of contact for the research team, answering detailed questions, presenting internal walkthroughs, and clarifying ambiguities with the development team.
* Leveraged this understanding to design the high-level architecture of a new research prototype, defining integration requirements for both research and production environments.
* Coordinated technical discussions and decisions during meetings and a business trip, delivering teaching sessions and deep-dive walkthroughs to accelerate team onboarding and alignment.
* Contributed to the team project of implementing an ML-based zero-day phishing detector module in C for Huawei NGFW System-on-Chip devices, including research, development, unit testing, performance benchmarking in the production environment.

> Primary project 2: Brand Identification Prototype (Python → Hyperscan)

* Led the development of a prototype to identify brands represented or impersonated by benign/phishing webpages, with solo ownership from idea to execution while incorporating team feedback.
* Built a catalog of structured brand-specific patterns (~200 brands) from multiple webpage components including titles, headers, copyright sections, links, and metadata.
* Developed multiple iterations of a Python prototype using BeautifulSoup and regex to validate the design and meet KPIs.
* Redesigned the system for streaming input in a firewall MITM setting, implementing Hyperscan-based incremental pattern matching.
* Iteratively refined patterns using an internally curated URLScan phishing and benign dataset, achieving approximately 75% recall, 99.5% precision, and 0.3% false positive rate.

> Primary project 3: Production C Implementation for ASE

* Converted two independent Python prototypes, one content-based and one URL-based, into high-performance C implementations.
* Executed both implementations solo under tight sprint deadlines, re-architecting pattern management, removing Python dependencies, and ensuring behavior equivalent to the original prototypes.
* Optimized for low latency and minimal memory usage (~300 bytes runtime memory, ~0.2 ms per execution), critical for firewall devices.
* Conducted peer review, static code checks, and Docker-based firewall environment testing, iterating on development team feedback.
* Delivered code for integration with an Adaptive Security Engine (ASE) product, wrote complete technical documentation, and assisted with end-to-end testing on real firewall devices. Met all stakeholder performance targets.

> Primary project 4: Advanced Evasive Phishing Research (HTML Smuggling)

* Investigated advanced and evasive phishing techniques that bypass traditional detectors, including staged attacks and JavaScript-driven delivery mechanisms.
* Performed a deep dive into 8–10 evasive phishing strategies, analyzing detection challenges, trade-offs, and applicability to a streaming firewall environment.
* Focused research on HTML smuggling attacks, where malicious payloads are dynamically reconstructed client-side to evade network inspection.
* Developed a Python-based prototype with a pattern matching engine, multi-stage processing logic, and a sophisticated scoring system to identify HTML smuggling behavior.
* Designed detection logic to identify characteristic code chains and execution patterns used in real-world HTML smuggling attacks.
* Conducted research, development, and benchmarking under constrained conditions with limited data and lack of reliable ground truth.
* Achieved promising early results with high precision, providing reliable identification of HTML smuggling techniques. Ongoing work.

> Secondary project: Overall System Design & Mentorship

* Designed the skeleton code and integration logic for the overall phishing detection prototype, guiding how individual research modules fit into the production pipeline.
* Coordinated with the product dev team and lead architect to ensure system-level designs met integration requirements.
* Mentored an intern to implement supporting C prototypes while independently handling BI content and URL parts in C.
* Supported research teammates in integrating their modules, ensuring smooth end-to-end production readiness.
* Conducted in-depth analysis of the product code, prepared technical documentation, and delivered multiple presentations to the team and stakeholders to improve technical understanding.

> Secondary project: ML Inference Pipeline Implementation

* Translated the core phishing ML inference pipeline from TensorFlow (Python) and ONNX (C) to the internal Mindspore-based SiteAI/EAI engine, ensuring performance parity across implementations.
* Optimized data buffering and preprocessing to support streaming input of packets while maintaining low latency.
* Conducted extensive benchmarking, debugging intermediate tensors, analyzing sample-level outputs, and logging vector states for accuracy verification.
* Integrated the inference pipeline into the research prototype and handed it to an intern for engineering-level integration into the product pipeline, mentoring throughout.

> Tertiary projects: Data Analysis & Pipelines

* Conducted analysis on various open-source and internal HTML datasets for benign and phishing sites, producing a conclusive report highlighting patterns for machine learning features used by colleagues.
* Performed multiple phases of URLScan data analysis to reverse-engineer the "primary request" in network events, developing a heuristic algorithm based on CDP events that correctly predicted the primary request across 2M URLScan samples.
* Developed a scraper bot for MWC conference demos, using a headless browser to collect CDP events, predict the primary request, and capture metadata/HTML pages for internal analysis and marketing prototype runs.
* Developed a webpage for live demo at MWC conference which dynamically presents the phishing detection rate of Huawei's product against its competitors.
* Completed multiple DevOps tasks to support early prototype demos to stakeholders, including HTML page design, simulated phishing attacks, MITM proxy setup, web-scraping bots, pytest infrastructure, and GitLab CI/CD pipelines.

> Other responsibilities

* Conducted thorough research in networking, web security, machine learning, and phishing attack prevention.
* Assisted in interviewing, onboarding, and mentoring new full-time team members and interns.
* Represented the technical team at the Huawei Network Summit 2024, assisting marketing and engaging with customers.
* Coordinated project direction, targets, and product integration details with stakeholders during a business trip to China.

### Storage4AI Team
(Senior Research Engineer, Jul 2023 – Jul 2024)

Worked on Next-Generation Data Infrastructure in the Intelligent Cloud Technologies Laboratory, Munich Research Center.

> Primary project

* Researched, designed, and implemented NHQ, a vector+scalar composite index based on HNSW, enabling efficient scalar filtering during vector search.
* Implemented NHQ across three phases: an open-source prototype on NMSLIB’s hnswlib, an internal implementation based on FAISS aligned with Knowhere / Milvus, and a production deployment in Huawei Cloud’s Long-term Memory Service (LMS).
* Led the project end-to-end as a solo developer, taking it from algorithm design and prototyping to internal adoption and production delivery, incorporating feedback from the team and stakeholders.
* Built a rigorous benchmarking framework using standard SIFT1M vector queries combined with carefully curated scalar filters of varying data types, cardinalities, and selectivities.
* Evaluated performance under controlled hardware and system configurations, varying CPU count, memory, and number of executors.
* Validated the solution through standalone testing, private cloud deployment, and end-to-end production cloud cluster evaluation.
* Achieved a final 1.5×–5× speedup over baseline HNSW with scalar post-filtering, while maintaining comparable recall and index size.
* Successfully delivered the project to production after meeting stakeholder-defined KPIs, leading to adoption in LMS.

> Secondary project

* Improved the debuggability of a Spark SQL–based system by instrumenting query execution to collect run-time scan and filter selectivity statistics (rows/bytes scanned vs. returned).
* Exposed predicate pushdown (near-data processing) behavior by updating the Spark History Server web UI.

> Other responsibilities

* Conducted thorough research in the fields of databases, distributed systems and vector storage.
* Presented deep dive sessions and participated in discussions to decide project directions.
* Coordinated project milestones and goals with stakeholders during a business trip to China.
