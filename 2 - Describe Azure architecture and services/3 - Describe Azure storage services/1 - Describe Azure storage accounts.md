# **Azure Storage Account**  
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
A **storage account** provides a unique namespace for your Azure Storage data that’s accessible from anywhere over HTTP or HTTPS. The data is secure, highly available, durable, and massively scalable.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**  
**Storage Account:** A service that provides a unique namespace in Azure for your storage data.  
**Namespace:** A unique identifier within Azure for storage data.

---

# **Choosing Storage Account Types**  
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
When you create a storage account, the **account type** determines which services and **redundancy options** are available.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**  
**Redundancy Options:** Methods used to replicate data to ensure availability and durability.  
**Account Type:** Defines the storage services and redundancy available.

---

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**  
**Redundancy Options**  
- **Locally Redundant Storage (LRS):** Data replicated within a single data center.  
- **Geo-Redundant Storage (GRS):** Data replicated to a secondary region.  
- **Read-Access Geo-Redundant Storage (RA-GRS):** Provides read access to data in the secondary region.  
- **Zone-Redundant Storage (ZRS):** Data replicated across multiple availability zones.  
- **Geo-Zone-Redundant Storage (GZRS):** Combines GRS and ZRS for higher resiliency.  
- **Read-Access Geo-Zone-Redundant Storage (RA-GZRS):** Provides read access to data in a geo-zone redundant setup.

---

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  
| **Account Type**             | **Supported Services**                                           | **Redundancy Options**                        | **Usage**                                                                                 |
|------------------------------|-------------------------------------------------------------------|----------------------------------------------|-------------------------------------------------------------------------------------------|
| **Standard General-purpose v2** | Blob Storage, Queue Storage, Table Storage, Azure Files         | LRS, GRS, RA-GRS, ZRS, GZRS, RA-GZRS         | Recommended for most scenarios; supports all storage services.                            |
| **Premium Block Blobs**       | Blob Storage (Data Lake Storage)                                  | LRS, ZRS                                     | For high transaction rates, smaller objects, or low latency.                             |
| **Premium File Shares**      | Azure Files                                                     | LRS, ZRS                                     | For enterprise/high-performance scale apps; supports SMB and NFS file shares.             |
| **Premium Page Blobs**       | Page Blobs only                                                  | LRS                                          | For applications needing page blobs.                                                    |

---
  
# **Naming Your Storage Account**  
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
When naming your storage account:  
- It must be between 3 and 24 characters long.  
- It can only contain numbers and lowercase letters.  
- It must be unique within Azure.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**  
**Account Name:** The unique name for your storage account in Azure.

---

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**  
**Storage Account Endpoints**  
Here’s the format for the endpoint of each Azure Storage service:

| **Storage Service**        | **Endpoint**                                               |
|----------------------------|------------------------------------------------------------|
| **Blob Storage**            | https://<storage-account-name>.blob.core.windows.net       |
| **Data Lake Storage Gen2**  | https://<storage-account-name>.dfs.core.windows.net        |
| **Azure Files**             | https://<storage-account-name>.file.core.windows.net       |
| **Queue Storage**           | https://<storage-account-name>.queue.core.windows.net      |
| **Table Storage**           | https://<storage-account-name>.table.core.windows.net      |

---
