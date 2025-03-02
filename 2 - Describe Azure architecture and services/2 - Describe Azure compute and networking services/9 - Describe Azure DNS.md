# **Azure DNS**  
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
Azure DNS is a hosting service for DNS domains, providing name resolution using **Microsoft Azure** infrastructure. You can manage your DNS records using the same credentials, APIs, tools, and billing as your other Azure services.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**  
**DNS (Domain Name System):** A system that translates domain names into IP addresses.  
**Azure DNS:** A service that hosts DNS domains on Microsoft Azure infrastructure.

---

# **Benefits of Azure DNS**  
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
1. **Reliability & Performance**  
2. **Security**  
3. **Ease of Use**  
4. **Customizable Virtual Networks**  
5. **Alias Records**

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**  
**Anycast Networking:** A method where multiple DNS servers respond to queries, selecting the nearest one for faster performance.  
**Azure Resource Manager (ARM):** The management framework used for deploying and managing Azure resources.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**  
**Reliability & Performance:**  
DNS domains are hosted on Azure's global network of DNS servers, providing:  
- **High availability**  
- **Fast performance**  
**Security:**  
Azure DNS is built on **Azure Resource Manager (ARM)** and provides:  
- **Azure Role-Based Access Control (RBAC):** Manages access to resources.  
- **Activity Logs:** Tracks user actions for troubleshooting.  
- **Resource Locking:** Prevents accidental changes or deletions.

---

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  
- **Alias Records:**  
  Use alias records to point to Azure resources (e.g., **Azure Public IP**, **Azure CDN**, **Azure Traffic Manager**) and have them automatically update if the underlying resource's IP changes.  
- **Ease of Use:**  
  Azure DNS integrates with the **Azure portal, PowerShell, and CLI**, allowing seamless DNS management for both internal and external resources.

---

# **Limitations of Azure DNS**  
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
Azure DNS does **not** allow you to **buy a domain name** directly. You can purchase a domain through App Service Domains or a third-party registrar, then host it in Azure DNS for record management.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**  
**App Service Domains:** A service from Azure to buy domain names.  
**Third-party Domain Registrar:** An external service to buy domain names, e.g., GoDaddy.
