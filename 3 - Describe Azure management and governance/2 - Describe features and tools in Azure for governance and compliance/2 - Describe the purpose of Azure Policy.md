# Azure Policy  

## ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
Azure Policy is a service that **creates, assigns, and manages policies** to enforce compliance and control resource configurations.  

It helps organizations:  
- **Ensure compliance** with corporate and regulatory standards.  
- **Prevent noncompliant resources** from being created.  
- **Automatically remediate** certain policy violations.  

---

## ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Supporting Details**  

### **How Azure Policy Works**  
1. **Defines & Enforces Rules** – Ensures resources follow specific policies.  
2. **Evaluates Compliance** – Highlights noncompliant resources.  
3. **Automatic Remediation** – Fixes certain policy violations (e.g., missing tags).  
4. **Policy Inheritance** – Policies applied at higher levels (subscription, resource group) automatically apply to lower levels.  

### **Azure Policy vs. Policy Initiatives**  
| **Feature** | **What It Does** |  
|------------|----------------|  
| **Policy** | Defines a single rule to enforce compliance. |  
| **Initiative** | Groups multiple policies for tracking compliance on a larger scale. |  

### **Integration with DevOps**  
Azure Policy integrates with **Azure DevOps**, applying rules during:  
- **Pre-deployment** (before resources are created).  
- **Post-deployment** (ongoing compliance monitoring).  

---

## ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Examples/ Facts**  

- **Example:**  
  A company requires all virtual machines (VMs) to be a specific size. **Azure Policy enforces this rule**, preventing noncompliant VMs from being created or resized.  

- **Fact:**  
  Policies apply at different levels: **resource, resource group, subscription** – and policies set at higher levels automatically apply to lower levels.  

- **Initiative Example:**  
  The **"Enable Monitoring in Azure Security Center"** initiative contains **over 100 policies**, including:  
  - Monitoring unencrypted SQL databases.  
  - Checking OS vulnerabilities.  
  - Ensuring endpoint protection is installed.  

---
