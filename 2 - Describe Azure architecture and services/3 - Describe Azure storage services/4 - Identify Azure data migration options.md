# Azure Data Migration Options

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- Azure supports **real-time migration** of infrastructure, applications, and data using **Azure Migrate**.
- Azure also supports **asynchronous migration** of data using **Azure Data Box**.

---

## Azure Migrate

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Azure Migrate**: A service that helps migrate on-premises environments to Azure.
- **Unified migration platform**: A single portal to start, run, and track migrations.
- **Integrated tools**: Built-in tools and third-party integrations for assessment and migration.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- Azure Migrate **assesses** and **migrates** on-premises infrastructure, databases, and applications.
- It **supports migration** of **VMware VMs, Hyper-V VMs, physical servers, and public cloud VMs**.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
Azure Migrate includes the following tools:
- **Azure Migrate: Discovery and Assessment** → Scans and evaluates **on-premises servers** for migration readiness.
- **Azure Migrate: Server Migration** → Moves VMs and physical servers to Azure.
- **Data Migration Assistant** → Evaluates **SQL Server** for unsupported features and migration readiness.
- **Azure Database Migration Service** → Migrates **databases** to **Azure SQL or SQL Managed Instances**.
- **Azure App Service Migration Assistant** → Assesses and migrates **.NET and PHP web apps**.

---

## Azure Data Box

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Azure Data Box**: A physical device used to transfer large amounts of data to and from Azure.
- **Maximum Storage Capacity**: **80 terabytes**.
- **Offline Data Transfer**: Ideal for situations where network connectivity is limited.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- The Data Box is **delivered to your datacenter** for local data transfer.
- Once the data is transferred, **the device is shipped back to Microsoft** for upload to Azure.
- The process is **tracked end-to-end** via the **Azure portal**.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
**Use Cases for Data Box (Import to Azure)**
1. **One-time migration** → Move large amounts of data to Azure.
   - Example: Moving a media library from **offline tapes** into Azure.
2. **Initial bulk transfer** → Perform an initial large transfer, followed by smaller **incremental updates** over the network.
3. **Periodic uploads** → Transfer large **recurring data loads**.

**Use Cases for Data Box (Export from Azure)**
1. **Disaster recovery** → Quickly restore Azure data **on-premises** after a failure.
2. **Security compliance** → Export data due to **government/security policies**.
3. **Cloud provider migration** → Move workloads **back on-premises** or to another cloud provider.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **NIST 800-88r1 standards** → Ensures that disks are **wiped securely** after data transfer.
- **Regional carrier shipping** → Ensures **safe transport** of the Data Box.

---

## Summary

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- **Azure Migrate** is the primary tool for **real-time migration** of infrastructure, apps, and data.
- **Azure Data Box** is a **physical device** for transferring large volumes of data **offline**.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- **Azure Migrate** helps **assess, plan, and execute** cloud migrations.
- **Azure Data Box** is used when **network bandwidth is limited** or when transferring **very large data sets**.
