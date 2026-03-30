# AZ-900 — 50 Practice Questions

> These are realistic AZ-900-style practice questions based on commonly covered exam topics.

## Part 1: Questions (3 options each)

### Q1
A startup wants to avoid buying servers upfront and pay only for resources used. Which cloud benefit is this?
- A. Capital expenditure (CapEx)
- B. Consumption-based pricing (OpEx)
- C. Dedicated hosting only

### Q2
A company keeps core banking systems on-premises but runs its customer portal in Azure. Which model is this?
- A. Public cloud
- B. Private cloud
- C. Hybrid cloud

### Q3
An app must handle sudden traffic spikes during sales events without downtime. Which cloud characteristic helps most?
- A. Elasticity
- B. Manual scaling only
- C. Fixed capacity

### Q4
Your team wants Microsoft to manage OS patching while developers focus on code. Which service model fits best?
- A. IaaS
- B. PaaS
- C. Private cloud

### Q5
A business uses Microsoft 365 for email and collaboration. This is an example of:
- A. IaaS
- B. PaaS
- C. SaaS

### Q6
Which cloud model usually gives the customer the most control over operating systems?
- A. SaaS
- B. PaaS
- C. IaaS

### Q7
A company needs strict control of physical infrastructure due to legal requirements. Which cloud type is best?
- A. Public cloud
- B. Private cloud
- C. Multi-cloud only

### Q8
Which concept means services remain available even when a component fails?
- A. High availability
- B. CapEx
- C. Data gravity

### Q9
Which term describes increasing or decreasing resources based on workload demand?
- A. Governance
- B. Scalability
- C. Latency

### Q10
Who is always responsible for identity and access management configuration in cloud solutions?
- A. Customer
- B. Cloud provider only
- C. Hardware vendor

### Q11
Under the shared responsibility model, in IaaS who typically patches the guest OS?
- A. Cloud provider
- B. Customer
- C. Microsoft support plan

### Q12
A company wants predictable discounts for steady VM usage over 1–3 years. Which option helps?
- A. Azure Reservations
- B. Spot VMs only
- C. Free tier

### Q13
Which cloud benefit improves by deploying an application across multiple regions?
- A. Reliability
- B. Local power usage
- C. CPU clock speed

### Q14
A team wants to launch a test environment in minutes and remove it after one day. Which cloud benefit is highlighted?
- A. Agility
- B. Physical isolation only
- C. Procurement delay

### Q15
Which statement is true about OpEx in cloud?
- A. Large upfront payment for hardware
- B. Ongoing pay-for-use spending
- C. No billing visibility

### Q16
Azure regions are:
- A. Logical tags only
- B. Sets of datacenters in a geographic area
- C. Resource groups with billing limits

### Q17
Availability Zones provide:
- A. Physical fault isolation within a region
- B. Subscription hierarchy
- C. Identity federation

### Q18
A team wants to organize resources by lifecycle and ownership. What should they use?
- A. Region pairs
- B. Resource groups
- C. Availability zones

### Q19
What is directly above resource groups in hierarchy?
- A. Subscription
- B. Region
- C. Management group

### Q20
An organization needs to apply governance across multiple subscriptions. What should they use?
- A. NSG
- B. Management groups
- C. Azure Bastion

### Q21
You need full admin access to a Windows server in Azure. Which service should you choose?
- A. Azure App Service
- B. Azure Virtual Machines
- C. Azure Functions

### Q22
Which service is best for running containerized apps with advanced orchestration and autoscaling?
- A. Azure Container Instances
- B. Azure Kubernetes Service (AKS)
- C. Azure Batch Explorer

### Q23
For simple short-lived container jobs without managing orchestration, use:
- A. AKS
- B. ACI
- C. Virtual Machine Scale Sets only

### Q24
Which service is best for hosting a web API without managing servers and OS patches?
- A. Azure App Service
- B. Azure Dedicated Host
- C. Azure VMware Solution

### Q25
Which Azure service is event-driven serverless compute?
- A. Azure Functions
- B. Azure Firewall
- C. Azure Load Balancer

### Q26
Which Azure service creates a private network boundary for resources?
- A. Azure DNS
- B. Azure Virtual Network
- C. Azure Policy

### Q27
What controls inbound and outbound traffic with rule-based filtering at subnet or NIC level?
- A. Network Security Group
- B. Resource lock
- C. Azure Reservations

### Q28
By default, two different VNets cannot communicate unless you configure:
- A. VNet peering or VPN/ExpressRoute
- B. Storage replication
- C. Resource tags

### Q29
A company needs private dedicated connectivity from on-premises to Azure, avoiding public internet. Choose:
- A. Site-to-site VPN only
- B. ExpressRoute
- C. Azure Front Door

### Q30
Which service distributes incoming traffic across multiple servers?
- A. Azure Load Balancer
- B. Azure Backup
- C. Azure Monitor

### Q31
Which Azure storage type is best for unstructured objects like images, videos, backups?
- A. Blob storage
- B. Queue storage
- C. Table storage

### Q32
Which storage option is used for persistent VM block storage?
- A. Azure Files
- B. Managed Disks
- C. Azure Queue

### Q33
Which redundancy option replicates data across availability zones in the same region?
- A. LRS
- B. ZRS
- C. GRS

### Q34
Which service provides managed relational database capabilities?
- A. Azure SQL Database
- B. Azure Blob Storage
- C. Azure Event Grid

### Q35
A globally distributed NoSQL database with multi-model APIs in Azure is:
- A. Azure SQL Managed Instance
- B. Azure Cosmos DB
- C. Azure Files

### Q36
What is Microsoft Entra ID primarily for?
- A. Identity and access management
- B. Block storage
- C. Web traffic routing

### Q37
Where should you store secrets, certificates, and encryption keys securely?
- A. Azure Key Vault
- B. Azure App Service settings only
- C. Azure Advisor

### Q38
Which service provides centralized telemetry (metrics, logs, alerts)?
- A. Azure Monitor
- B. Azure Reservations
- C. Azure Marketplace

### Q39
Which service shows outages and advisories impacting Azure services in your subscriptions/regions?
- A. Azure Service Health
- B. Azure Cost Management
- C. Azure DevOps

### Q40
Which tool gives recommendations for cost, reliability, performance, and security improvements?
- A. Azure Advisor
- B. Azure Policy
- C. Azure Arc

### Q41
Which feature controls **who** can do **what** on Azure resources?
- A. RBAC
- B. NSG
- C. Availability zones

### Q42
Which feature enforces standards such as allowed locations or required tags?
- A. Azure Policy
- B. Azure Load Balancer
- C. Azure DNS

### Q43
A production storage account must not be deleted accidentally but should remain editable. Use:
- A. ReadOnly lock
- B. CanNotDelete lock
- C. No lock

### Q44
What are Azure tags mainly used for?
- A. Packet filtering
- B. Metadata for organization, automation, and cost reporting
- C. Encrypting data in transit

### Q45
Which statement about tags is correct?
- A. Tags are always inherited automatically
- B. Tags can be enforced using Azure Policy
- C. Tags replace RBAC

### Q46
Which deployment approach defines desired infrastructure state in JSON templates?
- A. ARM templates
- B. Manual portal-only deployment
- C. Firmware scripting

### Q47
A finance team wants alerts when spending reaches a threshold. What should be configured?
- A. Cost Management budget
- B. NSG rule
- C. Availability set

### Q48
Which calculator estimates Azure service costs before deployment?
- A. Pricing calculator
- B. SLA calculator
- C. Advisor scorecard

### Q49
Which calculator compares on-premises costs to Azure migration costs?
- A. TCO calculator
- B. Pricing calculator
- C. Cost anomaly detector

### Q50
Which statement about SLAs is correct?
- A. Higher SLA percentage generally means less allowed downtime
- B. SLA defines RBAC permissions
- C. SLA removes need for architecture resiliency

---

## Part 2: Answers + Short Description

| Q# | Correct Answer | Short Description |
|---|---|---|
| 1 | B | Pay-as-you-go is an OpEx consumption model. |
| 2 | C | Hybrid cloud combines on-premises and public cloud. |
| 3 | A | Elasticity automatically matches resources to demand spikes. |
| 4 | B | PaaS offloads OS/runtime management to provider. |
| 5 | C | Microsoft 365 is SaaS: ready-to-use application service. |
| 6 | C | IaaS gives most control over VMs and OS. |
| 7 | B | Private cloud supports strict control/compliance needs. |
| 8 | A | High availability keeps services running during failures. |
| 9 | B | Scalability is the ability to scale resources up/down. |
| 10 | A | Customers manage identities and access settings. |
| 11 | B | In IaaS, guest OS patching is customer responsibility. |
| 12 | A | Reservations reduce cost for steady long-term usage. |
| 13 | A | Multi-region deployments improve resilience/reliability. |
| 14 | A | Fast provisioning/deprovisioning shows cloud agility. |
| 15 | B | OpEx is recurring usage-based spending. |
| 16 | B | A region is one geographic area with datacenters. |
| 17 | A | Availability zones isolate failures physically in-region. |
| 18 | B | Resource groups organize resources by lifecycle/ownership. |
| 19 | A | Resource groups are contained inside subscriptions. |
| 20 | B | Management groups apply governance across subscriptions. |
| 21 | B | Azure VMs provide full server admin control. |
| 22 | B | AKS is managed Kubernetes for orchestration/autoscale. |
| 23 | B | ACI is lightweight for simple container workloads. |
| 24 | A | App Service is PaaS for web apps/APIs. |
| 25 | A | Functions run event-driven serverless code. |
| 26 | B | VNet is Azure’s private networking foundation. |
| 27 | A | NSG filters traffic with allow/deny rules. |
| 28 | A | Separate VNets require peering or private connection. |
| 29 | B | ExpressRoute is dedicated private connectivity. |
| 30 | A | Load Balancer distributes traffic across instances. |
| 31 | A | Blob storage is optimized for unstructured object data. |
| 32 | B | Managed Disks provide persistent block storage for VMs. |
| 33 | B | ZRS replicates across availability zones in-region. |
| 34 | A | Azure SQL Database is managed relational DB PaaS. |
| 35 | B | Cosmos DB is globally distributed NoSQL database. |
| 36 | A | Entra ID handles authentication and identity management. |
| 37 | A | Key Vault securely stores secrets/keys/certificates. |
| 38 | A | Azure Monitor centralizes logs, metrics, and alerts. |
| 39 | A | Service Health reports Azure incidents and advisories. |
| 40 | A | Advisor gives best-practice recommendations. |
| 41 | A | RBAC defines access permissions by role and scope. |
| 42 | A | Azure Policy enforces and audits resource compliance. |
| 43 | B | CanNotDelete blocks deletion but allows modifications. |
| 44 | B | Tags add metadata for organization and reporting. |
| 45 | B | Policy can enforce required tags automatically. |
| 46 | A | ARM templates are declarative IaC in JSON. |
| 47 | A | Budgets track spend and trigger alerts. |
| 48 | A | Pricing calculator estimates expected Azure costs. |
| 49 | A | TCO calculator compares current and cloud costs. |
| 50 | A | Higher SLA means less acceptable downtime window. |
