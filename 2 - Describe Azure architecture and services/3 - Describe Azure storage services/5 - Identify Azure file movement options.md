# **Identify Azure File Movement Options**  
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
Azure provides tools for moving **individual files** or **small file groups**, complementing large-scale migration solutions like **Azure Migrate** and **Azure Data Box**.

Azure offers three key tools for moving files:  
- **AzCopy** (Command-line tool for file transfers)  
- **Azure Storage Explorer** (GUI-based storage management)  
- **Azure File Sync** (Syncs Windows file servers with Azure)  

---

## **AzCopy** 
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
- AzCopy is a **command-line tool** used for copying files or blobs to/from Azure storage.
- **AzCopy does NOT support two-way synchronization.** It only copies files in **one direction** based on the source and destination.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**  
- **File transfer** – Upload, download, copy, or sync files between storage accounts.  
- **Cross-cloud support** – Can move files between **Azure and other cloud providers**.  
- **One-way synchronization** – Files sync **only in one direction**, from source to destination.  
---

## **Azure Storage Explorer**
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
Azure Storage Explorer is a **graphical application** for managing files and blobs in an Azure Storage Account.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**  
- **Standalone app** – Works on **Windows, macOS, and Linux**.  
- **Uses AzCopy** – Runs AzCopy in the background for file transfers.  
- **Storage management** – Upload, download, and transfer files between storage accounts.  

#### ![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Additional but Important**  
- Ideal for users who prefer a **graphical interface** instead of command-line tools.  

---

## **Azure File Sync** 
#### ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**  
Azure File Sync allows **Windows file servers** to sync with **Azure Files**, maintaining performance and compatibility.

#### ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Key Terms and Definitions**  
- **File share centralization** – Syncs local Windows file servers with **Azure Files**.  
- **Bi-directional sync** – Automatically syncs changes **both ways**.  
- **Cloud tiering** – Frequently accessed files stay local; rarely used files stay in Azure.  

#### ![#f0e15d](https://placehold.co/15x15/f0e15d/f0e15d.png) **Supporting Details/Examples**  
- **Access via multiple protocols** – Supports **SMB, NFS, and FTPS**.  
- **Disaster recovery** – If a local server fails, a new one can sync from Azure.  
- **Multiple caches worldwide** – Maintain synced copies across multiple locations.  
