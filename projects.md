# Academic Projects

## Masters at EPFL

### PowerSGD with Hybrid Block Floating Point
(Mar 2022 - Jun 2022)

* Tested the viability of gradient compressed HBFP and pushed the limits of using PowerSGD alongside HBFP.
* Ran several image classification experiments on a 2-GPU cluster to conclude consistent improvement in accuracy over plain HBFP, in addition to the advantage of compressed gradients.
* Experiments covered multiple ResNet and DenseNet models on the CIFAR dataset to explore various model and dataset sizes, and draw independent conclusions for varying hyperparameters.
* Achieved excellent accuracy, comparable with the floating point counterpart, even for large models with a reasonable mantissa size, upto HBFP-6.

### Gradient Compression with New Numerical Encodings 
(Oct 2021 - Dec 2021)

* The project was part of the Advanced Multiprocessor Architecture course at EPFL, Switzerland.
* Investigated the effectiveness of gradient compression on DNN models which are trained on a hardware emulator that uses hybrid block floating point encoding instead of the standard floating point.
* Integrated the PowerSGD compression algorithm and HBFP Emulator utility functions (EPFLML \& PARSA labs, EPFL) to emulate specific tensors and multiplication operations in BFP format.
* Extended the Python scripts for PowerSGD to support BFP emulation using rounding and truncation operations. Tested the design with several image classification experiments using ResNet18 model on the CIFAR10 dataset with different combinations of mantissa sizes and gradient reducer ranks. 
* Achieved an accuracy of about 94\% with HBFP (cf. 94.7\% with FP) despite using a lower precision encoding of 4 bits only, when using a reasonable mantissa size and reducer rank.
* Implemented a preliminary RTL design for the gradient compression hardware block which will serve as the foundation for integrating HBFP on a GPU cluster.

### Actors / Directors Constellation
(May 2021 - Jun 2021)

* The project was part of the Data Visualization course at EPFL, Switzerland.
* Visualized and presented the relationship between directors and actors from various IMDb movies, through an interactive website, featuring a graph network and side bar charts.
* Extracted and processed data from multiple datasets using standard Python libraries. The website was primarily designed using JavaScript, and supported by HTML and CSS.
* Implemented the main visualization, animations and several features using D3.js libraries and Jekyll tools, allowing scope for future improvements.
* Show project: https://com-480-data-visualization.github.io/data-visualization-project-2021-datavizards/

### L3 Compiler and M&S Garbage Collector
(Apr 2021 - Jun 2021)

* The project was part of the Advanced Compiler Construction course at EPFL, Switzerland.
* Implemented a compiler for a Lisp-Like-Language (L3) from a project skeleton in Scala. The design involved multiple steps – desugaring, IR translation, closure conversion and various optimizations.
* Implemented a mark-and-sweep garbage collector in C for the L3 virtual machine. The method was designed to trigger whenever there are no more memory blocks left to be allocated.
* Involved the design of efficient data structures to manage the memory as well as splitting and coalescing blocks to optimize the memory space.

### Spectre Attack
(May 2021 - Jun 2021)

* The project was part of the Advanced Computer Architecture course at EPFL, Switzerland.
* Performed a spectre attack on a victim function in C, and demonstrated a microarchitectural side-channel attack capable of stealing data from any memory location.
* The attack required training the branch predictors to mis-speculate load instructions and delay the branch resolution so that the data traces in the cache can be exploited.
* Executed a standard prime + probe cache attack to illegally read data from the memory. Various parameters in the algorithm were fine tuned for the machine to provide consistently competitive results.

### Deep Learning Framework
(Apr 2021 - May 2021)

* The project was part of the Deep Learning course at EPFL, Switzerland.
* Designed a mini deep learning framework from scratch using only PyTorch’s tensor operations and the math library (without autograd or the neural-network modules). 
* Implemented the forward and backward pass algorithms including the Linear, ReLU, Tanh and sequential layers with an MSE Loss metric and SGD optimizer.
* Tested the frameworks using multiple models and a custom dataset. Tested different weight initialization methods and parameters to achieve competitive test error rates of about 1.5\%.

### Digit Image Classification
(Apr 2021 - May 2021)

* The project was part of the Deep Learning course at EPFL, Switzerland.
* Implemented multiple network architectures using PyTorch modules to compare two digits visible in a two-channel image (MNIST dataset).
* Performed experiments to study the improvements achieved using weight sharing and auxiliary losses. Further improved the performance using various ML techniques, notably, dropout and skip connections.
* A convolutional model with skip connections, weight sharing and auxiliary losses achieved the best performance with an error rate of 8.28 ± 0.84 %.

### Distributed Execution of Near-Neighbour Algorithms
(Apr 2021 - May 2021)

* The project was part of the Database Systems course at EPFL, Switzerland.
* Implemented multiple near-neighbour algorithms in Scala over Apache Spark, and evaluated the performance and accuracy to confirm theoretical hypotheses.
* Designed a Locality Sensitive Hashing (LSH) based method which uses MinHash to compute approximate results. This implementation performed much faster than the naïve implementation.
* Improved the algorithm – using load balancing, broadcasting, AND OR composition – and analysed the results to discover specific scenarios where each improvement gives the best results. 
* Experiments were performed based on Jaccard similarity on a movie dataset containing a list of keywords for each entry. Multiple datasets, queries and seed values were tested iteratively on a 10-node cluster.

### HLS Design Optimization
(Apr 2021 - May 2021)

* The project was part of the Advanced Computer Architecture course at EPFL, Switzerland.
* Performed area‑timing analysis for several loop kernels using Vivado HLS for naïve and optimized implementations of the designs.
* Optimized the HLS designs to improve timing with minimal effect to area utilization while keeping the same clock speed.
* Involved refactoring of the C++ code and use of HLS pragmas for optimized design, along with TCL scripts to ensure reproducible results.
* Achieved best performance (II=1) for most kernels. Proved why some kernels cannot be improved further with given area limitations.

### Out-of-Order Processor
(Mar 2021 - Apr 2021)

* The project was part of the Advanced Computer Architecture course at EPFL, Switzerland.
* Implemented a cycle‑accurate simulator of an out‑of‑order processor in python based on the MIPS R10000 microarchitecture and RISC‑V ISA.
* Implemented RTL stages to read an assembly code, update internal data structures to dynamically extract parallelism and execute the program.
* Designed several data structures to closely mimic hardware storage and accurately represent the microarchitectural state of the processor.
* Capable of reading multiple instructions per cycle, resolving dependencies and using forwarding paths, and recovering from precise exceptions.

### VLIW Processor Scheduler
(Mar 2021 - Apr 2021)

* The project was part of the Advanced Computer Architecture course at EPFL, Switzerland.
* Implemented a cycle‑accurate scheduler for a VLIW processor in python based on the Intel Itanium microarchitecture and RISC‑V ISA loop ops.
* Used a special loop op with architectural support for software pipelining through predication, rotating registers and specialised data structures.
* Designed a scheduling algorithm using the ASAP heuristic, while taking into account dependency analysis and register allocation.
* Capable of generating optimized VLIW schedules with and without the use of software pipelining for an input assembly program.

### Database Engine
(Feb 2021 - Mar 2021)

* The project was part of the Database Systems course at EPFL, Switzerland.
* Implemented a full-fledged database engine in Scala capable of processing input queries on large datasets efficiently.
* Implemented six operators (scan, filter, project, join, aggregate, sort) in a volcano-style model which handles a tuple-at-a-time. Further, the engine was was modified to support RLE encoding by implementing the decode and reconstruct operators.
* Optimized the engine to execute the queries in a certain order using Apache Calcite as the query parser and optimizer.
* Converted the tuple-oriented model to a column-oriented model by using selection vectors and mapping functions in all the basic operators. Such a model extends support to DSM page layout.
* Using appropriate data structures and efficient algorithms, the database engine ranked among the top 10 fastest implementations in class.

### Camera-to-LCD Display System
(Nov 2020 - Dec 2020)

* The project was part of the Embedded Systems course at EPFL, Switzerland.
* Implemented an Altera DE0-Nano-SoC based system for capturing image frames using the TRDB-D5M camera, and displaying them live on the LT24 LCD display.
* The camera and LCD controllers were implemented as custom IP cores in VHDL to work independently from each other. This was achieved by using a simple C program to manage external DDR3 buffers for reading and writing image frames.
* My contribution was designing the camera controller capable of acquiring image frames pixel-by-pixel, processing them and storing them into the memory in proper order. The memory transfer was done on an Avalon bus using DMA burst transfer. 
* The design was optimized to use FIFOs to decouple various stages, and generate Avalon control signals using a finite-state-machine.

### Extended ROBDD Package
(Nov 2020 - Dec 2020)

* The project was part of the Design Technologies for Integrated Systems course at EPFL, Switzerland.
* Studied the theoretical and practical aspects of using Reduced Order Binary Decision Diagrams (ROBDD) to represent digital logic functions. Extended an ROBDD package, written in C++, by adding three new features.
* Improved the memory efficiency by enabling complemented edges for a more efficient representation, and implementing a node reference counter to help in garbage collection. 
* Improved the timing efficiency by using operation caches to store the most recent operation results.

### Languages' influence on social networks
(Nov 2020 - Dec 2020)

* The project was part of the Applied Data Analysis course at EPFL, Switzerland. 
* Studied and extended the results presented in the 'Testing Proportions from Twitter Studies..' paper (Liang H & Fu K-w, 2015). 
* Processed and visualised the data for users’ behaviour on Twitter to find any interesting patterns. Studied the influence of a Twitter user’s language on their behaviour on Twitter in terms of online presence, networking patterns and activity.
* Presented the findings by a specific case study between the users from western and eastern countries, in the form of a jupyter notebook and a web page.
* Show project: https://rayacers.github.io/language-social-network-pattern/

### Clock as a Custom IP Component
(Oct 2020 - Oct 2020)

* The project was part of the Embedded Systems course at EPFL, Switzerland.
* Designed a specific programmable interface for the Altera DE0-Nano-SoC to display the time on a 6-digit 7-segment LED display. 
* Implemented a custom slave IP component in VHDL to display the locally generated time or a manually entered value via the Avalon interface.
* This required careful calibration of the counters at the correct frequency, not only to generate the real time, but also to maintain the correct frequency for enabling the LED segments one-at-a-time.

### Servomotor control
(Sep 2020 - Sep 2020)

* The project was part of the Embedded Systems course at EPFL, Switzerland.
* Designed an embedded system in C to control a servomotor using potentiometer input demonstrating basic timer and interrupt concepts.
* Programmed the MSP432 to read potentiometer input using the ADC, translated it to a variable duty PWM cycle using the timer and set the output as the rotation angle of a servomotor.


## Bachelors at BITS

### MIPS-like Processor Design
(Feb 2019 - Apr 2019)

* The project was part of the Computer Architecture course at BITS Goa, India. 
* Developed a MIPS-like processor in verilog as two different architectures – single-cycle processor (with 8 instructions) and 4-stage pipeline processor (with 3 instructions).
* Designed the processor’s components (data path, control unit, instruction memory, arithmetic logic unit and register file) from scratch, and simulated on Modelsim.

### FMCW Radar Signal Processing Unit
(Jan 2018 - Dec 2018)

* The project was carried out at the Reconfigurable Computing lab of BITS Goa, India.
* Designed an efficient algorithm to plot an accurate spectrogram for conditioned reflectometry data. It was tested and simulated on MATLAB. 
* Implemented multiple approaches using different signal processing concepts – butterworth filter, cubic spline interpolation, wavelet decomposition and empirical mode decomposition. 
* Designed a python GUI for an interactive execution of the algorithm. This helped in studying and comparing the performance of different approaches. 
* Optimized the algorithm to allow hardware implementation on FPGA.

### Smart Library System
(Sep 2018 - Nov 2018)

* The project was part of the Embedded System Design course at BITS Goa, India.
* Implemented two separate components – noise detection and seat vacancy detection – on Arduino Mega units. 
* Mounted each unit to a table and programmed it to read audio sensor and load mat readings. The noise level was interpreted and displayed using an LED array directly.
* The data from each Arduino unit was collected by a master LPC2378 board, and forwarded to an HTML webpage via the ethernet interface.

### Voice Scrambler and Descrambler
(Oct 2018 - Nov 2018)

* The project was part of the Digital Signal Processing course at BITS Goa, India. 
* Implemented a DSP unit on the TI C6748 kit that scrambles a voice signal using a specific key before transmission. The received signal can be descrambled using the exact same algorithm and the given key. 
* The algorithm involved accurate low-pass filters and modulation of the generated sine-wave signals. The design was tested and simulated on MATLAB.

### Music Control System
(Sep 2018 - Oct 2018)

* The project was part of the Embedded System Design course at BITS Goa, India.
* Designed a music control system on LPC2378 using the standard Keil mu-vision libraries to play mp3 files from an SD card.
* The files were read onto the board using USB interface, and the board’s hardware was used for sound, display and volume control.
* Designed an interactive display in the form of a python GUI to control the music system.

### Light and Temperature monitoring
(Aug 2018 - Sep 2018)

* The project was part of the Embedded System Design course at BITS Goa, India.
* Designed an embedded system on Arduino Mega to receive light and temperature data from LM35 and LDR sensors. 
* Automated the data collection using python scripts, and designed a python GUI to access the data.

### Automated Lawn Sprinkler System
(Apr 2018 - May 2018)

* The project was part of the Microprocessor Programming and Interfacing course at BITS Goa, India.
* Simulated the design of an 8086 based Automated Lawn Sprinkler System on Proteus 8.7 using the specifications of actual hardware.
* It involved I/O mapping, memory mapping, clock generation, and interrupt handling. The system was designed using the MASM Assembly language.

### Messaging System using Radio Frequency Waves
(Nov 2017 - Dec 2017)

* The project was part of the Electromagnetic Theory course at BITS Goa, India. 
* Programmed an RF transceiver and Arduino Uno boards to generate and receive message in the form of RF waves. 
* Demonstrated the plane polarized nature of electromagnetic waves and tested the range of the system experimentally.
