# **Azure Conditional Access**  

Conditional Access is a **security tool** in **Microsoft Entra ID** that grants or denies **access** to resources based on **identity signals**.

## **How Conditional Access Works**  

Conditional Access **collects signals, makes access decisions, and enforces security rules**.

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
- **Empowers users** to work from anywhere **securely**.  
- **Protects** the organization's assets from **unauthorized access**.  
- **Provides granular MFA control** based on **risk signals**.

- --

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**  
- **Conditional Access** – A security tool in Microsoft Entra ID that controls access based on **identity signals**.  
- **Identity Signals** – Factors like **who** the user is, **where** they are, and **what device** they're using.  
- **Multifactor Authentication (MFA)** – A security feature that requires **multiple forms of verification** before granting access.  
- **Enforcement** – The action taken based on access decisions (**allow, deny, or require MFA**).  

---

## **Conditional Access Process**  

1️⃣ **Collect Signals**  
   - User **identity** (who they are).  
   - User **location** (where they are signing in from).  
   - Device **type and security status**.  

2️⃣ **Make a Decision**  
   - **Allow full access** – If sign-in is from a known, trusted location.  
   - **Challenge with MFA** – If the sign-in is from an unusual or high-risk location.  
   - **Block access** – If the sign-in is from an **untrusted** or **high-risk** source.  

3️⃣ **Enforce the Decision**  
   - **Allow** access.  
   - **Require MFA** (e.g., second authentication factor).  
   - **Deny** access.  

![CondAccessProcess](https://learn.microsoft.com/en-us/training/wwl-azure/describe-azure-identity-access-security/media/conditional-access-9bd268b8-757297cb.png)

---

## **When to Use Conditional Access?**  

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**  
✅ **Require MFA** based on user role, location, or network.  
✅ **Limit access** to services only through **approved client applications**.  
✅ **Restrict access** to only **managed, secure devices**.  
✅ **Block access** from **untrusted sources** (e.g., unknown or unexpected locations).  

---

## **Example Use Cases**  

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  
- **MFA for admins, but not regular users**.  
- **Only approved email apps can connect to company email**.  
- **Users must sign in from company-managed devices**.  
- **Block logins from unknown locations** to prevent unauthorized access.  

