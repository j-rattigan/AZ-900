# **Defense-in-Depth Security Model**  

Defense-in-depth is a **layered security strategy** that protects information by **slowing attacks and preventing unauthorized access**.

---

## **Why is Defense-in-Depth Important?**  

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
🔹 **Prevents unauthorized access to data**  
🔹 **Uses multiple security layers** – If one layer is breached, another protects against further exposure.  
🔹 **Reduces reliance on a single security measure**  
🔹 **Provides alerts** for security teams to respond to threats.  

---

## **What is Defense-in-Depth?**  

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**  

- **Defense-in-Depth** – A security strategy using **multiple layers of protection** to prevent attacks.  
- **Layered Security** – Each layer has its own security controls, **protecting data at the center**.  
- **Least Privilege Access** – Users and systems get **only the access they need** to perform their tasks.  
- **DDoS Protection** – **Defends against large-scale attacks** that could disrupt services.  

---

## **Layers of Defense-in-Depth**  

Defense-in-depth is **visualized as layers**, with **data at the center** and other security layers protecting it.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**  

🔹 **Layers of Security (from outer to inner):**  
1️⃣ **Physical Security** – Protects **buildings and hardware**.  
2️⃣ **Identity & Access** – Manages **user authentication and access control**.  
3️⃣ **Perimeter Security** – Uses **firewalls and DDoS protection** to stop large attacks.  
4️⃣ **Network Security** – **Limits internal communication** to stop attacks from spreading.  
5️⃣ **Compute Security** – Protects **virtual machines and devices** from malware and vulnerabilities.  
6️⃣ **Application Security** – Ensures **secure app development** with encryption and best practices.  
7️⃣ **Data Security** – **Controls access to sensitive business and customer data**.  

![DefinDepth](https://learn.microsoft.com/en-us/training/wwl-azure/describe-azure-identity-access-security/media/defense-depth-486afc12-71a03f12.png)

---

## **Breaking Down Each Layer**  

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  

### **🔒 1. Physical Security**  
🏢 **Protects datacenter buildings and computing hardware.**  
✅ **Controlled access** to prevent unauthorized entry.  
✅ **Monitors and secures physical assets** (e.g., servers, storage).  

---

### **🔑 2. Identity & Access Security**  
👤 **Manages user authentication and access control.**  
✅ **Uses Single Sign-On (SSO) & Multi-Factor Authentication (MFA).**  
✅ **Controls access to infrastructure and tracks sign-in events.**  

---

### **🌍 3. Perimeter Security**  
🛑 **Defends against large-scale network attacks.**  
✅ **Uses Distributed Denial of Service (DDoS) protection.**  
✅ **Deploys perimeter firewalls to detect malicious traffic.**  

---

### **📡 4. Network Security**  
🌐 **Limits communication between resources to reduce attack spread.**  
✅ **Deny-by-default approach** – Blocks traffic unless explicitly allowed.  
✅ **Restricts internet access** (both inbound & outbound).  
✅ **Implements secure connections between cloud and on-premises networks.**  

---

### **💻 5. Compute Security**  
🖥️ **Protects virtual machines & computing resources.**  
✅ **Secures access to VMs.**  
✅ **Uses endpoint protection & keeps systems patched.**  

---

### **📱 6. Application Security**  
🛠️ **Builds security into the development lifecycle.**  
✅ **Ensures apps are free of vulnerabilities.**  
✅ **Stores sensitive information securely.**  

---

### **📊 7. Data Security**  
🔐 **Protects stored business & customer data.**  
✅ **Controls access to databases, storage, and SaaS applications.**  
✅ **Ensures regulatory compliance for data protection.**  

---

## **Key Takeaways**  

✅ **Defense-in-depth = Multiple security layers to slow down attacks.**  
✅ **If one layer fails, others protect against further damage.**  
✅ **Data is the most valuable asset and must be secured at all times.**  
✅ **Azure provides security tools for every layer of defense.**  

