NOTES:

- Consumption based - Pay as you go
- Not all Azure Regions currently support availability zones.  Availability zones are primarily for VMs, managed disks, load balancers and databases.
- Regions, Availability Zones, Datacenters are physical concepts.
- Zonal service- created in specific availablity zone. To create resiliency I need to create another instance in different zone. Example: VM.
- Zone redundant - spans through availability zones automatically.
- Virtual networks, Azure Files, Azure VMs, - IaaS
- Azure SQL Databases, Azure App Service, Azure Web Apps service, Azure Kubernetes Service - PaaS
- Availability zones are primarily for VMs, managed disks, load balancers and databases.
- Azure Reservations are pricing option available to reduce costs and making predicting future spending easier.
<hr>

- Governance hierarchy: Azure AD instance > Root Management Group > Management Groups > Subscriptions > Resource Groups > Resources. Those are called scopes.
- Each Azure AD is given a single top-level management group called the root management group.
- Governance is inherited down.
- Governance constructs: RBAC (who), Policy (what), Budget (how much), Resource Locks.
- You can apply those constructs on Management Group level, Subscription Level or Resource Group Level.
- Resource groups are not boundary of connectivity. It is possible to connect resources in two separate resource groups. Resources in resource group have common lifecycle.

- We want to create things using ARM JSON templates. Everything in Azure is stored in JSON.  We want to provision things using ARM templates because they are declarative.
- How to do it => IMPERATIVE. What is my desired end state => DECLARATIVE.

- Resource lock is inherited down. CAN NOT DELETE - can change it but not delete. READONLY - you can not even change it.
- Optional metadatada that we can set = tag (esentially key:value). Tag is not inherited. It can be enforced using Azure Policy e.g: if resource is missing this tag go and copy it from resource group.
- A blueprint is composed of artifacts. Azure Blueprints currently supports the following resources as artifacts: Resource Groups, ARM template, Policy Assignment, Role Assignment.
- There is a Data Plane (create row at table, create file in storage etc.) and a Control Plane Azure (create, delete, modify resources etc.). All of these concepts like RBAC, Policies etc. are making impact at Control Plane because they are going through ARM.

- VM - virtualizaing the hardware. VM is a set of resources: CPU, Memory, Network. Different SKUs for VM. Ratio CPU:Memory.
- Azure Dedicated Host - If I don't want to share host. I buy a host of a particular SKU and then I can run VMs on that host.
- Containers - more about virtualizing the software. We have a registry with images. We take an image and run it in container instance. Container spins up almost instanlty which is not the case with VM.
- ACI (Azure Container Instances) - run just couple of containers. If i want richer set of capabilities, autoscale, full orchestraction => Kubernetes. I can set up Kubernetes myself on VM but there is AKS (Azure Kubernetes Service). What I see are the nodes, everything else is managed. My containers runs in pods.
- Azure App Service - web focused workload e.g.: API, WebApp, mobile app...
- Serverless - Azure Functions, Azure Logic App, Event Grid - pushing events to configured destination.
- Azure Virtual Network is a service that provides the fundamental building block for your private network in Azure. 
- NSG (Network Security Group) filter network traffic between Azure resources in an Azure virtual network. A network security group contains security rules that allow or deny inbound network traffic to, or outbound network traffic from, several types of Azure resources. For each rule, you can specify source and destination, port, and protocol.
- Storage Account – every other type of storage builds on top of this. Storage Account lives in specific region. There is redundancy related to it because regions expose idea of availability zones.
- Redundancy options – LRS, ZRS, GRS, GZRS. ZRS – not available if region does not support availability zones.
- Endpoints and services in one VNET can not communicate with endpoints and services in another VNET. That can be connected with VNET Peering. On Premises network can be connected to Azure via site-to-site VPN.
<hr>

- Microsoft Cloud Adoption Framework - guidance designed to help you create and implement the business and technology strategies in Azure.

- Azure ID Connect, Azure ID Connect Cloud Sync - sync from on-premises Active Directory to AAD
- Azure AD - 
- Azure support plans: Basic, Developer, Standard, Professional Direct, Premier.
