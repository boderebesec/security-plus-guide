# System Hardening, Mobile & Wireless Security — Domain 4: Security Operations

Topic: System Hardening, Mobile Security, and Wireless Security  
Domain: 4.0 Security Operations

---

## Purpose of Security Operations

Security operations principles and controls are designed to maintain and enhance the integrity, availability, and confidentiality of systems—through hardened configurations, device management, and secure network practices.

---

## 1. System Hardening

System hardening reduces vulnerabilities by limiting attack surfaces and enforcing secure configurations.

### Core Practices
- **Remove unnecessary services:** Disable unused ports and services to minimize exposure  
- **Secure configurations:** Apply vendor baselines, NIST hardening guides, and CIS Benchmarks  
- **Patch management:** Regular OS and application updates; automate where possible  
- **Account management:** Enforce least privilege, lock unused accounts, disable guest access  
- **Logging & monitoring:** Enable system auditing, alerting, and log retention  

### Common Hardening Targets
- Operating systems (Windows, Linux, macOS)  
- Hypervisors and virtual machines  
- Databases and application servers  
- IoT and embedded devices  

---

## 2. Mobile Security

Mobile platforms introduce unique risks due to app ecosystems, portability, and user behavior.

### Threats
- Jailbreaking/rooting  
- Malicious apps, spyware, and stalkerware  
- Insecure APIs and data leakage  
- OS fragmentation and delayed updates  

### Protections
- **Mobile Device Management (MDM):** Enforce security policies, restrict app installs, enable remote wipe  
- **Containerization:** Isolate business data from personal environments  
- **App vetting:** Allow only signed and reviewed applications  
- **Biometrics & MFA:** Strengthen device access controls  
- **Full-disk encryption & VPNs:** Secure communications  

---

## 3. Wireless Security

Wireless networks are inherently open to proximity-based threats.

### Risks
- Rogue access points  
- Evil twin attacks  
- Interference and jamming  
- Weak encryption protocols  

### Best Practices
- Use **WPA3** or **WPA2-AES**; never use WEP  
- Disable **WPS** to prevent brute-force attacks  
- Configure SSIDs carefully: avoid defaults, consider hiding or obscuring names  
- Implement **MAC filtering** to restrict device access  
- Deploy **captive portals** for guest networks  
- Use **802.1X authentication** with RADIUS/LDAP integration  

---

## Summary Table

| Area               | Key Focus                    | Controls/Tools                         |
| ------------------ | ---------------------------- | -------------------------------------- |
| System Hardening   | Reduce attack surface        | CIS Benchmarks, patch management       |
| Mobile Security    | Device & app protection      | MDM, encryption, VPN, containerization |
| Wireless Security  | Secure transmission & access | WPA3, MAC filtering, 802.1X            |

---

## References

- NIST SP 800-70 Rev. 4 — Security Configuration Checklists  
  https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-70r4.pdf  
- CIS Benchmarks  
  https://www.cisecurity.org/cis-benchmarks/  
- CompTIA SY0-701 Exam Objectives  
  https://www.comptia.org/certifications/security#examdetails  
- OWASP Mobile Security Testing Guide (MSTG)  
  https://owasp.org/www-project-mobile-security-testing-guide/  
- NIST SP 800-153 Rev. 1 — Guidelines for Securing Wireless LANs  
  https://csrc.nist.gov/publications/detail/sp/800-153/rev-1/final 