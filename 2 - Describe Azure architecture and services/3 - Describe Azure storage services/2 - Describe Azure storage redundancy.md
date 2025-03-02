# Describe Azure storage redundancy
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
Azure Storage always stores multiple copies of your data to protect against **planned and unplanned events** like hardware failures, power outages, or disasters. Redundancy ensures **availability** and **durability** even in the face of failures.

When choosing a redundancy option, consider:
- **Cost vs. availability**
- How data is replicated in the **primary region**
- Replication to a **secondary region** for disaster protection
- **Read access** to replicated data in secondary regions

---

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Redundancy**: Storing multiple copies of data to protect against failures.
- **Availability**: The ability to access data when needed.
- **Durability**: The likelihood that data will remain intact and uncorrupted over time.
- **Recovery Point Objective (RPO)**: The time gap between the last write in the primary region and the copy in the secondary region.

---

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- **Primary Region Replication**:
  - **Locally Redundant Storage (LRS)**: Data replicated 3 times in the primary region, but if a disaster strikes the region, all replicas could be lost.
  - **Zone-Redundant Storage (ZRS)**: Data replicated across **three availability zones** in the primary region. **High availability** even if one zone fails.
  - **Recommendation**: Use **ZRS** for high availability requirements.

---

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Locally Redundant Storage (LRS)**:
  - **Durability**: 99.999999999% (11 nines).
  - **Use**: Protects against server rack and drive failures, but not regional disasters.

![LRS](https://learn.microsoft.com/en-us/training/wwl-azure/describe-azure-storage-services/media/locally-redundant-storage.png)

- **Zone-Redundant Storage (ZRS)**:
  - **Durability**: 99.9999999999% (12 nines).
  - **Use**: Suitable for high availability and keeping data within a specific region.

![ZRS](https://learn.microsoft.com/en-us/training/wwl-azure/describe-azure-storage-services/media/zone-redundant-storage.png)
---

## - **Secondary Region Redundancy**:
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
  - **Geo-Redundant Storage (GRS)**: Replicates data from the primary region to a **secondary region** for **regional disaster protection**.
  - **Geo-Zone-Redundant Storage (GZRS)**: Combines **ZRS** in the primary region and **LRS** in the secondary region for both high availability and protection from regional outages.

## - **Geo-Zone-Redundant Storage (GZRS)**:
  - **Durability**: At least 99.99999999999999% (16 nines).
  - **Use**: For maximum consistency, durability, and disaster recovery.

---

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Geo-Redundant Storage (GRS)**: Replicates data to a secondary region asynchronously. 
- **Geo-Zone-Redundant Storage (GZRS)**: Combines **ZRS** in the primary region and **LRS** in the secondary region.

---

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Read Access**: 
  - With **RA-GRS** (Read-Access Geo-Redundant Storage) or **RA-GZRS** (Read-Access Geo-Zone-Redundant Storage), data is available to read even when the **primary region is available**.
  - **Important**: The secondary region data may not be up-to-date due to **RPO**.

---
#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**

- **Geo-Redundant Storage (GRS)**: RPO is typically **less than 15 minutes**, but there is no SLA for replication time.

![GRS](https://learn.microsoft.com/en-us/training/wwl-azure/describe-azure-storage-services/media/geo-redundant-storage.png)
---

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- **Data Loss Risk**: Asynchronous replication between primary and secondary regions means that if the primary region fails, **data loss is possible** due to the time lag in replication.
