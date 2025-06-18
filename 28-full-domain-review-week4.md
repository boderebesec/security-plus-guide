# Security+ SY0-701 — Domain 4 Full Review  
**Topic:** Security Operations    

---

## Purpose of Security Operations

Security Operations is the backbone of modern cybersecurity practice. It encompasses monitoring, incident response, vulnerability management, secure configuration, identity lifecycle, automation, and forensics—ensuring systems are hardened, observed, and resilient to threats. This domain aligns closely with real-world SOC tasks and incident-readiness frameworks.

---

## 1. Secure Configuration & Hardening

- **System Hardening:** Disable unused services/ports; enforce strong passwords; restrict permissions  
- **Baselining:** Establish a secure system image and enforce uniformity across environments  
- **Mobile/Wireless Security:**  
  - Use MDM for app control and remote wipe  
  - Enforce WPA3, disable WPS, monitor rogue APs  
- **Sandboxing:** Isolate risky or unknown applications in VMs or containers  

---

## 2. Application Security

- **Secure SDLC:** Embed security into design, code review, testing, deployment, and maintenance  
- **Code Testing:** SAST, DAST, IAST, SCA  
- **OWASP Top 10:** Address risks such as injection, broken auth, insecure deserialization  
- **Mitigations:** Input validation; parameterized queries; least-privilege service accounts; WAFs  

---

## 3. Asset Management

- **Inventory:** Track hardware, software, and data assets  
- **Lifecycle Control:** Document acquisition → tagging → classification → disposal  
- **CMDB Integration:** Centralize asset status with change logs and vulnerability data  
- **Rogue Detection:** Scan for unauthorized or unmanaged devices  

---

## 4. Vulnerability Management

- **Scan Types:** Internal vs. external; authenticated vs. unauthenticated; agent vs. agentless  
- **Cadence:** Weekly, monthly, and post-change scans  
- **Prioritization:** Combine CVSS scores with asset criticality  
- **Remediation & Validation:** Patch, re-test, and document fixes  
- **Tools:** Nessus, OpenVAS, Qualys, Microsoft Defender for Endpoint  

---

## 5. Monitoring, Logging & Alerts

- **Log Sources:** Endpoints, firewalls, authentication systems, applications, DNS  
- **Tools:** Syslog/journald, telemetry agents, SIEM platforms  
- **Practices:** NTP time-sync; centralized log forwarding; role-based log access; retention compliance  

---

## 6. Identity & Access Management

- **Onboarding/Offboarding:** Automate joiner-mover-leaver workflows (SCIM/HRIS)  
- **SSO:** Single login across services (SAML, OIDC)  
- **PIM/PAM:** Just-in-time elevation, session recording, credential vaulting  
- **MFA:** TOTP, push notifications, biometrics  
- **Access Models:** RBAC and ABAC  

---

## 7. Scripting & Automation

- **Benefits:** Reduce errors; accelerate response; scale controls  
- **Tools:** Bash, Python, PowerShell, Ansible, SOAR  
- **Use Cases:** Automatic firewall updates; account suspension; asset discovery; alert enrichment  

---

## 8. Incident Response & Recovery

- **Phases:** Preparation → Detection & Analysis → Containment → Eradication → Recovery → Lessons Learned  
- **Playbooks:** Predefined response steps for common scenarios  
- **Containment:** Isolate affected systems and network segments  
- **Eradication:** Remove malware and unauthorized access  
- **Recovery:** Restore from clean backups; verify system integrity  

---

## 9. Digital Forensics & Log Analysis

- **Forensics Phases:** Identification → Preservation → Analysis → Reporting  
- **Evidence Handling:** Write-blockers; hash verification (MD5/SHA-256); chain-of-custody  
- **Volatile Data:** Capture RAM, processes, and network connections first  
- **Tools:** Autopsy, FTK Imager, Volatility, Wireshark  
- **Log Analysis:** Correlate audit trails, login events, and file-integrity alerts  

---

## Summary Table

| Area                         | Focus                                  | Tools/Methods                               |
| -----------------------------| -------------------------------------- | -------------------------------------------- |
| Configuration & Hardening    | Lock down systems                      | Baselines, CIS Benchmarks, sandboxing       |
| Application Security         | Prevent exploitable code               | SDLC, SAST/DAST, OWASP Top 10               |
| Asset Management             | Maintain full visibility               | CMDB, automated discovery                   |
| Vulnerability Management     | Discover and remediate weaknesses      | CVSS prioritization, automated scans        |
| Monitoring & Logging         | Detect anomalies and audit activities  | SIEM, syslog, NTP, telemetry                |
| IAM                          | Control identities and privileges      | SSO, PIM/PAM, MFA, RBAC/ABAC                |
| Scripting & Automation       | Streamline operations and response     | Python, PowerShell, Ansible, SOAR           |
| Incident Response & Recovery | Handle incidents methodically          | NIST IR lifecycle, playbooks                |
| Forensics & Log Analysis     | Preserve and analyze evidence          | Imaging, memory dumps, hash verification    |

---

## References

- NIST SP 800-61r2: Computer Security Incident Handling Guide  
  https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf  
- NIST SP 800-86: Guide to Integrating Forensic Techniques  
  https://csrc.nist.gov/publications/detail/sp/800-86/final  
- OWASP Top 10  
  https://owasp.org/www-project-top-ten/  
- MITRE ATT&CK Framework  
  https://attack.mitre.org/  
- CompTIA Security+ SY0-701 Objectives  
  https://www.comptia.org/en-us/certifications/security/#objectives