
# Azure Virtual Machines (VMs)

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
**Azure Virtual Machines (VMs)** allow you to create and use VMs in the cloud, providing Infrastructure as a Service (IaaS). They give flexibility similar to a physical computer but without needing physical hardware.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**
- **Infrastructure as a Service (IaaS)**: A cloud computing model that delivers virtualized computing resources over the internet.
- **Virtual Machine (VM)**: A virtualized server that behaves like a physical computer but is hosted in the cloud.
- **Image**: A pre-configured template used to quickly create a VM (can include OS, software, etc.).

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
VMs are ideal when you need:
- **Control over OS**: Full customization of the operating system.
- **Custom software**: Ability to run custom software in your VM.
- **Custom hosting**: Ability to configure hosting settings to suit your needs.

You still need to manage the software running on the VM, even though the hardware is handled by Azure.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- Use **preconfigured VM images** to quickly create VMs.
- **Example**: An image could already have an OS and software like development tools or web hosting environments.

---

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
You can **scale** VMs in Azure to meet the needs of your workload.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**
- **Scale Sets**: Allows you to automatically manage and configure multiple identical VMs.
- **Availability Sets**: Grouping VMs for high availability to avoid service interruption due to power or network failures.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
- **Virtual Machine Scale Sets (VMSS)**: Automatically manage, configure, and scale VMs based on demand.  
  **Example**: Azure automatically adjusts the number of VMs based on traffic or predefined schedules.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Availability Sets**: Ensure that VMs are spread across multiple power and network sources to maintain service in case of failures.

---

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
VMs are useful in many scenarios, from **testing** to **disaster recovery**.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**
- **Disaster Recovery**: The process of using cloud-based resources like VMs to recover critical applications after a failure.

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
**Examples of when to use VMs**:
1. **Testing & Development**: Easily create different OS and software configurations for testing purposes.
2. **Running Apps in Cloud**: Economically run applications with fluctuating demand.
3. **Extend Datacenter**: Move applications like SharePoint to the cloud for easier management.
4. **Disaster Recovery**: Create VMs to recover applications in case of datacenter failure.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Lift and Shift**: Move physical servers to the cloud by creating an image of the physical server and running it as a VM.

---

#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
When provisioning a VM, you also choose **resources** for that VM.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**
- **VM Resources**: Include VM size (CPU cores, RAM), storage (HDD, SSD), and networking settings (IP addresses, ports).

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**
Choosing the right resources ensures your VM is tailored to your needs.

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**
- **Example**: You can select the number of CPU cores or amount of RAM based on the workload the VM will handle.

---
