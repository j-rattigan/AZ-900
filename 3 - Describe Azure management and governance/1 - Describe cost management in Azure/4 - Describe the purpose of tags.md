# Azure Resource Tags  

## ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
Tags are used to organize and manage Azure resources efficiently. They help with:  
- **Resource Management** – Quickly locate and group resources by workloads, business units, or owners.  
- **Cost Optimization** – Track spending by grouping resources and allocating budgets.  
- **Operations & Security** – Classify resources based on criticality, security level, or compliance.  

---

## ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Supporting Details**  

### **Managing Resource Tags**  
- Tags can be added, modified, or deleted using:  
  - **Azure Portal**  
  - **Azure CLI**  
  - **PowerShell**  
  - **REST API**  
  - **Azure Resource Manager Templates**  
- Tags **do not inherit** from subscriptions or resource groups, allowing flexible customization.  
- **Azure Policy** can enforce tagging rules to ensure compliance and consistency.  

### **Use Cases for Tags**  
| **Purpose** | **How Tags Help** |  
|------------|------------------|  
| **Governance & Compliance** | Ensures alignment with regulations like ISO 27001. |  
| **Workload Optimization** | Helps track resources involved in complex deployments. |  
| **Automation** | Enables tools like Azure DevOps to automate resource management. |  

---

## ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Examples/ Facts** 

- **Example Tag Structure:**  
  | **Tag Name** | **Value** |  
  |------------|---------|  
  | AppName | Name of the application using the resource |  
  | CostCenter | Internal cost center code |  
  | Owner | Business owner responsible for the resource |  
  | Environment | "Prod," "Dev," or "Test" |  
  | Impact | "Mission-Critical," "High-Impact," or "Low-Impact" |  

- **Fact:** Tags allow you to track which resources are **mission-critical** by using the "Impact" tag. Non-tagged resources are automatically considered **non-critical**.  

---

