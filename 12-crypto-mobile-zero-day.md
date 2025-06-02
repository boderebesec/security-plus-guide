# Cryptographic, Mobile, and Zero-Day Vulnerabilities — Domain 2: Threats, Vulnerabilities, and Mitigations

Focus: Identify and mitigate cryptographic weaknesses, mobile risks, and unknown zero-day threats  
Purpose: Strengthen understanding of exploitable flaws that stem from insecure defaults, user behavior, and delayed response

---

## Cryptographic Vulnerabilities

Cryptographic flaws often result from **poor implementation**, **weak key usage**, or **deprecated algorithms** — not the math itself.

**Common Crypto Issues**:

* Weak Algorithms: MD5, SHA-1 (vulnerable to collision attacks)
* Poor Key Management: Hardcoded, reused, or overly simple keys
* Improper Implementation: ECB mode, incorrect key lengths
* Expired or Self-Signed Certificates: Insecure trust model
* Lack of Encryption: Data sent or stored in plaintext (especially credentials)

**Mitigations**:

* Use strong, modern algorithms (AES, SHA-256 and higher)
* Rotate and securely store cryptographic keys
* Enforce PKI with trusted CAs and TLS 1.2+
* Follow NIST/FIPS standards (e.g., 140-3 validated modules)

---

## Mobile Device Vulnerabilities

Mobile devices introduce challenges due to user behavior, OS fragmentation, and constant connectivity.

**Key Risk Areas**:

* Unsecured Apps: Sideloaded APKs or shady third-party sources
* Outdated OS Versions: Missed patches, unsupported builds
* Jailbreaking/Rooting: Loss of sandbox protections
* Data Leakage: Through weak app permissions, clipboard access, cloud sync
* App Permissions Abuse: Overreach into contact lists, sensors, or files

**Mobile Security Controls**:

* Use Mobile Device Management (MDM) tools
* Require full-disk encryption, screen locks, and biometric/PIN auth
* Apply app whitelisting and containerization
* Restrict external connectivity (Bluetooth, NFC, USB, etc.)

---

## Zero-Day Vulnerabilities

Zero-days are flaws exploited **before vendors become aware or can issue a fix** — often seen in **targeted attacks**.

**Key Traits**:

* No public disclosure or patch at time of use
* May be weaponized by nation-states or advanced persistent threats (APTs)
* Often identified via incident forensics or intelligence feeds

**Detection & Mitigation**:

* Use behavior-based security (EDR, NGAV)
* Monitor for indicators of compromise (IOCs)
* Share and consume threat intel from ISACs and vendors
* Apply layered defense and limit exposure through segmentation

---

## Summary Takeaways

* Cryptographic mistakes often stem from **bad implementation**, not algorithm design
* Mobile platforms are **highly exploitable** without enterprise controls
* Zero-day threats demand **behavioral detection** and rapid response readiness

---

## References

* NIST SP 800-175B – Cryptographic Mechanisms: [https://doi.org/10.6028/NIST.SP.800-175Br1](https://doi.org/10.6028/NIST.SP.800-175Br1)
* OWASP Mobile Top 10: [https://owasp.org/www-project-mobile-top-ten/](https://owasp.org/www-project-mobile-top-ten/)
* CISA Known Exploited Vulnerabilities Catalog: [https://www.cisa.gov/known-exploited-vulnerabilities-catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog)
* CompTIA SY0-701 Exam Objectives: [https://www.comptia.org/certifications/security](https://www.comptia.org/certifications/security)