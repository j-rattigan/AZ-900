#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**

### Azure Management Infrastructure Overview
The Azure management infrastructure includes **Azure resources**, **resource groups**, **subscriptions**, and **accounts**.  
Understanding this hierarchy will help you organize your projects and products within Azure.

---

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**

- **Azure Resources**: Anything you create, provision, or deploy in Azure, such as Virtual Machines (VMs), virtual networks, databases, etc.
- **Resource Groups**: Logical containers for resources. They group resources together, and actions on a resource group apply to all resources within it.

---

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**

### Resource Groups
- When you create a resource, you place it into a **resource group**.
- A **resource** can only belong to **one** resource group at a time. You can move it between groups, but it will no longer be in the original group.
- **Resource groups cannot be nested**.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Action on Resource Group**: Deleting a resource group deletes all its resources.
- **Access Control**: Granting or denying access to a resource group applies to all resources within it.

![ResourceGroups](https://learn.microsoft.com/en-us/training/wwl-azure/describe-core-architectural-components-of-azure/media/resource-group-eb2d7177-ff67d816.png)

---

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**

- **Azure Subscriptions**: Units of management, billing, and scale that organize your Azure resources and their access control.
- **Subscription Boundaries**:
    - **Billing Boundary**: Defines how Azure costs are billed and reported.
    - **Access Control Boundary**: Defines how access policies are applied.

---

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**

### Subscriptions
- **Azure subscription** links to an **Azure account** for identity and authorization (via **Microsoft Entra ID**).
- An account can have **multiple subscriptions** for different purposes (e.g., different billing models, resource access policies).

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- You can create additional subscriptions to separate environments like **development**, **production**, or for **compliance** reasons.
- **Separate Subscriptions for Billing**: Different subscriptions can be used for managing costs, e.g., one for **production** workloads and another for **development**.
    - 
![Subscriptions](https://learn.microsoft.com/en-us/training/wwl-azure/describe-core-architectural-components-of-azure/media/subscriptions-d415577b-04961c4b.png)

---

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**

- **Management Groups**: Containers for **Azure subscriptions** that allow you to apply governance and management policies.

---

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**

### Management Groups
- **Management groups** are used to organize **subscriptions**. 
- Policies applied to a **management group** affect all subscriptions and resources underneath it.
- **Nested Management Groups**: You can nest management groups up to 6 levels deep.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Policy Inheritance**: A policy (like limiting VM locations to a region) will automatically apply to all subscriptions within a management group.
- **User Access**: Azure RBAC (Role-Based Access Control) assigned at the management group level will apply to all resources below it.

![ManagementGroups](https://github.com/user-attachments/assets/b1bc8adc-4996-4c79-92ba-4b7173906dce)

---

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**

### Key Facts About Management Groups
- **Up to 10,000 management groups** can be supported in a single directory.
- **Management groups** can have up to **6 levels of nesting**.
- Each management group and subscription can only have **one parent**.

---
