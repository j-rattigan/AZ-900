# Azure Virtual Networking Overview
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
Azure virtual networks enable Azure resources to communicate with each other, users on the internet, and your on-premises resources. Think of it as an extension of your on-premises network.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Virtual Network (VNet):** A private network in Azure that provides isolation, segmentation, and secure communication between resources.
- **Subnets:** Smaller address spaces within a VNet that help organize and secure resources.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- VNet enables secure communication between resources, including VMs, web apps, and databases.
- Key capabilities include routing traffic, filtering traffic, and connecting virtual networks.

---

# Key Networking Capabilities of Azure Virtual Networks
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- **Isolation and segmentation** – Create isolated networks within Azure.
- **Internet communications** – Enable external communication via public IP addresses.
- **Internal communication** – Enable secure communication between Azure resources.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Public Endpoints:** Accessible from anywhere with a public IP.
- **Private Endpoints:** Only accessible within a VNet with a private IP.

---

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Isolation & Segmentation:** Define private IP address space; not internet routable. Can segment into subnets.
- **Internet Communications:** Use public IP or load balancer for inbound internet connections.
- **Communicate Between Resources:** 
  - **VMs, App Services, and Kubernetes** can all communicate through VNets.
  - Use **Service Endpoints** to connect resources like Azure SQL Database and storage accounts to VNets for enhanced security.

---

# How to Connect On-Premises to Azure
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
Azure allows you to create a hybrid network with your on-premises environment.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Point-to-site VPN:** Secure connection from a single computer to Azure VNet.
- **Site-to-site VPN:** Connects on-premises VPN device to Azure’s VPN gateway.
- **Azure ExpressRoute:** Dedicated private connection to Azure, bypassing the internet.

---

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- **ExpressRoute** is used for higher bandwidth and better security.
- **VPN connections** help link local and cloud environments, providing seamless connectivity.

---

# Routing and Filtering Network Traffic
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
Azure allows for traffic management between subnets and between on-premises and Azure.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Route Tables:** Rules for how traffic is directed between subnets.
- **BGP (Border Gateway Protocol):** Propagates on-premises routes to Azure virtual networks.
- **NSGs (Network Security Groups):** Inbound and outbound security rules for controlling traffic.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- **Network Security Groups (NSGs)** allow you to create custom rules to allow/block traffic based on IP addresses, ports, and protocols.
- **Network Virtual Appliances (NVAs)** function as firewalls or optimize WAN.

---

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Virtual Network Peering** allows direct, private communication between virtual networks. Traffic travels over Microsoft's backbone network and not the public internet.
- **User-Defined Routes (UDR)** give you more control over traffic flow between subnets or VNets.

---

# Summary of Azure Virtual Networking
Azure Virtual Networks provide secure and scalable networking capabilities to connect resources both within Azure and with on-premises systems, enabling full control over traffic routing, security, and communication.
