# Encryption Overview

**Domain:** 1.0 General Security Concepts

---

## What Is Encryption?

Encryption is the process of transforming plaintext into ciphertext using algorithms and keys to protect data confidentiality.

### Core Encryption Elements

- **Plaintext**: original, readable data  
- **Ciphertext**: encrypted, unreadable output  
- **Algorithm**: mathematical formula used (for example, AES or RSA)  
- **Key**: secret used to perform encryption and decryption  

---

## Symmetric Encryption

Uses a single key for both encryption and decryption.

| Feature        | Description                     |
| -------------- | ------------------------------- |
| **Key use**    | same key used on both ends      |
| **Speed**      | fast, efficient                 |
| **Drawback**   | key distribution is a challenge |

### Common Algorithms

- AES (Advanced Encryption Standard)  
- DES and 3DES (deprecated)  
- Blowfish and Twofish  

---

## Asymmetric Encryption

Uses a key pair: public key for encryption and private key for decryption.

| Feature           | Description                              |
| ----------------- | ---------------------------------------- |
| **Public key**    | used to encrypt                          |
| **Private key**   | used to decrypt                          |
| **Reversible use**| also supports digital signatures         |

### Use Cases

- secure email (PGP)  
- SSL/TLS (HTTPS)  
- digital signatures  

---

## Public Key Infrastructure (PKI)

Supports secure key exchange, certificate management, and trust.

### Key Components

- **CA (Certificate Authority)** – issues certificates  
- **RA (Registration Authority)** – verifies identities  
- **CSR (Certificate Signing Request)** – initiates a certificate request  
- **CRL/OCSP** – certificate revocation checking  
- **Digital certificate** – binds identity to a public key  

---

## Encryption Concepts in Action

| Scenario                           | Method Used                   |
|------------------------------------|-------------------------------|
| Encrypting a file for storage      | Symmetric (AES)               |
| Sending secure email               | Asymmetric (RSA + PGP)        |
| Authenticating a server over HTTPS | PKI and digital certificate   |

---

## References

- NIST SP 800-175B Rev. 1 – Cryptographic Standards: https://doi.org/10.6028/NIST.SP.800-175Br1  
- NIST SP 800-57 Pt. 1 Rev. 5 – Key Management: https://doi.org/10.6028/NIST.SP.800-57pt1r5  
- ISO/IEC 27001:2022 – Cryptographic Controls: https://www.iso.org/isoiec-27001-information-security.html  
- CompTIA SY0-701 Exam Objectives: https://www.comptia.org/certifications/security  
