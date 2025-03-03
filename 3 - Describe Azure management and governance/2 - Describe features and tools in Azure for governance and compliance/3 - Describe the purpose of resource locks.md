# Resource Locks in Azure

## ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- A **resource lock** prevents accidental deletion or modification of resources.  
- Even with **Azure RBAC** policies, users with permissions may still delete critical resources.  
- Resource locks **override RBAC permissions**—even the owner must remove the lock before making restricted changes.  
- Locks apply at multiple levels:  
  - **Individual resources**  
  - **Resource groups**  
  - **Entire subscriptions**  
- Locks are **inherited**: If a lock is placed on a resource group, all resources inside it are affected.  

## ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Supporting Details**
### **Types of Resource Locks**
1. **Delete Lock**:  
   - Users **can read & modify** the resource.  
   - Users **cannot delete** the resource.  

2. **ReadOnly Lock**:  
   - Users **can read** the resource.  
   - Users **cannot modify or delete** the resource.  
   - This is similar to the **Reader role** in Azure RBAC.  

### **Managing Resource Locks**
- Resource locks can be managed using:  
  - **Azure Portal** (via Settings pane of a resource)  
  - **PowerShell**  
  - **Azure CLI**  
  - **Azure Resource Manager (ARM) templates**  

## ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Examples/ Facts**
- A **storage account** with a **ReadOnly Lock** prevents changes to configurations but allows data access.  
- To **modify a locked resource**, follow these steps:  
  1. **Remove the lock** first.  
  2. **Perform the action** (modify/delete) based on permissions.  
- **Example scenario**: A company applies a **Delete Lock** on its production database to prevent accidental deletion.  

