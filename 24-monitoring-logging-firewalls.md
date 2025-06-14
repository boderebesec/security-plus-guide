# Monitoring, Logging & Firewalls — Domain 4 & 5: Security Operations & Incident Response

Topic: Centralized Monitoring, Logging Practices, Firewall Implementation  
Domain: 4.0–5.0 Security Operations & Incident Response

---

## Purpose of Security Operations & Incident Response

Security operations ensure visibility into system activities, enforce network segmentation, and implement layered defenses that support threat detection, compliance, and response across environments.

---

## 1. Monitoring & Logging

Monitoring and logging provide situational awareness across IT assets, helping identify anomalies, breaches, and operational issues in real time.

**Key Principles**  
- Centralized logging: aggregate logs from multiple sources into a single platform (e.g., SIEM)  
- Log retention & integrity: define retention policies and ensure tamper-proofing with hashing or WORM storage  
- Timestamps & normalization: use NTP for time synchronization and consistent log formats for correlation  
- Event types: authentication logs, access control events, system errors, process starts/stops, privilege escalations  
- Alerting & correlation: define thresholds and leverage user/entity behavior analytics (UEBA)  

**Log Sources**  
- Firewalls, routers, IDS/IPS  
- Operating systems (Windows Event Logs, syslog)  
- Applications and authentication services  
- Cloud services (CloudTrail, Azure Monitor)  

**Monitoring Tools**  
- SIEM (Splunk, Elastic Stack, Microsoft Sentinel)  
- Endpoint Detection & Response (EDR)  
- NetFlow, SNMP, packet capture systems  

---

## 2. Firewall Technologies

Firewalls control ingress and egress traffic at network boundaries to prevent unauthorized access and support segmentation.

**Firewall Types**  
- Packet-filtering: rules based on IP, port, protocol  
- Stateful inspection: tracks active sessions and context  
- Application-level gateway (proxy): inspects application-layer payloads  
- Next-generation firewall (NGFW): integrates IDS/IPS, deep packet inspection, content filtering  

**Firewall Placement**  
- Perimeter: between internet and internal network  
- Internal segmentation: between user VLANs, server farms, R&D zones  
- Host-based: control traffic on individual systems  

**Best Practices**  
- Implicit deny: block all by default, allow explicitly  
- Use ACLs for segmentation and least privilege  
- Enable logging on firewall rules for visibility  
- Periodically review and validate rulesets  

---

## 3. Intrusion Detection & Prevention

IDS/IPS systems monitor network or host activity to identify and block malicious behavior.

**Types**  
- NIDS: network-wide visibility to detect scanning, sniffing, protocol anomalies  
- HIDS: host-based monitoring of file changes, registry access, process anomalies  
- Signature vs anomaly-based: known attack patterns vs behavioral deviations  

**Placement**  
- Inline (IPS) for active blocking  
- Tap/mirror port (IDS) for passive detection  

**Integration**  
- Feed alerts into SIEM for correlation  
- Trigger automated playbooks via SOAR  

---

## Summary Table

| Area                  | Key Focus                   | Tools/Practices                             |
| --------------------- | --------------------------- | ------------------------------------------- |
| Monitoring & Logging  | Visibility & detection      | SIEM, WEF/syslog, NTP, UEBA                 |
| Firewall Management   | Traffic filtering & control | NGFW, ACLs, zoning, rule auditing           |
| IDS/IPS               | Threat detection/prevention | NIDS, HIDS, signature/anomaly-based         |

---

## References

- NIST SP 800-92 (Log Management): https://doi.org/10.6028/NIST.SP.800-92  
- CIS Control 8: Audit Log Management: https://www.cisecurity.org/controls  
- MITRE ATT&CK Framework: https://attack.mitre.org/  
- NIST SP 800-41 Rev. 1 (Firewalls): https://csrc.nist.gov/publications/detail/sp/800-41/rev-1/final
- CompTIA Security+ SY0-701 Exam Objectives: https://www.comptia.org/en-us/certifications/security/#objectives
