# Azure Physical Infrastructure

This section covers the core architectural components of Azure's physical infrastructure, including datacenters, regions, availability zones, region pairs, and sovereign regions.

---
| **Component**  | ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important** | ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Supporting Details** | ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Examples/ Facts** |
|------------------------------|----------------------------------|-----------------------------------------|----------------------------------------------|
| **Azure Physical Infrastructure** | Azure’s physical infrastructure starts with datacenters—facilities similar to large corporate datacenters with dedicated power, cooling, and networking. | 🔹 **Datacenter**: A facility with racks of servers and supporting infrastructure. <br> 🔹 **Physical Infrastructure**: The hardware and facilities that support cloud services. | 🔹 **Datacenters**: Are not directly accessible; they are organized to support business-critical workloads by ensuring redundancy and low latency. |
| **Regions** | A Region is a geographical area that contains one or more datacenters connected with low-latency networks. You must often choose a region when deploying Azure resources. | 🔹 **Region**: A geographical grouping of datacenters. <br> 🔹 **Low-Latency Network**: A fast network connecting datacenters in the same region. | 🔹 **Azure Regions**: Azure intelligently assigns and controls resources within a region to balance workloads efficiently. <br> 🔹 **Global Azure Services**: (e.g., Microsoft Entra ID, Azure Traffic Manager) do not require region selection. |

---

## Availability Zones

| **Component**             | ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important** | ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Supporting Details** | ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Examples/ Facts** |
|---------------------------|----------------------------------|-----------------------------------------|----------------------------------------------|
| **Availability Zones**    | Availability Zones are physically separate datacenters within a single region. Each zone has its own power, cooling, and networking to act as an isolation boundary. | 🔹 **Availability Zone**: A separate datacenter or group of datacenters within a region designed for fault isolation. <br> 🔹 **Isolation Boundary**: A feature that prevents failures in one zone from affecting others. | 🔹 **Usage**: VMs, managed disks, load balancers, and SQL databases can be zonal, zone-redundant, or non-regional. <br> 🔹 **Cost Consideration**: Duplicating services and transferring data between zones may incur extra costs. |

![Availability Zones](https://learn.microsoft.com/en-us/training/wwl-azure/describe-core-architectural-components-of-azure/media/availability-zones-c22f95a3-14cd8677.png)

---

## Region Pairs

| **Component**             | ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important** | ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Supporting Details** | ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Examples/ Facts** |
|---------------------------|----------------------------------|-----------------------------------------|----------------------------------------------|
| **Region Pairs**          | Region Pairs consist of two Azure regions within the same geography, located at least 300 miles apart to provide disaster recovery and failover options. | 🔹 **Region Pair**: Two regions paired together for resource replication and resilience. <br> 🔹 **Failover**: The automatic switching to a redundant system in case of failure. | 🔹 **Examples**: West US paired with East US, South-East Asia paired with East Asia. <br> 🔹 **Special Cases**: Some regions have one-direction pairing, meaning only one region backs up the other. |

![Region Pairs](https://learn.microsoft.com/en-us/training/wwl-azure/describe-core-architectural-components-of-azure/media/region-pairs-7c495a33-85c0fa20.png)

---

## Sovereign Regions

| **Component**             | ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important** | ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Supporting Details** | ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Examples/ Facts** |
|---------------------------|----------------------------------|-----------------------------------------|----------------------------------------------|
| **Sovereign Regions**     | Sovereign Regions are isolated instances of Azure, set apart for compliance or legal requirements. | 🔹 **Sovereign Region**: An Azure instance isolated from the main Azure cloud, tailored for government or compliance needs. | 🔹 **Examples**: US DoD Central, US Gov Virginia, US Gov Iowa; China East, China North. <br> 🔹 These regions include additional compliance certifications and operate under strict security controls. |

---
