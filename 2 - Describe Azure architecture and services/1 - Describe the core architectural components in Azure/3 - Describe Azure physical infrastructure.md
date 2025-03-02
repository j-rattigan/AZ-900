# Azure Physical Infrastructure

This section covers the core architectural components of Azure's physical infrastructure, including datacenters, regions, availability zones, region pairs, and sovereign regions.

---

## Physical Infrastructure

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- Azure’s physical infrastructure starts with **datacenters**—facilities similar to large corporate datacenters with dedicated power, cooling, and networking.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Datacenter:** A facility with racks of servers and supporting infrastructure.
- **Physical Infrastructure:** The hardware and facilities that support cloud services.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- Datacenters are grouped into **Azure Regions** and **Availability Zones** to provide resiliency and reliability.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- Datacenters are not directly accessible; they are organized to support business-critical workloads by ensuring redundancy and low latency.

---

## Regions

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- A **Region** is a geographical area that contains one or more datacenters connected with low-latency networks.
- You must often choose a region when deploying Azure resources.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Region:** A geographical grouping of datacenters.
- **Low-Latency Network:** A fast network connecting datacenters in the same region.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- Some Azure services or specific features (like certain VM sizes or storage types) are available only in select regions.
- Global Azure services (e.g., Microsoft Entra ID, Azure Traffic Manager) do not require region selection.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- Azure intelligently assigns and controls resources within a region to balance workloads efficiently.

---

## Availability Zones

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- **Availability Zones** are physically separate datacenters within a single region.
- Each zone has its own power, cooling, and networking to act as an isolation boundary.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Availability Zone:** A separate datacenter or group of datacenters within a region designed for fault isolation.
- **Isolation Boundary:** A feature that prevents failures in one zone from affecting others.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- To ensure resiliency, at least **three separate availability zones** are present in all AZ-enabled regions.
- They support mission-critical applications by enabling redundancy and high availability.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Usage:** VMs, managed disks, load balancers, and SQL databases can be zonal, zone-redundant, or non-regional.
- **Cost Consideration:** Duplicating services and transferring data between zones may incur extra costs.

![Availability Zones](https://learn.microsoft.com/en-us/training/wwl-azure/describe-core-architectural-components-of-azure/media/availability-zones-c22f95a3-14cd8677.png)

---

## Region Pairs

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- **Region Pairs** consist of two Azure regions within the same geography, located at least 300 miles apart to provide disaster recovery and failover options.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Region Pair:** Two regions paired together for resource replication and resilience.
- **Failover:** The automatic switching to a redundant system in case of failure.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- Region pairs help reduce the impact of natural disasters or outages, ensuring continuity by replicating resources.
- Paired regions receive staggered updates to minimize downtime.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Examples:** West US paired with East US, South-East Asia paired with East Asia.
- **Special Cases:** Some regions have one-direction pairing, meaning only one region backs up the other.

![Region Pairs](https://learn.microsoft.com/en-us/training/wwl-azure/describe-core-architectural-components-of-azure/media/region-pairs-7c495a33-85c0fa20.png)

---

## Sovereign Regions

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- **Sovereign Regions** are isolated instances of Azure, set apart for compliance or legal requirements.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Sovereign Region:** An Azure instance isolated from the main Azure cloud, tailored for government or compliance needs.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- These regions often serve specific customer groups, such as U.S. government agencies or partners in China.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Examples:** US DoD Central, US Gov Virginia, US Gov Iowa; China East, China North.
- They include additional compliance certifications and operate under strict security controls.

---
