# **Azure ExpressRoute**
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
Azure ExpressRoute allows you to extend your on-premises network to the Microsoft cloud via a private connection with a provider. This connection is called an **ExpressRoute Circuit**.  
It provides a faster, more reliable, and secure connection compared to the public internet.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**  
**ExpressRoute Circuit:** A private connection used to connect your on-premises network to the Microsoft cloud.  
**Connectivity Provider:** The service that facilitates the private connection for ExpressRoute.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**  
- **Connectivity Options:**  
  1. **Any-to-any IP VPN**  
  2. **Point-to-point Ethernet Network**  
  3. **Virtual Cross-Connection**  

These options allow secure, fast connections without using the public internet.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  
ExpressRoute connections offer:  
- **Reliability**: More consistent speeds and latencies than public internet.  
- **Higher Security**: Data doesn’t travel over the internet.  
- **Global Connectivity**: Access to Microsoft services worldwide.

---

# **Benefits of ExpressRoute**  
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
- **Direct Connectivity** to Microsoft cloud services, including:  
  - **Microsoft Office 365**
  - **Microsoft Dynamics 365**
  - **Azure Virtual Machines**
  - **Azure Storage & Cosmos DB**

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**  
**BGP (Border Gateway Protocol):** Used to exchange routing information between on-premises networks and Azure services.  
**ExpressRoute Global Reach:** Enables data exchange across different on-premises locations without using the public internet.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**  
**Dynamic Routing**  
ExpressRoute uses **BGP** for dynamic routing, which adapts to network changes automatically.  

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  
- If you have an office in Asia and a datacenter in Europe, you can connect them with **ExpressRoute Global Reach** to avoid using the public internet.

---

# **ExpressRoute Connectivity Models**  
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
1. **CloudExchange Colocation:** Your facility is physically colocated at a cloud exchange, where you request a virtual cross-connect to Microsoft cloud.
2. **Point-to-Point Ethernet:** Direct connection from your facility to Microsoft cloud.
3. **Any-to-Any Networks:** Integrates your wide area network (WAN) with Azure.
4. **Directly from ExpressRoute Sites:** High-speed connection directly to Microsoft’s global network.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**  
**Colocation:** Physically placing your facility at a cloud exchange to facilitate a secure connection to the Microsoft cloud.  
**ExpressRoute Direct:** Provides dual high-speed connections to Microsoft’s global network, supporting **Active/Active** connectivity.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**  
**Security Considerations**  
Since ExpressRoute doesn’t travel over the internet, it’s more secure. However, **DNS queries, certificate revocation list checks,** and some **Azure CDN requests** will still be transmitted over the public internet.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  
This separation ensures sensitive data remains private, while other data still benefits from the global Microsoft infrastructure.
