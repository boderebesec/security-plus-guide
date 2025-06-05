# Cloud, Network, Virtualization, and IoT/SCADA — Domain 3: Security Architecture

Topic: Cloud, Network, Virtualization, and IoT/SCADA  
Domain: 3.0 Security Architecture

---

## Purpose of Security Architecture

Security architecture principles and controls are designed to protect data and resources across different environments—Cloud, Network, Virtualization, IoT, and SCADA—by reducing risk, enforcing segregation, and enabling continuous monitoring.

---

## Cloud Threats

**Threat Types:**
- Misconfigured storage (e.g., open S3 buckets)  
- Insecure APIs  
- Overprivileged service accounts  
- Lack of network segmentation  

**Mitigations:**
- Cloud Security Posture Management (CSPM): Continuously scan for misconfigurations  
- IAM hardening: Enforce least privilege and role-based access controls  
- Encryption at rest and in transit: Secure data stored and moving across networks  
- Logging and monitoring: Utilize AWS CloudTrail, Azure Monitor, or equivalent for auditing  
- Container scanning & image signing: Verify container images before deployment  

---

## Network-Based Threats

**Threat Types:**
- Flat networks (no segmentation)  
- Outdated protocols (e.g., Telnet, SMBv1)  
- Rogue devices or unmonitored ports  

**Mitigations:**
- Firewalls & ACLs: Define and enforce allowed traffic flows  
- Network segmentation & microsegmentation: Restrict lateral movement between zones  
- IDS/IPS: Detect and block anomalous or malicious packets  
- Zero Trust Network Architecture (ZTNA): Verify every connection, assume no implicit trust  
- Network Access Control (NAC): Enforce endpoint compliance before granting access  

---

## Virtualization Threats

**Threat Types:**
- Hypervisor escape (attacker moves from a VM to the host)  
- VM sprawl and outdated templates (unpatched or orphaned VMs)  
- Snapshot and image tampering (malicious modifications before deployment)  

**Mitigations:**
- Role separation: Distinguish VM administrator and hypervisor administrator privileges  
- Secure hypervisor configuration: Disable unused services, enforce strong authentication, patch host OS  
- Management network isolation: Use a separate interface for hypervisor management traffic with ACLs and MFA  
- Inter-VM traffic monitoring: Deploy virtual firewalls or host-based tools to inspect VM-to-VM communications  

---

## IoT/Embedded Device Threats

**Threat Types:**
- Default or hardcoded credentials  
- Lack of regular patching (firmware and OS)  
- Weak physical security (devices easily accessible)  
- Insecure communication protocols (unencrypted or unsigned messages)  

**Mitigations:**
- Network isolation: Place IoT/OT devices on separate VLANs or air-gapped segments  
- Secure gateways & firewalls: Route IoT traffic through gateways that enforce protocol validation  
- Asset discovery & inventory: Maintain up-to-date records of every device, firmware version, and patch status  
- Specialized IDS for ICS/IoT: Deploy tools (e.g., Nozomi, Claroty) that understand ICS protocols and detect anomalies  

---

## SCADA/ICS Threats

**Threat Types:**
- Insider sabotage or unauthorized configuration changes  
- Unpatched PLCs/RTUs (programmable logic controllers/remote terminal units)  
- Physical intrusion or sensor spoofing (false measurements fed to controllers)  

**Mitigations:**
- Follow IEC 62443 & NIST SP 800-82 guidance: Implement industry-standard ICS controls  
- Secure remote access: Enforce VPN with MFA, limit access windows, and monitor sessions  
- Change management for legacy systems: Document every modification, test in isolated environments before production  
- Availability-oriented defenses: Prioritize uptime (e.g., fault-tolerant designs, redundant controllers)  

---

## Review Summary

- Understand how shared responsibility shifts across SaaS, PaaS, and IaaS for Cloud security.  
- Enforce segmentation and least-privilege routing to mitigate network-based threats.  
- Secure hypervisor and management interfaces to prevent virtualization attacks.  
- Isolate IoT/SCADA devices, maintain asset inventories, and deploy specialized IDS to detect anomalies.  
- In ICS environments, availability often takes precedence—design controls that preserve uptime without sacrificing integrity.

---

## References

- NIST SP 800-82 Revision 2 – Industrial Control Systems Security Guide: https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-82r2.pdf  
- CIS Benchmarks – Center for Internet Security configuration baselines: https://www.cisecurity.org/cis-benchmarks  
- AWS Well-Architected Framework – AWS best practices for secure architectures: https://docs.aws.amazon.com/wellarchitected  
- OWASP IoT Top 10 – Common IoT/embedded device risks and mitigations: https://owasp.org/www-project-internet-of-things/  