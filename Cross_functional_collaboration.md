## 📁 Cross functional collaborations (STAR Method)
*Post silicon involvement*

<details>
<summary><b>🛠️ Silicon Reliability & Burn-in Fix </b></summary>

* **Situation:** Silicon failed reliability tests after three days of burn-in due to an unexpected MCU sleep mode during FW inactivity.
* **Task:** Identify the root cause of the BIST-mode failure and implement a hardware fix for the B0 silicon revision.
* **Action:** Collaborated with Post-Silicon Validation to diagnose the FW/HW conflict, updated the B0 design to shut down the MCU during these cycles, and added debug straps for future visibility.
* **Result:** Fix verified across all corners in GLS, resulting in a **100% success rate** for the production chip.
* **Impact:** **Ensured 100% production-ready silicon for the B0 revision** and established a permanent validation procedure for all subsequent MCU-based SoCs.
* **Takeaway:** Post-silicon success requires a "big picture" understanding of how firmware and hardware interact under extreme reliability conditions.
</details>
