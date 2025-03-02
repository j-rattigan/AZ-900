# **Azure Role-Based Access Control (RBAC)**  

Azure **RBAC** is a system that **manages permissions** to **control who can access what** in your cloud environment.

---

## **Why is Azure RBAC Important?**  

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
🔹 **Follows the Principle of Least Privilege** – Users should only have the **minimum access** needed to complete their tasks.  
🔹 **Prevents Over-Permissioning** – Example: If a user only needs **read access** to a **storage blob**, they **shouldn’t** get **write access**.  
🔹 **Simplifies Permission Management** – Instead of assigning permissions **one by one**, Azure RBAC allows you to **assign roles to groups**.  

---

## **How Azure RBAC Works**  

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**  
- **Azure RBAC** – A security system that controls access to Azure resources **based on roles**.  
- **Roles** – A set of **permissions** assigned to a user or group (e.g., **Owner, Reader, Contributor**).  
- **Scope** – The **range of resources** a role applies to (e.g., **Subscription, Resource Group, Individual Resource**).  
- **Inheritance** – When a **parent scope** has a role, it automatically applies to **all child scopes**.  

---

## **RBAC Example**  

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  
💡 **Scenario:** You hire a new engineer. Instead of manually assigning them **access to every resource**, you:  
✅ Add them to the **Azure RBAC group for engineers**.  
✅ They **automatically** get the **same access** as other engineers.  
✅ If **new resources** are added, they **inherit permissions** without needing changes.  

---

## **How is Role-Based Access Applied?**  

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**  
🔹 **RBAC is applied at a Scope**, which can be:  
   - **Management Group** (multiple subscriptions).  
   - **Subscription** (all resources within).  
   - **Resource Group** (a collection of related resources).  
   - **Single Resource** (an individual VM, storage account, etc.).  

🔹 **Example:**  
   - If a **user is assigned "Owner"** at the **Management Group** level, they **control all subscriptions** within it.  
   - If a **group is assigned "Reader"** at the **Subscription** level, all members can **view all resources** but **not edit them**.  

![HowRBAC](https://learn.microsoft.com/en-us/training/wwl-azure/describe-azure-identity-access-security/media/role-based-access-scope-4b12a8f3-7f40fc55.png)

---

## **How is Azure RBAC Enforced?**  

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
🔹 **Azure RBAC is enforced** through **Azure Resource Manager** (ARM).  
🔹 **RBAC only applies to Azure resource management**, **not application security**.  
🔹 **RBAC uses an "Allow" model** – If you have multiple roles, **you inherit the highest level of permission**.  

💡 **Example:**  
   - If **one role grants Read access** to a resource group…  
   - And **another role grants Write access** to the same group…  
   - The user **has both Read & Write access**.  

---

## **Key Takeaways**  

✅ **RBAC helps manage permissions efficiently** by assigning **roles instead of individual permissions**.  
✅ **RBAC applies to different scopes** and follows a **hierarchical structure** (higher levels inherit permissions).  
✅ **RBAC is enforced through Azure Resource Manager** and **does not** control application-level security.  

