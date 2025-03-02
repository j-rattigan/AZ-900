# Describe Azure storage services

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**

- **Azure Storage** includes a variety of services for different data storage needs in the cloud. 

---

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**

- **Azure Blobs**: Massively scalable object store for text and binary data.
- **Azure Files**: Managed file shares for cloud or on-premises deployments.
- **Azure Queues**: Messaging store for reliable communication between application components.
- **Azure Disks**: Block-level storage for Azure VMs.
- **Azure Tables**: NoSQL table storage for structured, non-relational data.

---

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**

- **Benefits of Azure Storage**:
  - **Durable & Highly Available**: Redundant storage protects against hardware failures, and data can be replicated across regions.
  - **Secure**: All data encrypted by default, with fine-grained access control.
  - **Scalable**: Azure Storage grows with your application needs.
  - **Managed**: Azure takes care of hardware, updates, and critical issues.
  - **Accessible**: Accessible globally over HTTP or HTTPS, with multiple client libraries available.

---

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**

- **Azure Blobs**:
  - **Ideal for**: 
    - Serving images/documents via browser.
    - Streaming video/audio.
    - Storing backup data, or archiving.
    - Analysis of data by on-premises or Azure-hosted services.

---

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**

- **Blob storage access**: 
  - Access via HTTP, HTTPS, REST API, PowerShell, CLI, or client libraries.
  - **Storage Tiers** for Cost Management:
    - **Hot**: Frequent access (e.g., website images).
    - **Cool**: Infrequent access, stored for 30+ days (e.g., invoices).
    - **Cold**: Infrequent access, stored for 90+ days.
    - **Archive**: Rare access, stored for 180+ days (e.g., long-term backups).

---

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**

- **Hot Access Tier**: Optimized for frequently accessed data.
- **Cool Access Tier**: Optimized for infrequently accessed data.
- **Cold Access Tier**: Optimized for rarely accessed data.
- **Archive Access Tier**: Lowest-cost tier for data with flexible retrieval needs.

---

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**

- **Azure Files**:
  - Fully managed file shares with SMB or NFS protocols.
  - Supports shared access between cloud and on-premises.
  - **Benefits**: 
    - **Shared Access** via SMB/NFS protocols.
    - **Fully Managed**: No need to manage hardware or OS.
    - **Resiliency**: Always available without downtime.

---

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**

- **Azure Queues**:
  - **Message Storage** for reliable communication.
  - Supports **asynchronous processing** (e.g., triggering Azure Functions).
  - Each message up to **64KB** in size.

---

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**

- **Azure Disks**:
  - **Block-level storage** for Azure VMs.
  - Managed by Azure, with high resiliency and availability.

- **Azure Tables**:
  - NoSQL storage for structured data.
  - Ideal for **hybrid or multi-cloud solutions**.
