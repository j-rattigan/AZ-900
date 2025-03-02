# Microsoft Entra ID and Directory Services

---

## ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- **Microsoft Entra ID** allows access to both Microsoft cloud applications and custom cloud applications.
- **Enhances security** by detecting suspicious sign-in attempts, such as logins from unknown locations or devices.
- **Microsoft Entra Connect** enables a seamless identity experience between cloud and on-premises environments
- **Microsoft Entra Domain** Services provides domain functionality without needing to manage domain controllers.

---

## ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**
- **Microsoft Entra ID**: A cloud-based identity and access management (IAM) service by Microsoft.
- **Active Directory (AD)**: An on-premises IAM service managed by an organization, running on Windows Server.
- **Microsoft Entra Connect**: A tool that syncs identities between on-premises Active Directory and Microsoft Entra ID.
- **Microsoft Entra Domain Services**: A managed service providing domain-related functions like LDAP, Kerberos, and NTLM authentication.

---

## ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- Microsoft Entra ID supports:
  - **Authentication** (MFA, self-service password reset, smart lockout, banned password lists).
  - **Single Sign-On (SSO)** (one username and password for multiple applications).
  - **Application Management** (integrating SaaS and on-premises applications).
  - **Device Management** (integrating with Intune for Conditional Access).

---

## ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Who uses Microsoft Entra ID?**
  - **IT Administrators**: Manage access to applications and resources.
  - **App Developers**: Add authentication features like SSO.
  - **Users**: Manage their own identity (password resets, etc.).
  - **Online Service Subscribers**: Already integrated with services like Microsoft 365, Azure, and Dynamics CRM.

- **How Microsoft Entra Domain Services Works**
  - Creates a **managed domain** with a **unique namespace** (domain name).
  - Deploys **two Windows Server domain controllers** in Azure.
  - Handles **backups and security** (Azure Disk Encryption).
  - Uses **one-way synchronization** from Microsoft Entra ID to Domain Services.

- **Example Benefits**
  - Allows **legacy applications** to run in the cloud without requiring modern authentication.
  - Enables **domain join, group policy, LDAP, and Kerberos/NTLM authentication** for cloud-based services.

---

## ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Key Takeaway**
Microsoft Entra ID is **the cloud equivalent of Active Directory**, enabling secure identity and access management. By integrating on-premises AD with Microsoft Entra ID, organizations can **create a seamless and secure hybrid identity solution**.

![InfoSync](https://learn.microsoft.com/en-us/training/wwl-azure/describe-azure-identity-access-security/media/azure-active-directory-sync-topology-7359f2b8-427db2d4.png)
