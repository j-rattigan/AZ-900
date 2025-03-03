# ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**

The Azure management infrastructure includes Azure resources, resource groups, subscriptions, and accounts.  
Understanding this hierarchy will help you organize your projects and products within Azure.

### Azure Resources
Anything you create, provision, or deploy in Azure, such as Virtual Machines (VMs), virtual networks, databases, etc.

### Resource Groups
Logical containers for resources. They group resources together, and actions on a resource group apply to all resources within it.

---

# ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Supporting Details**

### Action on Resource Group:
- Deleting a resource group deletes all its resources.

### Access Control:
- Granting or denying access to a resource group applies to all resources within it.

### Azure Subscriptions:
- Units of management, billing, and scale that organize your Azure resources and their access control.

### Separate Subscriptions for Billing:
- Different subscriptions can be used for managing costs, e.g., one for production workloads and another for development.

### Management Groups:
- Containers for Azure subscriptions that allow you to apply governance and management policies.

---

# ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Examples/ Facts**

- Up to 10,000 management groups can be supported in a single directory.
- Management groups can have up to 6 levels of nesting.
- Each management group and subscription can only have one parent.
