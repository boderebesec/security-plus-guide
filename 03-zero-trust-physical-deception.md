# Zero Trust, Physical Security, Deception Technologies

**Domain:** 1.0 General Security Concepts

---

## Zero Trust Architecture (ZTA)

Zero Trust is a security model based on the principle “Never trust, always verify.”

### Key Tenets

- Continuous verification: authenticate and authorize every session  
- Least privilege access: grant only what’s absolutely needed  
- Microsegmentation: divide networks into isolated zones  
- Assume breach: design as if compromise is inevitable  

### Core Components

- Identity verification (MFA, IAM)  
- Network segmentation (VLANs, firewalls)  
- Endpoint monitoring (EDR)  
- Policy enforcement (ABAC, RBAC)  

---

## Physical Security

Controls to protect personnel, hardware, and facilities:

| Layer                  | Description               | Examples                        |
| ---------------------- | ------------------------- | ------------------------------- |
| Perimeter              | Outside boundary          | Fences, lighting, gates         |
| Exterior               | Entry points to buildings | Doors, locks, badge readers     |
| Internal               | Inner rooms/zones         | Secure server rooms, mantraps   |
| Personnel Security     | Human-centered policies   | ID badges, guards, visitor logs |

**Control Types**

- Deterrent: warning signs, cameras  
- Preventive: locks, mantraps  
- Detective: CCTV, alarms  
- Compensating: extra guards  

---

## Deception and Disruption Technologies

Creates traps or fake environments to detect attackers.

| Tool                 | Purpose                                       |
| -------------------- | --------------------------------------------- |
| Honeypots            | Simulated vulnerable system to lure attackers |
| Honeynets            | Networks of honeypots                         |
| Tarpits              | Slow attackers by responding very slowly      |
| Fake credentials     | Detect exfiltration or access misuse          |

**Benefits**

- Early attack detection  
- Attacker telemetry  
- Isolation from production  

---

## References

- NIST SP 800-207 – Zero Trust Architecture: https://doi.org/10.6028/NIST.SP.800-207  
- CISA Zero Trust Maturity Model: https://www.cisa.gov/zero-trust-maturity-model  
- NIST SP 800-53 Rev. 5 – PE & SI Controls: https://doi.org/10.6028/NIST.SP.800-53r5  
- CompTIA SY0-701 Exam Objectives: https://www.comptia.org/certifications/security  
