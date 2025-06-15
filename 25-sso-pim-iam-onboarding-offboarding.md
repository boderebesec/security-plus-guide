# Single Sign-On, Privileged Access & Identity Lifecycle — Security+ SY0-701

Topic: Identity and Access Management  
Domain: 4.0 Security Operations

---

## Purpose of IAM

Identity and Access Management ensures only authorized users gain access to the right systems, at the right time, for the right reasons. A strong IAM strategy reduces risk, supports compliance, and improves operational efficiency

---

## 1. Single Sign-On (SSO)

Single Sign-On allows users to authenticate once and gain access to multiple systems without logging in again for each service

### Benefits
- User convenience: fewer logins reduce password fatigue  
- Centralized control: administrators manage access in one place  
- Reduced attack surface: fewer credentials mean fewer phishing targets  

### How it Works
- Federated identity: trust between systems using identity providers (SAML, OAuth, OpenID Connect)  
- Token-based authentication: a login session generates a token used across services  

### Risks
- Single point of failure: if SSO fails, access to all connected systems is blocked  
- Token hijacking: secure handling of tokens is critical  

---

## 2. Privileged Identity Management (PIM)

Privileged Identity Management manages elevated (admin/root) access across systems and applications

### Features
- Just-in-Time access: temporary privilege elevation when needed  
- Approval workflows: require sign-off before granting elevated roles  
- Session recording: monitor and log all privileged actions  

### Benefits
- Minimized attack window: reduces time users have dangerous permissions  
- Auditability: supports compliance and forensic investigations  
- Separation of duties: enforces role-based controls  

---

## 3. Identity Lifecycle: Onboarding & Offboarding

### Onboarding
- Identity proofing: verify user legitimacy  
- Automated provisioning: integrate HRIS (e.g., SCIM)  
- Role-based access control: assign permissions based on job function  
- MFA enforcement: require multi-factor authentication at first login  

### Offboarding
- Account disablement or deletion: remove access immediately  
- Revoke sessions and tokens: ensure active sessions are terminated  
- Device recovery or wipe: retrieve or wipe corporate devices  
- Access removal: revoke access to SaaS, VPN, and other services  
- Log archiving: retain logs for compliance and investigation  

---

## Summary Table

| Area                    | Key Focus                   | Tools & Concepts                                    |
| ----------------------- | --------------------------- | --------------------------------------------------- |
| Single Sign-On (SSO)    | Centralized authentication  | SAML, OAuth2, OpenID Connect, identity providers    |
| Privileged Access (PIM) | Managed elevated privileges | JIT access, approval workflows, session logging     |
| Identity Lifecycle      | Provisioning & deprovisioning | SCIM, RBAC, MFA, HRIS integration, token revocation |

---

## References

- NIST SP 800-53 Rev. 5 — AC Control Family  
  https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final  
- CompTIA Security+ SY0-701 Objectives  
  https://www.comptia.org/en-us/certifications/security/#objectives
- OWASP Authentication Cheat Sheet  
  https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html  
- Microsoft PIM Documentation  
  https://learn.microsoft.com/en-us/azure/active-directory/privileged-identity-management/ 