# TryHackMe DFIR: An Introduction - Room Writeup

## Overview
This repository contains the full writeup and notes for the **[DFIR: An Introduction](https://tryhackme.com/module/digital-forensics-and-incident-response)** room on TryHackMe. 

Digital Forensics and Incident Response (DFIR) is a critical domain within defensive cybersecurity. It combines the disciplines of **Digital Forensics** (collecting, analyzing, and preserving digital evidence/artifacts from operating systems, file systems, RAM, and network logs) and **Incident Response** (evaluating security alerts, containing active threats, evicting threat actors, and restoring affected infrastructure to safe operational states).

---

## Tasks & Walkthrough

### Task 1: Introduction
- **Overview:** Introduces the DFIR module concepts and setting up the environment.

---

### Task 2: The Need for DFIR
- **Overview:** Explains why DFIR capabilities are mandatory for modern SOCs and Blue Teams. It covers detecting attacker footprints, distinguishing true positives from false alarms, determining breach scope and timeframe, and evicting threat actors.
- **Questions & Answers:**
  - **Question 2.1:** What does DFIR stand for?
    - **Answer:** `Digital Forensics and Incident Response`
  - **Question 2.2:** DFIR requires expertise in two fields. One of the fields is Digital Forensics. What is the other field?
    - **Answer:** `Incident Response`

---

### Task 3: Basic Concepts of DFIR
- **Overview:** Covers core principles including **Artifacts** (evidence pieces like registry keys, event logs, file timestamps), **Evidence Preservation** (write-blocking and analyzing copies), **Chain of Custody** (verifiable evidence tracking), **Order of Volatility** (data lifespan: RAM vs disk), and **Timeline Creation**.
- **Questions & Answers:**
  - **Question 3.1:** Complete the timeline creation exercise in the attached static site. What is the flag that you get after completion?
    - **Answer:** `THM{DFIR_REPORT_DONE}`

---

### Task 4: DFIR Tools
- **Overview:** Introduces key industry tooling:
  - **Eric Zimmerman's Tools (EZ Tools):** Suite of Windows forensic parsers for registry, file system, shellbags, and timeline analysis.
  - **KAPE (Kroll Artifact Parser & Extractor):** Automates artifact collection and parsing.
  - **Autopsy:** GUI-based open-source digital forensics platform for disk image analysis.
  - **Volatility:** Advanced memory forensics framework for RAM analysis.
  - **Redline:** FireEye memory analysis and IOC collector tool.
  - **Velociraptor:** Advanced open-source endpoint monitoring and incident response platform.

---

### Task 5: The Incident Response Process
- **Overview:** Examines the structured incident response lifecycles:
  - **SANS PICERL Model:** Preparation → Identification → Containment → Eradication → Recovery → Lessons Learned.
  - **NIST SP 800-61 Model:** Preparation → Detection & Analysis → Containment, Eradication, and Recovery → Post-Incident Activity.
- **Questions & Answers:**
  - **Question 5.1:** At what stage of the IR process are disrupted services brought back online as they were before the incident?
    - **Answer:** `Recovery`
  - **Question 5.2:** At what stage of the IR process is the threat evicted from the network after performing the forensic analysis?
    - **Answer:** `Eradication`
  - **Question 5.3:** What is the NIST-equivalent of the step called “Lessons learned” in the SANS process?
    - **Answer:** `Post-Incident Activity`

---

### Task 6: Conclusion
- **Overview:** Summarizes introductory principles and lays out the pathway for deep-dive Windows, Linux, and memory forensics modules.
