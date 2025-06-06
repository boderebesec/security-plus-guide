# Infrastructure Security, Ports & Firewalls, Secure Communications — Domain 3: Security Architecture

Topic: Infrastructure Security, Ports & Firewalls, Secure Communications  
Domain: 3.0 Security Architecture

---

## Purpose of Security Architecture

Security architecture principles and controls are designed to protect data and resources across different environments—Cloud, Network, Virtualization, IoT, and SCADA—by reducing risk, enforcing segregation, and enabling continuous monitoring.

---

## 1. Infrastructure Security

Infrastructure security includes the physical and logical defenses used to protect hardware, networks, and data systems. It spans on-premises, hybrid, and cloud environments.

**Key Concepts:**
- **Layered Defense (Defense in Depth):** Combines physical, technical, and administrative controls.  
- **Network Segmentation:** Dividing critical assets across zones (DMZ, internal, secure) to reduce lateral movement.  
- **Asset Visibility:** Using asset inventory, logging, and monitoring for full situational awareness.  

**Controls:**
- **Physical:** Locks, cameras, access logs  
- **Technical:** Network Access Control (NAC), VLANs, host firewalls  
- **Administrative:** Access policies, training, incident response plans  

---

## 2. Port Security & Firewalls

### Common Ports & Services

| Port | Protocol | Description             |
| ---- | -------- | ----------------------- |
| 22   | SSH      | Secure remote access    |
| 23   | Telnet   | Insecure shell          |
| 80   | HTTP     | Unencrypted web traffic |
| 443  | HTTPS    | Secure web traffic      |
| 53   | DNS      | Domain resolution       |
| 25   | SMTP     | Email transmission      |
| 110  | POP3     | Email retrieval         |
| 3389 | RDP      | Remote desktop          |

### Firewall Types

- **Packet-Filtering Firewalls:** Basic allow/deny rules based on IP and port.  
- **Stateful Firewalls:** Track connection state and allow return traffic.  
- **Proxy Firewalls:** Perform deep inspection at the application layer.  
- **Next-Gen Firewalls (NGFW):** Combine content inspection, threat detection, and application awareness.  

### Best Practices

- **Implicit Deny:** All traffic is blocked unless explicitly allowed.  
- **Least Privilege:** Only open required ports and protocols.  
- **Zone-Based Policies:** Use DMZs and access control rules to isolate networks.  

---

## 3. Secure Communications

### Secure Protocols

- **HTTPS (TLS 1.2/1.3):** Encrypts web traffic end-to-end.  
- **IPSec:** Provides VPN tunneling for site-to-site and remote access.  
- **SFTP / SCP:** Secure file transfers over SSH.  
- **STARTTLS / SMTPS:** Encrypts email in transit.  
- **RDP with Network Level Authentication (NLA):** Authenticates users before session initiation.  

### Email Security

- **S/MIME:** Uses certificate-based digital signing and encryption (relies on PKI).  
- **PGP:** User-managed email encryption with a web-of-trust model.  
- **SPF / DKIM / DMARC:** Prevent spoofing and enforce email authenticity.  

### Certificate Best Practices

- Use certificates issued by trusted Certificate Authorities (CAs).  
- Select strong key sizes (e.g., RSA 2048+, ECC when appropriate).  
- Monitor certificate expiration and timely revocation.  

---

## Summary Table

| Area                  | Key Focus                   | Implementation Tools                          |
| --------------------- | --------------------------- | ----------------------------------------------|
| Infrastructure        | Defense in Depth            | NAC, network segmentation, policy enforcement |
| Ports & Firewalls     | Network traffic control     | Stateful firewalls, ACLs, zone isolation      |
| Secure Communications | Confidentiality & integrity | TLS, IPSec, PKI, email signing                |

---

## References

* CompTIA Security+ SY0-701 Exam Objectives: https://www.comptia.org/en-us/certifications/security/#objectives  
* Mozilla TLS Security Guidelines: https://wiki.mozilla.org/Security/Server_Side_TLS  
* NIST SP 800-41 Revision 1 (Guidelines on Firewalls and Firewall Policy): https://csrc.nist.gov/publications/detail/sp/800-41/rev-1/final  
* CIS Controls v8: https://www.cisecurity.org/controls 