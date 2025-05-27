# Hashing, Obfuscation, Review

**Domain:** 1.0 General Security Concepts

---

## Hashing

Hashing is a one-way function that transforms data into a fixed-length value (“hash”) to ensure data integrity.

### Key Characteristics

- **Deterministic**: same input → same output  
- **One-way**: cannot reverse back to original data  
- **Fixed size**: output length is constant  
- **Collision-resistant**: hard to find two inputs with the same hash  

### Common Hash Algorithms

| Algorithm | Output Size | Notes                                |
| --------- | ----------- | -------------------------------------|
| MD5       | 128-bit     | deprecated, collision-prone          |
| SHA-1     | 160-bit     | deprecated                           |
| SHA-2     | 256-bit+    | industry standard (SHA-256, SHA-512) |
| SHA-3     | 256-bit+    | newer, NIST-approved                 |

Used for file integrity checks, password storage (with salts), and digital signatures.

---

## Obfuscation

Obfuscation makes code, data, or processes difficult to understand, delaying or deterring analysis.

### Common Techniques

- Code obfuscators  
- Variable/function renaming  
- Packing or encoding binaries  
- Stripping symbols  

Obfuscation is not a substitute for encryption—it’s a defense-in-depth measure.

---

## Hashing vs Encryption vs Obfuscation

| Feature     | Hashing                 | Encryption                | Obfuscation             |
| ----------- | ----------------------- | --------------------------| ------------------------|
| Purpose     | Verify integrity        | Ensure confidentiality    | Delay or deter analysis |
| Reversible? | No                      | Yes (with key)            | Yes (with effort)       |
| Use Cases   | Passwords, file checks  | Data transmission/storage | Protect source/binaries |

---

## Summary Notes

- Hashing is integrity-focused; always salt passwords.  
- Use SHA-256 or stronger in new systems.  
- Pair obfuscation with encryption for robust protection.

---

## References

- NIST SP 800-107 Rev. 1 – Hashing Usage: https://doi.org/10.6028/NIST.SP.800-107r1  
- NIST SP 800-57 Part 1 Rev. 5 – Key Management: https://doi.org/10.6028/NIST.SP.800-57pt1r5  
- CIS Controls v8 – Secure Configuration: https://www.cisecurity.org/controls/cis-controls-list  
- CompTIA SY0-701 Exam Objectives: https://www.comptia.org/certifications/security  