# Digital Certificates, Asymmetric vs Symmetric Encryption

**Domain:** 1.0 General Security Concepts

---

## Digital Certificates

A digital certificate binds an identity to a public key and proves ownership of that key.

### Certificate Elements

- **Subject**: owner identity  
- **Issuer**: Certificate Authority (CA)  
- **Public key**  
- **Serial number**  
- **Validity period**  
- **Digital signature**  

### Common Certificate Types

| Certificate Type        | Purpose                                  |
| ----------------------- | ---------------------------------------- |
| SSL/TLS                 | Secures HTTPS websites                   |
| Code Signing            | Verifies software integrity/authenticity |
| Email                   | Enables encrypted & signed email         |
| Client                  | Authenticates users to services          |
| Root / Intermediate     | PKI trust chain hierarchy                |

---

## Asymmetric Encryption (Recap)

- Uses **public** and **private** keys  
- Common algorithms: **RSA**, **ECC**  
- Enables confidentiality, authentication, and non-repudiation  

### Roles

- Encrypt with recipient’s **public key** → only the holder of the **private key** can decrypt  
- Sign with your **private key** → anyone can verify with your **public key**  

---

## Symmetric Encryption (Recap)

- Same key used for both encryption and decryption  
- Faster but less scalable in multi-user environments  
- Common algorithms: **AES**, **DES** (deprecated), **Blowfish**, **Twofish**  

---

## Comparing Symmetric vs Asymmetric

| Feature          | Symmetric                  | Asymmetric                       |
| ---------------- | ---------------------------| -------------------------------- |
| Key Use          | Same secret key            | Public/private key pair          |
| Speed            | Fast                        | Slower (more overhead)           |
| Use Case         | Data-at-rest                | Key exchange, digital signatures |
| Scalability      | Poor (key management)       | Good (PKI solves distribution)   |

---

## Key Terms

- **Key Pair**: the public and private keys in asymmetric encryption  
- **Digital Signature**: proves integrity and authenticity  
- **Certificate Authority (CA)**: trusted entity that issues and signs certificates  

---

## References

- NIST SP 800-57 Part 1 Rev. 5 – Key Management: https://doi.org/10.6028/NIST.SP.800-57pt1r5  
- NIST SP 800-175B Rev. 1 – Cryptographic Standards: https://doi.org/10.6028/NIST.SP.800-175Br1  
- ISO/IEC 27001:2022 – Cryptographic Controls: https://www.iso.org/isoiec-27001-information-security.html  
- CompTIA SY0-701 Exam Objectives: https://www.comptia.org/certifications/security 