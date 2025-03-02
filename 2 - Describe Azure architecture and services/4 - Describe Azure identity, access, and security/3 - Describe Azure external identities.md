# **Azure External Identities**  

Azure **External Identities** allow organizations to securely interact with people **outside** their organization, such as **partners, suppliers, vendors, or customers**.

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
- External users **bring their own identities** (Google, Facebook, corporate, government-issued, etc.).  
- The **external identity provider** manages authentication.  
- Microsoft Entra ID or Azure AD B2C **controls access** to protect resources.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**  
- **External Identity** – A person, device, or service **outside** your organization.  
- **Microsoft Entra External ID** – A system for securely managing **external** users.  
- **B2B (Business-to-Business) Collaboration** – Allows external users to sign in with their **preferred identity**.  
- **B2B Direct Connect** – Establishes a **two-way** trust with another Microsoft Entra organization.  
- **B2C (Business-to-Customer)** – Manages external consumer identities for **custom or SaaS apps** using Azure AD B2C.  

---

## **How External Identities Work**  

External identities **allow users to sign in using their own credentials** from various identity providers.

![ExternalIdenties](https://learn.microsoft.com/en-us/training/wwl-azure/describe-azure-identity-access-security/media/azure-active-directory-external-identities-5a892021-ca79a69c.png)

---

## **Key Capabilities of External Identities**  

#### **1️⃣ B2B Collaboration**  
External users can **sign in** with their existing identity and access **Microsoft and enterprise apps**.  

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  
- Users appear in your **directory as guest users**.  
- Supports **SaaS apps and custom-developed apps**.  

#### **2️⃣ B2B Direct Connect**  
A **mutual** two-way trust between Microsoft Entra organizations for **seamless collaboration**.  

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  
- Currently **only supports** **Teams shared channels**.  
- External users **don’t appear** in your directory but can be **monitored in Teams Admin Center reports**.  

#### **3️⃣ B2C (Business-to-Customer)**  
Manages **customer identities** for **non-Microsoft apps** using **Azure AD B2C**.  

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  
- Used for **modern SaaS apps and custom applications**.  
- **Not** intended for Microsoft apps.  

---

## **Managing Guest Access in Microsoft Entra ID**  

With **Microsoft Entra B2B**, organizations can **invite and manage** guest users securely.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**  
- Guest users can be invited **by admins or other users**.  
- **Social identities** (e.g., Microsoft accounts) can also be used.  

---

## **Controlling Access for Guest Users**  

To **maintain security**, guest users should have **appropriate access levels**.

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
- **Access reviews** can be performed by a decision-maker or guest users.  
- Microsoft Entra ID provides **suggestions** for continued access.  
- **After a review, access can be removed** for guests who no longer need it.  
