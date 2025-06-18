# Digital Forensics & Log Sources — Domain 4: Security Operations

Topic: Forensic Analysis & Logging  
Domain: 4.0 Security Operations

---

## Purpose of Security Operations

Security operations use digital forensics and comprehensive logging to detect, investigate, and respond to security incidents, ensuring accountability and compliance.

---

## 1. Digital Forensics

Digital forensics involves collecting, preserving, analyzing, and reporting digital evidence from systems affected by security incidents.

### Key Objectives
- Preserve evidence integrity for legal or internal investigations  
- Determine the scope and impact of security incidents  
- Reconstruct attacker behavior and timelines  

### Forensics Phases
1. **Identification**  
   - Determine evidence sources: endpoints, cloud, memory  
2. **Preservation**  
   - Use write blockers; verify hashes (MD5, SHA-256); document chain of custody  
   - Capture disk images, memory dumps, network traffic (PCAPs)  
3. **Analysis**  
   - Examine file timestamps, log entries, and user activity  
   - Identify persistence mechanisms, malware artifacts, and lateral movement  
4. **Reporting**  
   - Document methodology, tools used, timelines, and conclusions  

Common tools: FTK, EnCase, Autopsy, Volatility, Wireshark

---

## 2. Log Sources & Management

Logs provide critical context for threat detection, investigation, and compliance.

### Important Log Types

| Log Type            | Description                                |
| ------------------- | -------------------------------------------|
| System logs         | OS events such as login attempts, shutdown |
| Application logs    | App-specific events (e.g., web server logs)|
| Security logs       | Alerts from EDR, antivirus, IDS/IPS        |
| Network logs        | Traffic patterns, firewall and DNS logs    |
| Authentication logs | Successful and failed login attempts       |
| Audit logs          | Configuration and permission changes       |

### Key Log Sources
- Endpoints: user and kernel events  
- Servers: application, system, and patch logs  
- Network devices: firewall, router, and switch logs  
- Cloud platforms: access logs, API usage, audit trails  
- SIEM platforms: aggregated logs, correlated events, alerts  

### Best Practices
- Use NTP for time synchronization and log normalization  
- Forward logs to a centralized SIEM or syslog server  
- Define and enforce retention policies (e.g., PCI DSS: one-year retention)  
- Secure log storage: encrypt archives and control access  

---

## Summary Table

| Area           | Key Focus                       | Tools & Practices                               |
| -------------- | --------------------------------| ------------------------------------------------|
| Forensics      | Evidence acquisition & analysis | Disk imaging, memory dumps, hash verification |
| Log Management | Threat detection & compliance   | SIEM, syslog, NTP, secure retention policies    |

---

## References

- NIST SP 800-86: Guide to Integrating Forensic Techniques — https://doi.org/10.6028/NIST.SP.800-86  
- NIST SP 800-92: Guide to Computer Security Log Management — https://csrc.nist.gov/publications/detail/sp/800-92/final  
- MITRE ATT&CK Framework — https://attack.mitre.org/  
- CompTIA Security+ SY0-701 Exam Objectives — https://www.comptia.org/en-us/certifications/security/#objectives  
