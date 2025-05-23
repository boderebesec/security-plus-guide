# CIA Triad, AAA, Authentication & Authorization Models

**Domain:** 1.0 General Security Concepts

---

## CIA Triad

The CIA Triad is the foundational model for cybersecurity. It defines three core goals of information security:

| Element             | Meaning                                            | Examples                               |
| ------------------- | -------------------------------------------------- | -------------------------------------- |
| Confidentiality     | Ensure data is accessible only to authorized users | Encryption, access controls            |
| Integrity           | Ensure data is accurate and untampered             | Hashing, checksums, digital signatures |
| Availability        | Ensure systems and data are accessible when needed | Redundancy, backups, fault tolerance   |

---

## AAA Framework

The AAA model defines how users are verified and held accountable within an environment:

| Component          | Function                                              | Examples                       |
| ------------------ | ----------------------------------------------------- | ------------------------------ |
| Authentication     | Verify identity                                       | Passwords, biometrics, MFA     |
| Authorization      | Determine what actions an authenticated user can take | RBAC, ACLs, group policies     |
| Accounting         | Track user actions and access                         | Logs, audits, session tracking |

---

## Authentication Factors

* Something you know – Password, PIN  
* Something you have – Token, smart card  
* Something you are – Biometrics (fingerprint, retina)  
* Somewhere you are – Location‐based (GPS, IP)  
* Something you do – Behavioral patterns (typing rhythm)  

---

## Authorization Models

| Model                                     | Description                                | Use Case Example                        |
| ----------------------------------------- | ------------------------------------------ | --------------------------------------- |
| DAC (Discretionary Access Control)        | Owner controls permissions                 | File/folder sharing on a local machine  |
| MAC (Mandatory Access Control)            | System‐enforced, based on classification   | Government/military data classification |
| RBAC (Role‐Based Access Control)          | Based on job roles                         | HR, Finance, IT departments in orgs     |
| ABAC (Attribute‐Based Access Control)     | Based on attributes (location, time, etc.) | Complex cloud or enterprise policies    |

---

## References

- [CompTIA SY0-701 Exam Objectives](https://www.comptia.org/certifications/security)  
- [NIST SP 800-53 Rev. 5 – Access Control](https://doi.org/10.6028/NIST.SP.800-53r5)  
- [ISO/IEC 27001:2022 – Access Control Standards](https://www.iso.org/isoiec-27001-information-security.html)  
