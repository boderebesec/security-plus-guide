# Indicators of Attacks — Domain 2: Threats, Vulnerabilities, and Mitigations

Focus: Understand early warning signals of malicious activity across each phase of an attack  
Purpose: Equip learners to detect intent-focused indicators and respond before full compromise

---

## Indicators of Attack (IOAs)

IOAs are early warning signals of malicious activity based on behavioral patterns and system state changes—often before full compromise or exfiltration occurs. Unlike IOCs (Indicators of Compromise), IOAs are intent-focused, making them more useful for real-time prevention and detection.

---

## 1. Indicators of Reconnaissance Activity

These signs show that an attacker is collecting information about the target environment.

Key Examples:
- External port scanning across subnets
- DNS lookups and zone transfers
- Crawling public-facing websites and employee pages
- Email enumeration and metadata harvesting
- WHOIS queries or OSINT gathering on IP ranges

Preventive Measures:
- Rate-limit queries and scans
- Block known scanning IPs
- Enable DNSSEC and configure zones correctly
- Obfuscate or hide email addresses on public pages

---

## 2. Indicators of Access Attempts

Evidence of active attempts to penetrate systems.

Behavior Patterns:
- Brute-force login attempts (many failures from a single source)
- Credential stuffing using known breach datasets
- Exploitation of unpatched service vulnerabilities
- Attempted logins with default or common credentials
- Use of legacy or deprecated protocols (e.g., Telnet, SMBv1)

Detection Methods:
- Correlate failed-login events in SIEM
- Alert on use of legacy protocols
- Monitor for anomalous privileged-account access

---

## 3. Indicators of Persistence

Once access is gained, attackers install methods to maintain long-term control.

Techniques to Watch:
- Creation of unauthorized local or domain accounts
- Registry or startup folder modifications
- Unusual scheduled tasks or cron jobs
- New or altered services running under SYSTEM
- Presence of tools like reverse shells or Cobalt Strike

Defensive Tactics:
- Baseline and monitor startup entries
- Use EDR to detect credential-store access
- Alert on nonstandard parent-child process relationships (for example, Word → PowerShell)

---

## 4. Indicators of Defense Evasion

Evidence that the attacker is attempting to remain undetected.

Common Tactics:
- Disabling antivirus or EDR components
- Modifying or clearing event logs (for example, using wevtutil or Clear-EventLog)
- Executing PowerShell with obfuscated or base64-encoded commands
- DLL side-loading or proxy execution
- Using signed-but-malicious binaries (Living Off the Land Binaries)

Mitigation Tools:
- Deploy Sysmon with Event Forwarding
- Enforce Windows Defender Application Control (WDAC)
- Correlate threat intelligence with process execution logs

---

## 5. Indicators of Exfiltration or Impact

These represent the attacker’s endgame—data theft or service disruption.

Signs to Track:
- Spikes in outbound traffic to unrecognized IPs or regions
- Use of uncommon ports or protocols (for example, DNS tunneling or ICMP)
- Archiving tools (7-Zip, WinRAR) invoked in nonstandard directories
- File renaming or encryption patterns indicative of ransomware
- Sudden shutdowns, reboots, or service failures

Mitigations:
- Implement DLP policies with content inspection
- Use zero-trust network access (ZTNA) and strict outbound ACLs
- Analyze network flows (NetFlow, Zeek)
- Monitor cloud egress points for anomalous activity

---

## Summary

| Phase               | Example Indicator                      | Detection Strategy                   |
| ------------------- | -------------------------------------- | -------------------------------------|
| Reconnaissance      | Repeated DNS lookups or port scans     | Firewall/IDS logs                    |
| Access Attempts     | Brute-force login from foreign IP      | SIEM correlation rules              |
| Persistence         | New account created during off-hours   | EDR and Active Directory monitoring |
| Defense Evasion     | Termination of antivirus processes     | EDR behavioral analytics            |
| Exfiltration/Impact | Outbound archive to unlisted IP        | DLP + anomaly detection             |

---

## References

- MITRE ATT&CK: Enterprise Techniques — https://attack.mitre.org/  
- NIST SP 800-94 – Intrusion Detection and Prevention — https://doi.org/10.6028/NIST.SP.800-94  
- CompTIA SY0-701 Exam Objectives — https://www.comptia.org/certifications/security  
