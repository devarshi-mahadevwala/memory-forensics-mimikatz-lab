# Memory Forensics Project – Mimikatz & Volatility

## 📌 Overview
This project demonstrates a real-world memory forensics workflow by simulating a credential theft attack using **Mimikatz** and analyzing system memory using **Volatility**.

Three memory snapshots were captured:
- **Pre-Attack**
- **During Attack**
- **Post-Attack**

These dumps were analyzed to identify malicious activity, credential artifacts, and attacker traces.

---

## 📄 Final Report (Primary Deliverable)
👉 **[Final Memory Forensics Report](./Final-Report/Memory_Forensics_Final_Report.pdf)**

This report contains:
- Environment setup
- Attack execution
- Memory acquisition methodology
- Volatility analysis
- Comparison of all three memory dumps
- Key forensic findings

---

## 🧪 Project Phases

### Phase 1 – Environment Setup
- Kali Linux attacker VM
- Windows 10 victim VM
- Isolated host-only network

📂 `Phase-1-Setup/`

---

### Phase 2 – Attack & Memory Acquisition
- Payload staging via HTTP
- Execution of Mimikatz
- Memory dumps captured at three stages
- Secure transfer of dumps to Kali

📂 `Phase-2-Attack/`

---

### Phase 3 – Memory Forensics Analysis
- Volatility 3 analysis
- Process, credential, and artifact investigation
- Timeline correlation

📂 `Phase-3-Volatility/`

---

## 📊 Presentation
📂 `Final-Presentation/`

---

## 🛠 Tools Used
- Mimikatz
- DumpIt
- Volatility 3
- Kali Linux
- Windows 10
- VMware Workstation

---

## 👤 Author
**Devarshi Mahadevwala**  
Postgraduate – Cybersecurity & Threat Management  
Seneca Polytechnic
