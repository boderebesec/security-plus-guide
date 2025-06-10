# Data Security Foundations — Domain 3: Security Architecture (Catch-up & Review)

Topic: Data Types, Classification, Security Models & Protection Methods  
Domain: 3.0 Security Architecture

---

## Purpose of Security Architecture

Security architecture principles and controls are designed to protect data and resources across different environments—Cloud, Network, Virtualization, IoT, and SCADA—by reducing risk, enforcing segregation, and enabling continuous monitoring.

---

## 1. Data Types

Understanding data types is essential for applying the right security measures.

**Types of Data:**
- Structured Data: Organized into rows/columns (e.g., SQL databases)  
- Unstructured Data: Media files, documents, logs (e.g., PDFs, videos)  
- Semi-structured Data: JSON, XML—does not follow strict schema  
- Metadata: Describes other data (e.g., file size, creation date)  

**Data States:**
- Data at Rest: Stored on physical/digital media (HDD, SSD, cloud)  
- Data in Transit: Moving across networks (VPN, TLS)  
- Data in Use: Actively processed by an application or system  

---

## 2. Data Classification

Classification determines handling requirements and access controls.

**Classification Levels:**
- Public: No harm if disclosed (e.g., press releases)  
- Internal/Private: Limited access (e.g., internal emails)  
- Confidential: May impact organization if leaked (e.g., financials)  
- Restricted/Highly Confidential: Highest impact if compromised (e.g., PII, trade secrets)  

**Government Classifications (U.S. Example):**
- Unclassified, Confidential, Secret, Top Secret  

**Labeling Considerations:**
- Who labels data  
- How labeling is applied (manual vs automated)  
- When relabeling is required  

---

## 3. Data Considerations

Security depends not just on classification, but on operational policies and compliance.

**Key Considerations:**
- Data Ownership: Defined responsibilities for protection  
- Retention & Archiving: Align timelines with legal/business requirements  
- Data Sovereignty: Jurisdictional controls based on storage location  
- Regulations: GDPR, HIPAA, PCI DSS, etc.  
- Disposition: Secure deletion, wiping, or destruction methods (NIST SP 800-88)  

**Data Lifecycle:**
1. Creation  
2. Storage  
3. Use  
4. Sharing  
5. Archival  
6. Disposal  

---

## 4. Methods to Secure Data

Controls must be selected based on data type, classification, and environment.

**Technical Controls:**
- Encryption: For data at rest, in transit, and in use  
- Masking & Tokenization: Obscure sensitive elements (e.g., credit cards)  
- Hashing: Integrity verification  
- Access Controls: RBAC, ABAC, or DAC models  

**Administrative Controls:**
- Policies: Classification, retention, access, usage  
- Awareness Training: Reduces human error and insider threats  

**Physical Controls:**
- Media Handling: Locked storage, badge access  
- Secure Disposal: Shredding, degaussing, destruction  

---

## Summary Diagram

| Stage     | Mechanism       |
| --------- | --------------- |
| Create    | Classification  |
| Use/Store | Controls        |
| Share     | Retention       |
| Dispose   | Sanitization    |

---

## Flashcards (Key Concepts)

**Q:** What are the three states of data?  
A: At rest, in transit, in use  

**Q:** Which method ensures confidentiality during transmission?  
A: TLS (Transport Layer Security)  

**Q:** What is data sovereignty?  
A: Laws applied to data based on its physical location  

**Q:** What is the purpose of data classification?  
A: To define access control and protection requirements  

**Q:** What method ensures permanent removal of sensitive data from storage?  
A: Sanitization (e.g., wiping, degaussing, destruction)  

---

## References

- NIST SP 800-88r1: Guidelines for Media Sanitization  
  https://csrc.nist.gov/publications/detail/sp/800-88/rev-1/final

- CompTIA Security+ SY0-701 Objectives  
  https://www.comptia.org/certifications/security

- ISO/IEC 27001: Information Security Management  
  https://www.iso.org/isoiec-27001-information-security.html

- CIS Controls v8 – Data Protection  
  https://www.cisecurity.org/controls/data-protection  
