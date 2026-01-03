# Memory Forensics Investigation Project  

This repository contains a complete end-to-end **Memory Forensics investigation**.  
The project simulates a real-world incident involving credential harvesting using Mimikatz, followed by forensic analysis using Volatility.

> 📌 **Start here:**  
> - 📄 **Final Report (PDF):** `Memory Forensics Project- Final Report.pdf`  
> - 📊 **Final Presentation:** `Memory Forensics Project- Final presentation.pptx`

---

## 📄 Final Deliverables (Primary Focus)

These files summarize the entire investigation and should be reviewed first:

- **Memory Forensics Project – Final Report (PDF)**  
  → Complete technical report covering setup, attack execution, memory acquisition, and forensic analysis

- **Memory Forensics Project – Final Presentation (PPTX)**  
  → Condensed version of the project for walkthroughs and presentations

---

## 🧠 Project Overview

This project follows a structured incident response workflow:

1. **Phase 1 – Environment Setup**
2. **Phase 2 – Live Attack & Memory Acquisition**
3. **Phase 3 – Memory Forensics Analysis (Volatility 3)**

Three separate memory dumps were collected:
- **Pre-attack**
- **During attack**
- **Post-attack**

These dumps were analyzed and compared to identify malicious activity and system state changes.

---

## 🗂 Repository Structure

project/
├── Phase 1 setup/
│   ├── screenshots/
│   ├── Memory Forensics Project Phase 1.docx
│   └── Memory Forensics Project Phase 1.pptx
│
├── phase 2 attack/
│   ├── screenshots/
│   └── Memory Forensics Project Phase 2.pptx
│
├── phase 3 volatility/
│   ├── screenshots/
│   └── Memory Forensics Project Phase 3.pptx
│
├── Project detail and workflow/
│   └── Memory Forensics Project Week 1.pptx
│
├── Memory Forensics Project- Final Report.docx
├── Memory Forensics Project- Final Report.pdf
├── Memory Forensics Project- Final presentation.pptx
└── README.md

---

## 🔧 Phase 1 – Environment Setup

**Objective:** Prepare a controlled lab environment for attack simulation and forensic analysis.

Key tasks:
- Configured **Kali Linux (Attacker & Forensics VM)** and **Windows 10 (Victim VM)**
- Verified network connectivity between VMs
- Disabled Windows Defender and firewall (lab-only environment)
- Installed required tools:
  - DumpIt
  - Mimikatz
  - Volatility 3
- Created clean **baseline snapshots** of both VMs

📁 Supporting material:
- `Phase 1 setup/`
- `Phase 1 setup/screenshots/`

---

## ⚔️ Phase 2 – Attack Execution & Memory Acquisition

**Objective:** Simulate credential harvesting and capture memory at critical points.

Actions performed:
- Hosted attack tools using an HTTP server on Kali
- Transferred tools to the Windows victim
- Executed **Mimikatz** to access credential-related memory
- Captured **three memory dumps** using DumpIt:
  - Pre-attack
  - During attack
  - Post-attack
- Safely transferred all memory dumps to Kali for analysis

📁 Supporting material:
- `phase 2 attack/`
- `phase 2 attack/screenshots/`

---

## 🔍 Phase 3 – Memory Forensics Analysis (Volatility)

**Objective:** Analyze memory dumps and identify malicious artifacts.

Analysis performed using **Volatility 3**, including:
- Process listing (`pslist`, `pstree`)
- Network connections (`netstat`)
- Handle analysis
- DLL inspection
- Process relationship comparison across all three dumps
- Identification of:
  - DumpIt execution
  - Mimikatz activity
  - LSASS interaction
  - Post-attack artifacts

📁 Supporting material:
- `phase 3 volatility/`
- `phase 3 volatility/screenshots/`

---

## 🧪 Tools Used

- Kali Linux
- Windows 10
- DumpIt
- Mimikatz
- Volatility 3
- VMware Workstation

---

## 🎯 Key Learning Outcomes

- Live memory acquisition during an active attack
- Forensic comparison across multiple memory states
- Detection of credential harvesting activity
- Practical Volatility 3 usage
- Incident response workflow execution

---

## ⚠️ Disclaimer

This project was conducted **strictly in an isolated lab environment** for academic purposes.  
All tools and techniques demonstrated here are intended for **defensive security research and learning only**.

---

## 👤 Author

**Devarshi Mahadevwala**  
Postgraduate Student – Cybersecurity & Threat Management  
