# Data Types, Classifications & Security Models — Domain 3: Security Architecture

Topic: Data Types, Classifications, and Formal Security Models  
Domain: 3.0 Security Architecture

---

## Purpose of Security Architecture

Security architecture ensures the proper handling and protection of data throughout its lifecycle—at rest, in use, and in transit. Data must be accurately classified, assigned ownership, and protected according to its confidentiality, integrity, and availability (CIA) needs.

---

## 1. Data Types

Different data types require different protection mechanisms, especially when regulated or business-critical.

**Common Data Types:**
- **Regulated Data:** Includes health (PHI), financial (PCI), or personal (PII) data governed by laws or frameworks.  
- **Trade Secrets:** Confidential internal formulas, business logic, or plans.  
- **Intellectual Property (IP):** Patents, trademarks, copyrights, and creative works.  
- **Legal Data:** Contracts, litigation documents, regulatory disclosures.  
- **Financial Data:** Income statements, payroll, investments, and budgets.  
- **Human vs. Non-Human Readable:** Human-friendly formats (PDFs, emails) vs. machine code or scripts.

---

## 2. Data Classification

Data classification involves labeling information to reflect its sensitivity and determining how it should be stored, accessed, and protected.

### Common Levels:
- **Public:** Intended for open consumption (e.g., press releases).  
- **Internal:** For use within the organization only.  
- **Confidential:** Sensitive data that could pose risk if leaked.  
- **Restricted/Critical:** High-sensitivity data requiring strict controls.

### Government (U.S. Fed-level) Classification:
- **Confidential:** Lowest classification; unauthorized disclosure could cause damage.  
- **Secret:** Serious damage if disclosed.  
- **Top Secret:** Exceptionally grave damage if exposed.

---

## 3. Security Models

Formal models help enforce policies for how data is accessed and modified.

### Bell-LaPadula (BLP)
- **Focus:** Confidentiality  
- **Rule:** *No Read Up, No Write Down*  
- **Use Case:** Military/Government systems

### Biba
- **Focus:** Integrity  
- **Rule:** *No Write Up, No Read Down*  
- **Use Case:** Healthcare, financial records

### Clark-Wilson
- **Focus:** Data integrity via process enforcement  
- **Key Concepts:** Separation of duties, well-formed transactions  
- **Use Case:** Commercial applications and accounting systems

### Brewer-Nash (Cinderella Model)
- **Focus:** Dynamic confidentiality, conflict-of-interest prevention  
- **Rule:** Access changes based on the user's data interaction history  
- **Use Case:** Legal firms, consulting companies

---

## Summary Table

| Area           | Focus           | Examples/Controls                        |
|----------------|-----------------|------------------------------------------|
| Data Types     | What to protect | IP, PHI, PII, contracts, financials      |
| Classification | Sensitivity     | Public, Internal, Confidential, Critical |
| Models         | Access Rules    | Bell-LaPadula, Biba, Clark-Wilson        |

---

## References

* CompTIA Security+ SY0-701 Exam Objectives: https://www.comptia.org/certifications/security#objectives  
* Cornell Data Types Overview: https://it.cornell.edu/security-and-policy/data-types-high-risk-moderate-risk-low-risk  
* Digital Guardian on Classification: https://www.digitalguardian.com/blog/5-common-data-classification-types  
* TechTarget – Data States Explained: https://www.techtarget.com/searchdatamanagement/reference/states-of-digital-data 