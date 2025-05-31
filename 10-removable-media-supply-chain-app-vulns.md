# Removable Media, Supply Chain Risks & Application Vulnerabilities — Domain 2: Threats, Vulnerabilities, and Mitigations

Focus: Understand how removable media, supply chain, and application weaknesses introduce risk
Purpose: Equip learners to identify and mitigate common physical-, vendor-, and software-based threats

---

## Removable Media Threats

Removable media (USB drives, SD cards, external HDDs) are major vectors because they bypass network controls and exploit user trust.

**Key Threats:**

* **Malware Injection**
  Auto-run executables or pre-planted malware on a device can infect hosts as soon as the media is attached.
* **Data Exfiltration**
  Sensitive files can be copied to an unauthorized device and physically carried offsite.
* **Device Misplacement**
  Lost or stolen drives often contain unencrypted data that can be recovered by an adversary.
* **Trust Exploitation**
  Social engineering (“found USB drive at reception”) tempts users to plug in unverified media.

**Best Practices:**

* Disable auto-run or auto-play features at the OS level.
* Enforce Data Loss Prevention (DLP) policies to detect or block unauthorized file transfers.
* Require full-disk encryption on approved removable devices (e.g., BitLocker To Go, VeraCrypt).
* Implement endpoint controls (e.g., USB port blockers, whitelist specific device IDs).

---

## Supply Chain Threats

Supply chain attacks compromise hardware, software, or services before they reach the enterprise.

**Common Scenarios:**

* **Hardware Tampering**
  Attackers modify firmware or embed malicious chips during manufacturing.
* **Compromised Updates**
  Signed patches or installers are altered to include backdoors before distribution.
* **Vulnerable Third-Party Software**
  Incorporating open-source libraries or vendor applications that contain unpatched flaws.
* **Subcontractor Breaches**
  A smaller vendor’s compromised environment can be leveraged to access larger clients.

**Notable Examples:**

* SolarWinds Orion compromise (malicious code inserted into official updates)
* Firmware implants in critical networking devices or IoT sensors

**Mitigation Strategies:**

* Perform formal Supply Chain Risk Assessments and vendor due diligence.
* Require a Software Bill of Materials (SBOM) to identify all components and versions.
* Monitor for unusual outbound traffic or behavior from newly installed components.
* Mandate time-bound patching and transparency contracts to enforce rapid vulnerability remediation.

---

## Application Vulnerabilities

Applications are frontline targets because they interact directly with users and often expose complex logic.

**Common Weaknesses:**

* **Improper Input Handling**
  Failure to sanitize or validate user input leads to SQL injection, cross-site scripting (XSS), or command injection.
* **Outdated Dependencies**
  Relying on old or unsupported libraries/frameworks that contain known CVEs.
* **Improper Error Handling**
  Revealing verbose stack traces, debug logs, or system information to an attacker.
* **Broken Authentication/Authorization**
  Weak session handling, predictable tokens, or misconfigured role permissions that allow privilege escalation.
* **Insecure Defaults**
  Applications shipped with default credentials, open ports, or unnecessary debuggers enabled.

**Key Notes:**

* Vulnerabilities are cataloged via CVE IDs and scored by CVSS for severity.
* Automated vulnerability scanners (e.g., Nessus, OWASP ZAP) can discover many common flaws.
* Runtime Application Self-Protection (RASP) and Web Application Firewalls (WAFs) offer additional defense.

---

## Summary Takeaways

* **Removable Media** risks combine physical asset control with user behavior.
* **Supply Chain** threats exploit “trusted” paths—hardware/firms you rely on daily.
* **Application Vulnerabilities** often result from coding errors, outdated components, or insecure default configurations.
* A layered defense—policy enforcement, user training, endpoint controls, and vendor scrutiny—reduces exposure.

---

## References

* NIST SP 800-161 Rev. 1 – Supply Chain Risk Management: [https://doi.org/10.6028/NIST.SP.800-161r1](https://doi.org/10.6028/NIST.SP.800-161r1)
* NIST SP 800-171 – Protecting Controlled Unclassified Information: [https://doi.org/10.6028/NIST.SP.800-171](https://doi.org/10.6028/NIST.SP.800-171)
* OWASP Top Ten – Application Security Risks: [https://owasp.org/www-project-top-ten/](https://owasp.org/www-project-top-ten/)
* CompTIA SY0-701 Exam Objectives: [https://www.comptia.org/certifications/security](https://www.comptia.org/certifications/security)
