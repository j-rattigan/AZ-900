#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
# **Azure Virtual Private Networks (VPNs)**  
A **VPN** uses an encrypted tunnel within another network, typically the public internet. It connects **trusted private networks** securely over an **untrusted** network to safely share sensitive information.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **VPN Gateway**: A virtual network gateway deployed in a dedicated subnet that enables connectivity between on-premises data centers, devices, and virtual networks.
- **Preshared Key**: A shared secret used for authentication in both **policy-based** and **route-based** VPNs.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- VPNs are typically used to encrypt traffic to prevent eavesdropping.
- There are **two types of VPNs** in Azure: **policy-based** and **route-based**.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Policy-based VPN**: Static IP addresses define which packets are encrypted.
- **Route-based VPN**: Uses IP routing to decide how to route packets based on routing protocols.

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
# **VPN Gateway Connectivity**
- **Site-to-Site**: Connects on-premises datacenters to virtual networks.
- **Point-to-Site**: Connects individual devices to virtual networks.
- **Network-to-Network**: Connects virtual networks to each other.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Active/Standby**: A configuration where one VPN instance is active, and another is on standby. When disruptions happen, the standby instance takes over.
- **Active/Active**: A configuration where both instances are active and provide redundancy with separate IPs.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- Active/standby provides automatic failover without user intervention.
- Active/active supports **BGP routing protocol** and offers better availability.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **ExpressRoute failover**: In case of **ExpressRoute** issues, a **VPN gateway** can serve as a backup using the internet to ensure continuous connectivity.
- **Zone-redundant gateways**: In availability zones, VPN and ExpressRoute gateways are deployed in multiple zones for **resiliency** and **scalability**.

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
# **High-Availability VPN Configurations**
1. **Active/Standby**: One active gateway and one standby for automatic failover.
2. **Active/Active**: Multiple active gateways, allowing for **redundancy** and **better availability**.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **BGP**: **Border Gateway Protocol**, used in active/active VPN gateways to provide dynamic routing.
- **Zone-redundant gateways**: Gateways deployed across different Azure availability zones to ensure high availability and fault tolerance.
