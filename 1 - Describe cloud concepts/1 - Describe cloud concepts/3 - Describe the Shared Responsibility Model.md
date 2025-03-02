# Describe the Shared Responsibility Model

The **Shared Responsibility Model** defines the division of responsibilities between the **cloud provider** and the **consumer** in cloud computing.

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
- In traditional data centers, a company is responsible for maintaining the physical space, servers, security, and software.
- In cloud computing, the responsibility is shared between the cloud provider and the consumer.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key terms and definitions**
- **Shared Responsibility Model**: The framework that divides responsibilities between the cloud provider and the consumer. It covers physical security, infrastructure, data, and access security.
- **Cloud Provider**: The entity that delivers cloud services, responsible for maintaining the physical infrastructure (e.g., datacenters, servers, security).
- **Consumer**: The user or organization using cloud services, responsible for managing the data, access security, and some infrastructure components.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**

| Cloud providers are responsible for | Consumers are responsible for |
|----------|----------|
| - Physical security <br> - Power and cooling <br> - Network connectivity <br>- The physical datacenter and network infrastructure | - Data stored in the cloud <br> - Managing access security (who can access what) <br> - Devices that connect to the cloud (e.g., phones, computers)|  

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- Example: In a traditional data center, your IT department maintains everything, but in the cloud, the provider handles infrastructure, while you handle data and access control.
- Example: If using a **cloud SQL database**:
  - The cloud provider maintains the database itself.
  - The consumer is responsible for the data in the database.
- Example: With a **virtual machine (VM)**, the consumer installs and maintains the SQL database and its updates, as well as the data within it.

![Image Alt Text](https://learn.microsoft.com/en-us/training/wwl-azure/describe-cloud-compute/media/shared-responsibility-b3829bfe.svg)

