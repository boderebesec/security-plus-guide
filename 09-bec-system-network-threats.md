# BEC, System Threats & Network Threats — Domain 2: Threats, Vulnerabilities, and Mitigations

Focus: Understand how email-, host-, and network-based attacks operate  
Purpose: Equip learners to identify and mitigate common communication, system, and network threats

---

## Business Email Compromise & Communication-Based Threats

Business Email Compromise relies on impersonation and urgency to trick victims into wiring funds or disclosing information.

Common methods include:  
- **Phishing** – generic bulk emails designed to steal credentials or deliver malware  
- **Spear Phishing** – highly targeted messages using personalized details  
- **Whaling** – attacks aimed at executives or high-value targets  
- **Vishing** – voice-based phishing over phone calls  
- **Smishing** – SMS-based phishing via text messages  
- **Pretexting** – fabricating scenarios to manipulate victims  
- **Pharming** – redirecting users to malicious websites  

BEC attacks usually use social engineering alone—no malware payloads.

---

## System-Based Attacks

These target endpoints, servers, or application vulnerabilities.

Key threats:  
- **Ransomware** – encrypts files and demands payment, sometimes exfiltrating data first  
- **Rootkits** – stealthy malware that hides in OS kernels or firmware  
- **Backdoors** – hidden access points that bypass normal authentication  
- **Logic Bombs** – dormant code triggered by specific events or dates  
- **Credential Dumping** – extracting passwords or hashes from memory (e.g., LSASS)  
- **Privilege Escalation** – exploiting flaws to gain higher privileges (horizontal or vertical)  
- **Fileless Malware** – runs in memory via legitimate tools (PowerShell, WMI)

Persistence and lack of hardening amplify these risks.

---

## Network-Based Attacks

These exploit weaknesses in data flows and network configurations.

Primary vectors:  
- **Denial-of-Service (DoS/DDoS)** – overwhelming resources (TCP/UDP floods, application-layer attacks)  
- **Man-in-the-Middle (MitM)** – intercepting or altering traffic (SSL stripping, rogue gateways)  
- **Session Hijacking** – stealing valid session tokens or cookies  
- **Replay Attacks** – resending intercepted data to bypass authentication  
- **MAC Flooding & ARP Poisoning** – forcing switches into hub mode or redirecting traffic  
- **DNS Poisoning** – corrupting DNS caches to redirect users  
- **Rogue Access Points & Evil Twins** – fake Wi-Fi networks to harvest credentials  

Misconfigured devices, unencrypted traffic, and flat networks multiply these threats.

---

## Review Insights

- BEC is purely social engineering—no malware required  
- Credential theft often kick-starts deeper system compromise  
- Network attacks go unnoticed without active monitoring (IDS/IPS)  
- Core defenses: MFA, least privilege, patch management, segmentation, strong filtering

---

## References

- CompTIA SY0-701 Exam Objectives: https://www.comptia.org/certifications/security  
- MITRE ATT&CK Framework – Credential Access (TA0006): https://attack.mitre.org/tactics/TA0006/  
- CISA Business Email Compromise: https://www.cisa.gov/news-events/news/business-email-compromise 