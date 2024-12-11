# Professional Experience

## Employment

### Huawei – Munich, Bavaria, Germany
(Senior Research Engineer, Jul 2023 – Present)

#### AI4Sec Team
(Senior Research Engineer, Aug 2024 - Present)

Working on Next-Generation Firewall System in the Applied Networking Technologies Laboratory, Munich Research Center.

> Primary project

* Currently, implementing and optimizing an ML-based zero-day phishing detector module in C for the Huawei NGFW System-on-Chip.
* Leading the system design of the project while coordinating the high-level design with cybersecurity and machine learning experts from the team.
* Conducted in-depth analysis of the product code, prepared technical documentation, and delivered multiple presentations to the team and stakeholders.

> Secondary project

* Currently implementing a Python component to identify the imitated brand from the HTML content of phishing credential request pages.
* Conducted data analysis on various open-source and internal datasets containing HTML content for benign and phishing sites. Prepared a conclusive report to highlight patterns which would assist the development of a CNN classifier model.
* Completed several DevOps tasks for a prototype demo to stakeholders: designed HTML pages, simulated phishing attacks, set up MITM proxy, ran web-scraping bots, set up pytest infrastructure and GitLab CI/CD pipeline.

> Other responsibilities

* Conducted thorough research in the fields of networking, web security, machine learning, and phishing attack prevention.
* Assisted in interviewing, onboarding and supporting new full-time members and interns for the team.
* Represented the technical team at the Huawei Network Summit 2024, assisting the marketing team and engaging with customers.
* Currently, coordinating project direction, targets and product integration with stakeholders during business trip to China.

#### Storage4AI Team
(Senior Research Engineer, Jul 2023 – Jul 2024)

Worked on Next-Generation Data Infrastructure in the Intelligent Cloud Technologies Laboratory, Munich Research Center.

> Primary project

* Researched, prototyped and delivered a vector+scalar composite index for a distributed multi‑tenant vector database in Huawei Cloud.
* Led the project, taking full responsibility for development and delivery while incorporating valuable feedback from the team and stakeholders.
* Achieved up to 5x performance improvement compared to the state‑of‑the‑art HNSW index, while maintaining similar accuracy and index size.

> Secondary project

* Improved the debuggability of a Spark‑based system by collecting relevant statistics on run‑time and updating the history server web interface.

> Other responsibilities

* Conducted thorough research in the fields of databases, distributed systems and vector storage.
* Presented deep dive sessions and participated in discussions to decide project directions.
* Coordinated project milestones and goals with stakeholders during business trip to China.

## Masters Internships

### Oracle – Zurich, Switzerland
(Research Assistant, Sep 2022 – Mar 2023)

* The work at Oracle was part of my Master's thesis at EPFL, jointly supervised by the company manager and the university professor.
* Explored various architecture choices to optimize the data load operation in an analytical query engine while collaborating with multiple teams.
* Conducted in depth hardware performance experiments using various benchmarks to test the viability of the proposed engine architecture.
* Experimented with storage technologies, MySQL features, data storage formats, page organization and code optimization at various levels.
* Developed a prototype which scales with data size and compute, while offering more than 3x performance improvement in the load speed.

### EPFL – Lausanne, Vaud, Switzerland

> Primary project

(Research Scholar: Speculation as a part of Dynamatic, Jun 2021 – Dec 2021)

* The project was part of my work as an MSc Research Scholar at the Processor Architecture Lab (LAP) while pursuing my Masters at EPFL, Switzerland.
* Designed and tested speculation in VHDL for some benchmark example programs (test prototype for automation). 
* Automated the generation of a VHDL hardware design of speculative components from any dataflow graph (graphviz dot file).
* Designed a C++ algorithm to convert a generic design into a speculative one. This involved modifying a dataflow graph to identify speculative paths and insert special components to allow speculative execution.

> Secondary project

(Research Scholar: Optimized Designs for Speculation, Jan 2022 – Aug 2022)

* The project was part of my work as an MSc Research Scholar at the Processor Architecture Lab (LAP) while pursuing my Masters at EPFL, Switzerland.
* Improved the VHDL design of the special speculative components to be completely elastic and more generic. This allows speculative execution for any component in the dataflow graph.
* Updated and expanded the functionality of several components for speculation including the regular DFG components as well as exclusive speculation control units with intricate handshake mechanisms.
* Incorporated the new designs in the automation scripts for VHDL code generation and enabling speculative execution.

> Tertiary project

(Research Scholar: Ray Tracing Accelerator, Feb 2021 – May 2021)

* The project was part of my work as an MSc Research Scholar at the Processor Architecture Lab (LAP) while pursuing my Masters at EPFL, Switzerland.
* Integrated the modified ray-tracing software (part of my Summer@EPFL 2019 internship) with the lab’s hardware implementation of the ray-tracing accelerator.
* Designed wrapper modules for the hardware accelerator and related components in order to interface it with an improved memory controller.

## Bachelors Internships

### NTU – Singapore

> Primary project

(Research Assistant, Aug 2019 – Dec 2019)

* The internship is also my undergraduate off-campus thesis. Worked at the Hardware and Embedded Systems Lab (HESL) at NTU, Singapore.
* Worked on the hardware area-time estimation part of an FPGA tool developed at HESL, which led to a publication at the ARC-2020 conference.
* Automated the process of modifying the LegUp generated RTL code. The script replaced vendor-specific code with generic code and added the floating-point soft IP cores, thus improving performance.
* My contribution improved the tool's accuracy on floating-point benchmarks with almost zero error, and made it possible to generalize the synthesis process to multiple vendor tools (Xilinx and Quartus).

> Publication

(Springer, Cham; Mar 25, 2020)

* Technique for Vendor and Device Agnostic Hardware Area-Time Estimation
* Co-author to a conference paper which proposes a novel technique for hardware area-time estimation of applications on FPGA. The work was carried out as a part of my undergraduate thesis at the Hardware and Embedded Systems Lab at NTU, Singapore.
* Show publication: https://link.springer.com/chapter/10.1007/978-3-030-44534-8_13

> Secondary project 

(Application Runtime Prediction, Nov 2019 - Dec 2019)

* The project was carried out at the Hardware and Embedded Systems lab at NTU, Singapore. 
* Implemented a regressor neural network to predict a C application’s runtime on a Nios processor which achieved a maximum R2 score of 0.95.
* The model was trained using the instruction counts of the translated assembly code to output a single value representing the execution time in number of clock cycles. The dataset for training the neural network was generated using C programs from existing benchmarks.
* My design contributed to the lab’s future work by providing a foundation on which better models can be built and optimized.

### EPFL – Lausanne, Vaud, Switzerland
(Summer Intern, May 2019 – Jul 2019)

* The internship was a part of the Summer@EPFL 2019 program. Worked at the Processor Architecture Laboratory (LAP) at EPFL, Switzerland.
* Explored and modified a ray tracing algorithm (NORI) in order to design a hardware accelerator on FPGA. Worked on the software part to support parallelism.
* Performed timing analysis to identify the critical path for acceleration and modified the ray-tracer to handle bundles of parallel light rays. 
* Worked on designing a hardware architecture in Chisel to deploy LAP's unique memory controller capable of handling irregular accesses more efficiently.

### CSIR CEERI – Pilani, Rajasthan, India
(Summer Intern, May 2018 – Jul 2018)

* The internship was part of the Practice School program at BITS Pilani. Worked in the IC Design group at CEERI, Pilani.
* Designed and implemented a floating-point unit capable of performing basic operations on single-precision IEEE754 format floating point numbers.
* The operations (add, subtract, multiply, divide) were implemented in verilog in the form of single-cycle and pipelined modes. 
* Different modes were simulated on Modelsim, synthesized using Vivado, and compared in terms of area and timing efficiency.
* The project introduced me to RTL design and optimization, FPGA implementation and floating-point arithmetic.

## Teaching Assistantships

### Computer Architecture
(Jan 2020 – May 2020)

* The work was part of bachelors at BITS Goa, India.
* Assisted the faculty in conducting and evaluating labs and assignments for a class of 80 students.

### Microprocessor Programming and Interfacing
(Jan 2019 – Apr 2019)

* The work was part of bachelors at BITS Goa, India.
* Assisted the faculty in conducting labs and tutorials for a class of 250 students. Taught a lecture series on System Design using Proteus, and mentored some student projects.

### Digital Design
(Aug 2018 – Dec 2018)

* The work was part of bachelors at BITS Goa, India.
* Assisted the faculty in conducting labs and quizzes for a class of 50 students.

