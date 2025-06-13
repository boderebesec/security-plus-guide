# Application Security, Asset Management & Vulnerability Scanning — Domain 4: Security Operations

Topic: Application Security, Asset Management, Vulnerability Scanning  
Domain: 4.0 Security Operations

---

## Purpose of Security Operations

Security operations principles and controls ensure applications are developed securely, organizational assets are tracked and managed, and vulnerabilities are identified and remediated to uphold integrity, availability, and confidentiality.

---

## 1. Application Security

Modern applications must be developed and deployed with integrated security controls to minimize exploitable vulnerabilities

**Key Principles**
- Secure SDLC: integrate security into requirements, design, development, testing, deployment, and maintenance  
- Input validation: sanitize and validate user inputs to mitigate injection flaws (e.g., SQLi, XSS)  
- Authentication & authorization: enforce MFA and implement role-based access control (RBAC)  
- Error handling: avoid verbose error messages that expose internal logic or stack traces  
- Code review & testing: perform static (SAST), dynamic (DAST), and interactive (IAST) analysis  
- Software composition analysis (SCA): identify vulnerabilities in third-party libraries  

### OWASP Top 10 Focus
- Broken access control  
- Cryptographic failures  
- Injection  
- Security misconfiguration  
- Insecure design  

---

## 2. Asset Management

Asset management ensures visibility and control over hardware, software, and data throughout the organization

**Types of Assets**
- Hardware: servers, routers, IoT devices, laptops  
- Software: applications, operating systems, firmware, SaaS subscriptions  
- Data: databases, logs, backups, customer records  

**Best Practices**
- Automated discovery: identify rogue devices and shadow IT  
- Inventory: maintain an up-to-date asset repository with ownership and criticality  
- Tagging and classification: organize assets by function, risk, and compliance requirements  
- Lifecycle management: track assets from onboarding to decommissioning  
- Integration: link asset inventory with CMDBs and SIEMs for centralized monitoring  

---

## 3. Vulnerability Scanning

Proactive vulnerability management reduces the attack surface and validates patching effectiveness

**Scanning Techniques**
- Authenticated vs unauthenticated: logged-in scans yield more accurate results  
- Internal vs external: assess exposure from within and outside network boundaries  
- Agent-based vs agentless: choose based on asset accessibility and operational constraints  

**Key Concepts**
- False positives/negatives: validate findings through manual triage or correlation  
- Scan frequency: schedule regular scans and after major changes or incidents  
- Remediation prioritization: use CVSS scores, asset criticality, and exploit availability  
- Compliance reporting: demonstrate adherence to regulations (PCI DSS, HIPAA)  

**Common Tools**
- Nessus  
- OpenVAS  
- Qualys  
- Rapid7 InsightVM  
- Microsoft Defender for Endpoint  

---

## Summary Table

| Area                   | Focus                        | Tools/Practices                            |
| ---------------------- | ---------------------------- | -------------------------------------------|
| Application Security   | Secure design & development  | SDLC, OWASP Top 10, SAST/DAST/IAST, SCA    |
| Asset Management       | Visibility & classification  | Automated discovery, CMDB/SIEM integration |
| Vulnerability Scanning | Detect and manage weaknesses | Authenticated scans, CVSS prioritization   |

---

## References

- OWASP Top 10: https://owasp.org/www-project-top-ten/  
- NIST Cybersecurity Framework: https://www.nist.gov/cyberframework  
- MITRE CVE Database: https://cve.mitre.org/  
- NIST SP 800-40 Rev. 4 (Vulnerability Management): https://doi.org/10.6028/NIST.SP.800-40r4  
- CompTIA Security+ SY0-701 Exam Objectives: https://www.comptia.org/en-us/certifications/security/#objectives 