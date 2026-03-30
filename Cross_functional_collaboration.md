## 📁 Cross functional collaborations (STAR Method)
*Post silicon involvement*

<details>
<summary><b>🔍 High-Stakes GLS Debug & ECO </b></summary>

* **Situation:** During the final sign-off phase, SoC-level Gate-Level Simulation (GLS) failed for a critical IP, despite passing all functional RTL verification. The failure was traced to a contradiction between the RTL and the physical netlist regarding flop retention behavior.
* **Task:** Identify the root cause of the behavior mismatch and implement an Emergency Change Order (ECO) to resolve the discrepancy without delaying the fast-approaching tape-out.
* **Action:** I performed a deep-dive debug and discovered the issue originated in the **Unified Power Format (UPF)** list definitions, which the synthesis tool had failed to recognize. As the IP Design Lead, I took sole responsibility for the resolution:
    * Proposed a strategic workaround to modify the register behavior, bypassing the synthesis limitation.
    * Manually implemented the ECO across all levels of netlists to save critical implementation time.
    * Guided for **Logical Equivalence Checking (LEC)** to ensure the fix was functionally perfect.
* **Result:** Successfully synchronized the RTL, UPF, and Netlist behavior, allowing the SoC to meet its sign-off milestones on schedule. I subsequently updated the master RTL and UPF libraries to prevent recurrence in future product generations.
* **Impact:** **Prevented a major tape-out delay** by taking technical ownership beyond my standard scope and received management recognition for rapid, high-pressure problem-solving.
* **Takeaway:** Senior leadership is defined by the ability to remain calm under extreme tape-out pressure and provide optimal, "out-of-the-box" solutions. By going above and beyond my defined role to manage the ECO and LEC personally, I ensured the team overcame a critical crisis that could have resulted in a multi-week schedule slip.
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
<summary><b>🔌 USB Downstream Port-Power & Over-Current Sense (OCS) Optimization</b></summary>

* **Situation:** USB2 and USB3 downstream ports utilized a shared-pin configuration for Port Power and Over-Current Sense (OCS). The RTL used a 4ms timer to filter OCS events (where a weak zero signaled an over-current event) to ensure valid reporting for power-off sequences.
* **Task:** Resolve a post-silicon failure where the initial power ramp-up on the VBUS line was being incorrectly identified as a valid OCS event, causing the ports to fail to power up properly.
* **Action:** Diagnosed that the initial voltage ramp lasted longer than the 4ms RTL filter, creating a false-positive OCS trigger. I redesigned the RTL to include a dedicated 10ms debounce timer at the start of the power-on sequence to mask the initial power surge.
* **Result:** Successfully validated the fix in post-silicon, ensuring downstream ports powered up correctly without false over-current triggers.
* **Impact:** **Ensured 100% functional reliability of USB power delivery** across all downstream ports and established a robust hardware debounce methodology for shared-pin power/sense architectures.
* **Takeaway:** Post-silicon validation requires a deep understanding of analog electrical characteristics (like power ramp-up) that are often simplified in RTL and Gate-Level Simulations (GLS).
</details>
