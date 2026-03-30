# AZ-900 — Describe Azure Architecture and Services (Practice Questions)

## How to use this file
- Focus area: **Describe Azure architecture and services**.
- Attempt each question before checking the answer.

---

## 1) Core Architectural Components

### Q1
What is an Azure **region**?

- A. A pricing tier for compute resources  
- B. A set of datacenters deployed within a specific geographic area  
- C. A virtual network boundary  
- D. A subscription billing unit

**Answer:** B

### Q2
What is an **availability zone** in Azure?

- A. A logical grouping of subscriptions  
- B. A physically separate datacenter location within an Azure region  
- C. A network security rule collection  
- D. A VM scale set policy

**Answer:** B

### Q3
Which statement about availability zones is correct?

- A. Every Azure region supports them  
- B. They are logical only, not physical  
- C. They provide fault isolation within a region  
- D. They can only be used for storage accounts

**Answer:** C

### Q4
What is an Azure **resource group** primarily used for?

- A. Network routing between regions  
- B. Organizing related resources for lifecycle management  
- C. Assigning global billing currency  
- D. Replacing subscriptions

**Answer:** B

### Q5
Which scope is directly above resource groups in Azure hierarchy?

- A. Management group  
- B. Region  
- C. Subscription  
- D. Availability zone

**Answer:** C

### Q6
What is the purpose of Azure **management groups**?

- A. Provide VM backup  
- B. Organize subscriptions and apply governance at scale  
- C. Replace Microsoft Entra ID  
- D. Host web applications

**Answer:** B

---

## 2) Compute Services

### Q7
Which service provides full control of OS and VM configuration?

- A. Azure App Service  
- B. Azure Functions  
- C. Azure Virtual Machines  
- D. Azure Logic Apps

**Answer:** C

### Q8
Which Azure service is best for container orchestration?

- A. Azure Container Instances (ACI)  
- B. Azure Kubernetes Service (AKS)  
- C. Azure Virtual Desktop  
- D. Azure Batch

**Answer:** B

### Q9
Which statement best describes Azure Container Instances (ACI)?

- A. Best for full Kubernetes orchestration  
- B. Best for simple container workloads without managing servers  
- C. Requires VMSS setup first  
- D. Runs only Windows containers

**Answer:** B

### Q10
Which service is a PaaS offering for hosting web apps and APIs?

- A. Azure Virtual Machines  
- B. Azure App Service  
- C. Azure Dedicated Host  
- D. Azure Bastion

**Answer:** B

### Q11
Which Azure service is event-driven, serverless compute?

- A. Azure Functions  
- B. Azure Load Balancer  
- C. Azure Firewall  
- D. Azure NetApp Files

**Answer:** A

### Q12
What is Azure Virtual Desktop used for?

- A. Hosting container images  
- B. Delivering virtualized desktop and app experiences  
- C. Monitoring on-premises servers only  
- D. Replacing Microsoft Entra ID

**Answer:** B

---

## 3) Networking Services

### Q13
What is an Azure Virtual Network (VNet)?

- A. A global DNS service  
- B. A private network in Azure  
- C. A container runtime  
- D. A storage redundancy option

**Answer:** B

### Q14
Which Azure service filters traffic using allow/deny rules by source, destination, port, and protocol?

- A. Azure DDoS Protection  
- B. Network Security Group (NSG)  
- C. Azure Front Door  
- D. Traffic Manager

**Answer:** B

### Q15
By default, can two VNets communicate without additional configuration?

- A. Yes, always  
- B. No, not by default  
- C. Only in the same region  
- D. Only with Azure Firewall

**Answer:** B

### Q16
What connects two Azure VNets privately?

- A. ExpressRoute  
- B. VNet Peering  
- C. Azure CDN  
- D. NSG flow logs

**Answer:** B

### Q17
Which service provides private dedicated connectivity from on-premises to Azure (not over public internet)?

- A. Site-to-site VPN  
- B. Azure ExpressRoute  
- C. Azure NAT Gateway  
- D. Azure DNS

**Answer:** B

### Q18
What does Azure Load Balancer do?

- A. Stores backup files  
- B. Distributes traffic across resources  
- C. Manages RBAC assignments  
- D. Encrypts data at rest

**Answer:** B

---

## 4) Storage Services

### Q19
What is the foundational Azure storage resource?

- A. Recovery Services Vault  
- B. Storage account  
- C. SQL managed instance  
- D. Azure Files endpoint

**Answer:** B

### Q20
Which storage type is best for unstructured data such as images and log files?

- A. Blob storage  
- B. Queue storage  
- C. Table storage  
- D. Disk storage

**Answer:** A

### Q21
Which storage service provides SMB/NFS file shares?

- A. Azure Disks  
- B. Azure Files  
- C. Blob storage  
- D. Data Lake Analytics

**Answer:** B

### Q22
Which redundancy option replicates data across availability zones in a region?

- A. LRS  
- B. ZRS  
- C. GRS  
- D. RA-GRS only

**Answer:** B

### Q23
Which storage option is used as persistent block storage for Azure VMs?

- A. Azure Queue storage  
- B. Azure Blob storage  
- C. Azure Managed Disks  
- D. Azure Archive tier only

**Answer:** C

---

## 5) Database and Analytics Services

### Q24
Which Azure database service is a fully managed relational database platform?

- A. Azure Cosmos DB only  
- B. Azure SQL Database  
- C. Azure Blob storage  
- D. Azure Event Hubs

**Answer:** B

### Q25
Which Azure database is globally distributed and supports multiple APIs?

- A. Azure SQL Database  
- B. Azure Database for PostgreSQL  
- C. Azure Cosmos DB  
- D. Azure Table storage

**Answer:** C

### Q26
What is Azure Synapse Analytics primarily used for?

- A. DNS management  
- B. Data warehousing and big data analytics  
- C. VM patching  
- D. Identity federation

**Answer:** B

---

## 6) Identity, Access, and Security Services

### Q27
What is Microsoft Entra ID (Azure AD) primarily used for?

- A. Hosting VMs  
- B. Identity and access management  
- C. Backing up disks  
- D. Managing virtual networks

**Answer:** B

### Q28
What does Azure Key Vault store?

- A. VM images only  
- B. Secrets, keys, and certificates  
- C. NSG rules  
- D. Azure Policy assignments

**Answer:** B

### Q29
Which service helps protect Azure resources from distributed denial-of-service attacks?

- A. Azure DDoS Protection  
- B. Azure Advisor  
- C. Azure Arc  
- D. Azure Bastion

**Answer:** A

### Q30
Which service provides security posture recommendations across Azure resources?

- A. Azure Monitor  
- B. Microsoft Defender for Cloud  
- C. Azure Service Bus  
- D. Azure Policy only

**Answer:** B

---

## Quick True/False

### Q31
A subscription can contain multiple resource groups.

**Answer:** True

### Q32
Azure regions and availability zones are both physical concepts.

**Answer:** True

### Q33
Azure App Service is typically classified as IaaS.

**Answer:** False

### Q34
AKS reduces the operational overhead of managing Kubernetes control plane components.

**Answer:** True

---

## Mini Review Checklist
- [ ] I can explain regions, availability zones, subscriptions, and resource groups.
- [ ] I can choose between VMs, App Service, Functions, ACI, and AKS.
- [ ] I can explain core networking services (VNet, NSG, peering, VPN/ExpressRoute, load balancing).
- [ ] I can distinguish Azure storage options and redundancy models.
- [ ] I can identify core Azure database, identity, and security services.

