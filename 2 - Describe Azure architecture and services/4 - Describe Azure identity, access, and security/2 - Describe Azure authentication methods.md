## Azure Authentication Methods
---

### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**

- **Authentication does NOT confirm access permissions**, only identity verification.
- **Single Sign-On (SSO) is only as secure as the initial authenticator**—if compromised, all connected services are at risk.
- **MFA significantly increases security by requiring multiple authentication factors**.
- **Passwordless authentication enhances security and convenience**, reducing password-related risks.

---

### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**

- **Authentication**: The process of establishing the identity of a person, service, or device by providing credentials.
- **Single Sign-On (SSO)**: A method that allows a user to sign in once and access multiple applications without re-entering credentials.
- **Multifactor Authentication (MFA)**: A security feature requiring multiple forms of authentication for access.
- **Passwordless Authentication**: A method where users authenticate using factors other than passwords, such as biometrics or security keys.

---

### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**

- Security and convenience used to be at odds, but modern authentication solutions offer both.
- **Password security levels vary**:
  - Passwords alone: **Low security, high convenience**.
  - Password + 2FA: **High security, low convenience**.
  - Passwordless: **High security, high convenience**.
 
![AuthMethods](https://learn.microsoft.com/en-us/training/wwl-azure/describe-azure-identity-access-security/media/passwordless-convenience-security-30321b4d-18aa7d73.png)

---

## Single Sign-On (SSO)

### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**

- Without SSO:
  - Users need **multiple passwords**.
  - Increased **help desk workload** (account lockouts, password resets).
  - Risk of **orphaned accounts** if a user leaves the organization.

- With SSO:
  - Users remember **only one password**.
  - **Access is linked to a single identity**, making security management easier.
  - **Reduces security risks and administrative effort**.

---

## Multifactor Authentication (MFA)

### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**

- **MFA requires at least two authentication factors**:
  - **Something you know** (password, security question).
  - **Something you have** (phone, security key, smart card).
  - **Something you are** (fingerprint, facial recognition).

- **Why MFA is crucial**:
  - **If a password is stolen, MFA prevents unauthorized access**.
  - **MFA should be enabled wherever possible for security benefits**.

---

## Microsoft Entra Multifactor Authentication

- Microsoft service that enables **MFA options like phone calls and app notifications**.
- **Enhances security by adding extra authentication steps** beyond passwords.

---

## Passwordless Authentication

### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- **Passwordless authentication requires prior setup on a trusted device**.
- **FIDO2 security keys offer the strongest passwordless authentication** with hardware-based security.
  
### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**

- Eliminates passwords, replacing them with **more secure and convenient methods**.
- Requires setup on a trusted device **before use**.
- Uses **a combination of device ownership (something you have) and a PIN or biometrics (something you are/know)**.

### **Passwordless Authentication Methods**

#### Windows Hello for Business
- **Best for information workers with a dedicated Windows PC**.
- Uses **biometric and PIN credentials tied to the user's PC**.
- **Integrated with public key infrastructure (PKI) and SSO**.

#### Microsoft Authenticator App
- **Turns iOS/Android phones into passwordless authentication tools**.
- Users confirm identity via **notifications, number matching, biometrics, or PIN**.

#### FIDO2 Security Keys
- **Unphishable, standards-based passwordless authentication**.
- Uses **external security keys (USB, Bluetooth, NFC)**.
- **No username/password needed once set up**.

---
