## 📁 Featured Case Studies (STAR Method)
*High-impact technical challenges and leadership outcomes:*

<details>
<summary><b>🚀 CDC/RDC Methodology Optimization </b></summary>

* **Situation:** Traditional CDC analysis tools were insufficient for complex SoC-level verification, often missing critical IP-level constraints.
* **Task:** Lead the transition to **VC SpyGlass** (AI/ML supported) and implement a robust SoC-level flow without existing IP constraints.
* **Action:** Independently spearheaded the implementation of the VC SpyGlass flow and presented data-driven benchmarks to stakeholders to secure organizational buy-in.
* **Result:** Improved design analysis efficiency by **30%** and established a standardized CDC flow now utilized across multiple SoC teams.
* **Impact:** **Successfully established a high-coverage verification baseline** that is now the blueprint for other SoC teams within the firm, ensuring scalable growth.
* **Takeaway:** Proactive adoption of advanced EDA capabilities and cross-team standardization is the key to managing the verification complexity of next-generation SoCs.
</details>

<details>
<summary><b>⚡ High-Yield PPA Optimization </b></summary>

* **Situation:** A high-performance PSoC family required extreme power efficiency for real-time IoT and machine learning applications.
* **Task:** As the SoC Integrator, I was responsible for reducing dynamic power consumption while maintaining performance across complex power domains.
* **Action:** Implemented advanced low-power design techniques and modular RTL refactoring, segregating the design into standalone IPs with independent power formats.
* **Result:** Achieved a **20% reduction in dynamic power consumption** and increased design configuration flexibility by **60%**.
* **Impact:** **Delivered industry-leading power efficiency** for the product line and enabled a **60% improvement in design reusability** for future derivative SoCs.
* **Takeaway:** Strategic modularization of RTL not only solves immediate PPA targets but creates a long-term "design for reusability" framework that accelerates future product cycles.
</details>

<details>
<summary><b>🔍 Critical LEC/UPF Debug & ECO </b></summary>

* **Situation:** "X" propagation issues were discovered in Gate-Level Simulation (GLS), threatening the project timeline.
* **Task:** As the IP Design Lead, I took ownership of the design fix, UPF updates, and proving Logical Equivalence (LEC).
* **Action:** Identified that UPF constraints failed to recognize flop retention behavior; collaborated with the Architect to switch to non-retention flops and implemented the ECO across 6 netlists.
* **Result:** Secured **LEC equivalence** in a critical timeframe, ensuring first-pass silicon success.
* **Impact:** **Received formal recognition and applause from upper management** for proactive problem-solving that saved the project schedule.
* **Takeaway:** Deep technical ownership and the ability to bridge the gap between RTL, UPF, and Physical Design are critical for resolving high-stakes sign-off bottlenecks.
</details>

<details>
<summary><b>🛠️ Silicon Reliability & Burn-in Fix </b></summary>

* **Situation:** Silicon failed reliability tests after three days of burn-in due to an unexpected MCU sleep mode during FW inactivity.
* **Task:** Identify the root cause of the BIST-mode failure and implement a hardware fix for the B0 silicon revision.
* **Action:** Collaborated with Post-Silicon Validation to diagnose the FW/HW conflict, updated the B0 design to shut down the MCU during these cycles, and added debug straps for future visibility.
* **Result:** Fix verified across all corners in GLS, resulting in a **100% success rate** for the production chip.
* **Impact:** **Ensured 100% production-ready silicon for the B0 revision** and established a permanent validation procedure for all subsequent MCU-based SoCs.
* **Takeaway:** Post-silicon success requires a "big picture" understanding of how firmware and hardware interact under extreme reliability conditions.
</details>

<details>
<summary><b>⚙️ Complex LEC Runtime Optimization </b></summary>

* **Situation:** A critical IP integration faced massive LEC runtime issues (8+ hours), which were deemed a "real challenge" even for tool experts.
* **Task:** Reduce verification turnaround time and resolve tool performance bottlenecks using alternate solvers.
* **Action:** Debugged and identified a critical RTL vector assigned a default 'X' value instead of '0'; customized tool settings to debug the comparison points more effectively.
* **Result:** Reduced verification time from 8 hours to **6 hours**.
* **Impact:** **Applauded by both Synopsys and the SoC project team** for identifying a tool-level resolution to a complex integration roadblock.
* **Takeaway:** Continuous learning and collaboration with EDA partners are cornerstones of effective problem-solving in advanced digital design.
</details>
