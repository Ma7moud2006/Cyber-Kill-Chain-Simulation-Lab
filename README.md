# Windows 10 Cyber Kill Chain Simulation & Incident Analysis

A comprehensive security assessment and attack simulation documenting a complete Cyber Kill Chain mapped to the **MITRE ATT&CK Framework** in an isolated lab environment.

## 🎯 Executive Summary
This project demonstrates an end-to-end attack simulation against an isolated Windows 10 (22H2) endpoint, covering the following stages:
- **Reconnaissance & Enumeration** (Nmap)
- **Credential Poisoning & Cracking** (Responder, Hashcat)
- **Initial Access & Privilege Escalation** (Evil-WinRM, Named Pipe Impersonation to SYSTEM)
- **Defense Evasion & Persistence** (Registry Run Keys, Scheduled Tasks, Startup Folder)
- **Command & Control** (Metasploit Meterpreter)
- **Credential Harvesting** (SAM Dumping)
- **Persistence Verification** (Automatic reconnect across reboots)

---

## 🛠️ Tools & Frameworks
- **Platform:** Kali Linux & Windows 10 (VMware Workstation)
- **Offensive & Testing Tools:** Nmap, Responder, Hashcat, CrackMapExec, Evil-WinRM, Metasploit Framework
- **Framework Mapping:** MITRE ATT&CK Framework

---

## 🛡️ Key Findings & Blue Team Recommendations
- **Findings:** Identified critical configuration weaknesses including disabled SMB signing, LLMNR/NBT-NS broadcast poisoning vectors, and weak credential complexity.
- **Defensive Mitigations:** Documented hardened configurations (GPO for LLMNR disabling, forced SMB signing, strong password policies) and SIEM Event ID monitoring signatures (e.g., Event IDs `4624`, `4657`, `4698`, `7045`, `4104`).

---

## 📄 Full Report
For the complete technical report, MITRE ATT&CK matrix mapping, and methodology:
👉 **[Download / View the Lab Report (PDF)](CyberKillChain_FLFL.pdf)**
