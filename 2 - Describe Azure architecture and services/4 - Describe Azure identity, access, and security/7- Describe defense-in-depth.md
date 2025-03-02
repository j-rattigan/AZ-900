# **Defense-in-Depth Security Model**  

Defense-in-depth is a **layered security strategy** that protects information by **slowing attacks and preventing unauthorized access**.

---
# Defense-in-Depth Overview

## **Why is Defense-in-Depth Important?**  

| **Category** | **Details** |
|--------------|-------------|
| ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important** | 🔹 Prevents unauthorized access to data <br> 🔹 Uses multiple security layers – If one layer is breached, another protects against further exposure. <br> 🔹 Reduces reliance on a single security measure <br> 🔹 Provides alerts for security teams to respond to threats. |
| ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions** | - **Defense-in-Depth**: A security strategy using multiple layers of protection to prevent attacks. <br> - **Layered Security**: Each layer has its own security controls, protecting data at the center. <br> - **Least Privilege Access**: Users and systems get only the access they need to perform their tasks. <br> - **DDoS Protection**: Defends against large-scale attacks that could disrupt services. |
| ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important** | **Layers of Security** (from outer to inner): |

---

## **Layers of Defense-in-Depth**
![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
Defense-in-depth is **visualized as layers**, with **data at the center** and other security layers protecting it.

| **Category** | **Details** |
|--------------|-------------|
| ![DefinDepth](https://learn.microsoft.com/en-us/training/wwl-azure/describe-azure-identity-access-security/media/defense-depth-486afc12-71a03f12.png) | **Layers of Security** (from outer to inner): <br> 1️⃣ **Physical Security** – Protects **buildings and hardware**. <br> 2️⃣ **Identity & Access** – Manages **user authentication and access control**. <br> 3️⃣ **Perimeter Security** – Uses **firewalls and DDoS protection** to stop large attacks. <br> 4️⃣ **Network Security** – **Limits internal communication** to stop attacks from spreading. <br> 5️⃣ **Compute Security** – Protects **virtual machines and devices** from malware and vulnerabilities. <br> 6️⃣ **Application Security** – Ensures **secure app development** with encryption and best practices. <br> 7️⃣ **Data Security** – **Controls access to sensitive business and customer data**. |

---

## **Breaking Down Each Layer**  

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  

<table style="border: 4px solid black; border-collapse: collapse;">
  <tr>
    <th style="border: 4px solid black; padding: 8px; text-align: left;">🔒 1. Physical Security</th>
    <th style="border: 4px solid black; padding: 8px; text-align: left;">🔑 2. Identity & Access Security</th>
    <th style="border: 4px solid black; padding: 8px; text-align: left;">🌍 3. Perimeter Security</th>
    <th style="border: 4px solid black; padding: 8px; text-align: left;">📡 4. Network Security</th>
    <th style="border: 4px solid black; padding: 8px; text-align: left;">💻 5. Compute Security</th>
    <th style="border: 4px solid black; padding: 8px; text-align: left;">📱 6. Application Security</th>
    <th style="border: 4px solid black; padding: 8px; text-align: left;">📊 7. Data Security</th>
  </tr>
  <tr>
    <td style="border: 4px solid black; padding: 8px;">🏢 **Protects datacenter buildings and computing hardware.** <br> ✅ **Controlled access** to prevent unauthorized entry. <br> ✅ **Monitors and secures physical assets** (e.g., servers, storage). <br></td>
    <td style="border: 4px solid black; padding: 8px;">👤 **Manages user authentication and access control.** <br> ✅ **Uses Single Sign-On (SSO) & Multi-Factor Authentication (MFA).** <br> ✅ **Controls access to infrastructure and tracks sign-in events.** <br></td>
    <td style="border: 4px solid black; padding: 8px;">🛑 **Defends against large-scale network attacks.** <br> ✅ **Uses Distributed Denial of Service (DDoS) protection.** <br> ✅ **Deploys perimeter firewalls to detect malicious traffic.** <br></td>
    <td style="border: 4px solid black; padding: 8px;">🌐 **Limits communication between resources to reduce attack spread.** <br> ✅ **Deny-by-default approach** – Blocks traffic unless explicitly allowed. <br> ✅ **Restricts internet access** (both inbound & outbound). <br> ✅ **Implements secure connections between cloud and on-premises networks.** <br></td>
    <td style="border: 4px solid black; padding: 8px;">🖥️ **Protects virtual machines & computing resources.** <br> ✅ **Secures access to VMs.** <br> ✅ **Uses endpoint protection & keeps systems patched.** <br></td>
    <td style="border: 4px solid black; padding: 8px;">🛠️ **Builds security into the development lifecycle.** <br> ✅ **Ensures apps are free of vulnerabilities.** <br> ✅ **Stores sensitive information securely.** <br></td>
    <td style="border: 4px solid black; padding: 8px;">🔐 **Protects stored business & customer data.** <br> ✅ **Controls access to databases, storage, and SaaS applications.** <br> ✅ **Ensures regulatory compliance for data protection.** <br></td>
  </tr>
</table>



## **Key Takeaways**  

✅ **Defense-in-depth = Multiple security layers to slow down attacks.**  
✅ **If one layer fails, others protect against further damage.**  
✅ **Data is the most valuable asset and must be secured at all times.**  
✅ **Azure provides security tools for every layer of defense.**  

