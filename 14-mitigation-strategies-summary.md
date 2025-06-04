# Mitigation Strategies & Summary Review — Domain 2: Threats, Vulnerabilities, and Mitigations

Topic: Mitigation Strategies & Summary Review  
Domain: 2.0 Threats, Vulnerabilities, and Mitigations

---

## Purpose of Mitigation

Mitigation strategies are implemented to reduce the attack surface, prevent exploitation of vulnerabilities, and lessen the impact of successful attacks. They apply before, during, and after incidents, and align with defense-in-depth principles.

---

## Access Control Threats

**Threat Types:**
- Unauthorized access  
- Credential theft  
- Session hijacking  

**Mitigations:**
- Multi-Factor Authentication (MFA): Combines factors (e.g., something you know + something you have)  
- Strong password policies: Enforce complexity, expiration, and reuse prevention  
- Least Privilege: Grant users only the access they absolutely need  
- Account Lockout Policies: Limit brute-force attempts  
- Session timeout & re-authentication: Prevent hijacking via idle sessions  

---

## Network-Based Threats

**Threat Types:**
- DDoS  
- Man-in-the-Middle (MitM)  
- Spoofing  
- Scanning  

**Mitigations:**
- Firewalls & ACLs: Define and enforce allowed traffic  
- Network segmentation & isolation: Protect critical systems by separating them  
- IDS/IPS: Detect and block malicious packets  
- DDoS protections: Implement rate-limiting, geo-blocking, or third-party mitigation services  
- VPNs & encryption: Secure remote communication channels  

---

## Email & Communication Threats

**Threat Types:**
- Phishing  
- Business Email Compromise (BEC)  
- Spoofing  

**Mitigations:**
- SPF, DKIM, DMARC: Authenticate senders and prevent spoofing  
- Secure email gateways: Scan attachments, links, and content  
- Phishing simulations and training: Increase employee awareness  
- Content Disarm & Reconstruction (CDR): Remove potential exploits from attachments  

---

## System-Based Threats

**Threat Types:**
- Exploitation of unpatched systems  
- Privilege escalation  

**Mitigations:**
- Patching & vulnerability management: Regular updates with proper tracking  
- Application whitelisting: Allow only approved applications to run  
- EDR solutions: Detect post-exploitation behavior  
- Hardened OS configurations: Disable unused ports and services  

---

## Application Vulnerabilities

**Threat Types:**
- Cross-Site Scripting (XSS)  
- SQL Injection (SQLi)  
- Logic flaws  
- Improper input handling  

**Mitigations:**
- Input validation and output encoding: Sanitize and neutralize user-supplied data  
- Secure coding practices: Follow OWASP Top Ten guidance  
- Web Application Firewall (WAF): Filter traffic for known application-layer attacks  
- SAST/DAST/IAST tools: Perform automated security testing during the SDLC  

---

## Removable Media Threats

**Threat Types:**
- Malware injection via USB devices  
- Data exfiltration via removable media  

**Mitigations:**
- Device control policies: Block unauthorized USB access  
- Data Loss Prevention (DLP) software: Detect and prevent sensitive file transfers  
- Disable autorun/autoplay for removable media  
- User training: Raise awareness of “baiting” attacks using malicious drives  

---

## Supply Chain Threats

**Threat Types:**
- Hardware implants  
- Compromised software updates  

**Mitigations:**
- Vendor vetting & Supply Chain Risk Management (SCRM)  
- Software Bill of Materials (SBOM): Track components and dependencies  
- Firmware integrity checks: Verify authenticity before installation  
- Signed updates: Ensure software comes from a trusted source  

---

## Cloud Threats

**Threat Types:**
- Misconfigurations  
- Exposed APIs  
- Excessive privileges  

**Mitigations:**
- Cloud Security Posture Management (CSPM): Detect insecure settings  
- IAM best practices: Enforce least privilege and role separation  
- Encryption at rest and in transit  
- Cloud logging: Enable audit trails (e.g., AWS CloudTrail, Azure Monitor)  

---

## Cryptographic Weaknesses

**Threat Types:**
- Use of outdated or broken algorithms  
- Poor key management  

**Mitigations:**
- Strong algorithms: AES-256, RSA-2048+, SHA-256  
- Key lifecycle controls: Secure generation, storage, and rotation  
- TLS 1.2/1.3: Enforce secure transport protocols  
- Certificate pinning & validation: Prevent MitM attacks in mobile and web applications  

---

## Zero-Day & Advanced Threats

**Mitigations:**
- Behavioral analytics (UEBA): Detect anomalous usage patterns  
- Threat intelligence feeds: Preemptively block known malicious indicators  
- EDR/XDR: Hunt threats beyond simple signatures  
- Incident response plans: Contain, eradicate, and recover quickly  

---

## Review Summary

- Match real-world threats with appropriate mitigations, not just theory  
- Understand how controls differ by environment (e.g., mobile vs. cloud)  
- Prepare for scenario-based questions that test prioritization and response selection  
- Tie mitigations to cyber kill-chain phases: Reconnaissance, Access, Action, Exfiltration  

---

## References

- NIST SP 800-53 Rev. 5 – Security and Privacy Controls: https://doi.org/10.6028/NIST.SP.800-53r5  
- OWASP Top Ten: https://owasp.org/www-project-top-ten/  
- CIS Controls v8: https://www.cisecurity.org/controls/cis-controls-list  
- CompTIA SY0-701 Official Objectives: https://www.comptia.org/certifications/security  