# AZ-900 Study Notes

## Pricing and cost

- **Consumption (pay-as-you-go)** — pay for what you use.
- **Azure Reservations** — pricing option to reduce cost and make future spend easier to predict.

---

## Physical layout: regions, zones, and datacenters

- **Regions**, **Availability Zones**, and **Datacenters** are **physical** concepts.
- **Not every region** supports **Availability Zones**. AZs are mainly relevant for **VMs**, **managed disks**, **load balancers**, and **databases**.
- **Zonal service** — deployed in **one** specific zone (e.g. a VM). For resilience, deploy **another instance in a different zone**.
- **Zone-redundant service** — **automatically** spans availability zones.

---

## Service models (IaaS vs PaaS)

**IaaS (you manage more of the stack)**

- Virtual networks
- Azure Files
- Azure VMs

**PaaS (platform manages more)**

- Azure SQL Database
- Azure App Service / Web Apps
- Azure Kubernetes Service (AKS)

---

## Governance: hierarchy and scopes

**Hierarchy (top → bottom)**

1. **Azure AD** (tenant)
2. **Root management group** (one per Azure AD)
3. **Management groups**
4. **Subscriptions**
5. **Resource groups**
6. **Resources**

These levels are **scopes** for applying governance.

- Governance **inherits downward**.
- **Management groups** — useful to **aggregate policy** (Azure Policy) across many subscriptions.

**Governance constructs**

| Construct | Typical question |
|-----------|------------------|
| **RBAC** | **Who** can do what |
| **Azure Policy** | **What** is allowed / required |
| **Budget** | **How much** spend |
| **Resource locks** | Prevent delete or changes |

**Where you can apply them:** management group, subscription, or resource group (and relevant scopes for individual resources where supported).

**Resource groups**

- **Not** a connectivity boundary — resources in **different** resource groups **can** connect.
- Resources in one group share a **common lifecycle** (organize/deploy/delete together).

---

## Why multiple subscriptions?

- Hit **subscription limits**
- **Different payment methods**
- **Isolation** (departments, projects, environments, etc.)

---

## ARM templates and declarative provisioning

- Azure resource definitions are **JSON**; **ARM** templates describe desired infrastructure.
- Prefer **declarative** (“**what** is my end state?”) over **imperative** (“**how** do I run each step?”).

---

## Resource locks

- Locks **inherit** down the hierarchy.
- **CanNotDelete** — can **modify**, cannot **delete**.
- **ReadOnly** — cannot **change** or **delete**.

---

## Tags

- Optional **key:value** **metadata** on resources.
- Tags are **not inherited** (unlike some governance settings).
- Can be **enforced** with **Azure Policy** (e.g. copy a required tag from the resource group if missing).

---

## Azure Blueprints

- A **blueprint** is made of **artifacts**.
- Supported artifact types include: **resource groups**, **ARM templates**, **policy assignments**, **role assignments**.

---

## Control plane vs data plane

- **Control plane** — create, update, delete **Azure resources** (goes through **ARM**). **RBAC**, **Policy**, etc. affect control plane.
- **Data plane** — work **inside** the service (e.g. insert a row, write a blob). Different permissions/APIs than resource management.

---

## Compute

**Virtual machines**

- Virtualizes **hardware** — CPU, memory, network; different **SKUs** and **CPU:memory** ratios.

**Azure Dedicated Host**

- **Dedicated physical host** — you do not share the host with other tenants; place VMs on **your** host of a chosen SKU.

**Containers**

- Virtualize **software** / app packaging — **image** in a **registry**, run as **container**.
- Containers start **much faster** than typical VMs.

**ACI (Azure Container Instances)**

- Good for **a few** containers, simpler scenarios.

**AKS (Azure Kubernetes Service)**

- When you need **orchestration**, **autoscaling**, richer platform — **nodes** visible to you; much of the control plane **managed**. Workloads run in **pods** (alternative: DIY Kubernetes on VMs).

**Azure App Service**

- **Web-focused**: APIs, web apps, mobile backends, etc.

**Serverless / event-driven (examples)**

- **Azure Functions**
- **Azure Logic Apps**
- **Event Grid** — route events to configured destinations

---

## Networking

**Azure Virtual Network (VNet)**

- Fundamental **private network** building block in Azure.

**NSG (Network Security Group)**

- Filters traffic **to/from** resources in a VNet.
- Rules: allow/deny **inbound** and **outbound**; specify **source**, **destination**, **port**, **protocol**.
- Can apply to several resource types associated with subnets/NICs (as per Azure design).

**VNet isolation and connectivity**

- Resources in **different VNets** do **not** talk by default → use **VNet peering** (or other connectivity patterns).
- VMs in **different subnets** of the **same VNet** **can** communicate by default (subject to NSGs and other rules).

**Hybrid**

- **On-premises** to Azure: e.g. **site-to-site VPN** (and other options exist for production).

---

## Storage

- **Storage account** — foundation; other storage patterns build on it; tied to a **region**.
- **Redundancy:** **LRS**, **ZRS**, **GRS**, **GZRS**.
- **ZRS** requires a region that **supports availability zones** (where applicable).

---

## Identity and hybrid directory

- **Azure AD** — cloud identity directory for Microsoft cloud (expand in official docs: users, groups, apps, devices, etc.).
- **Azure AD Connect** / **Azure AD Connect cloud sync** — sync from **on-premises AD** to **Azure AD**.

---

## Cloud adoption and support

- **Microsoft Cloud Adoption Framework (CAF)** — guidance for business and technology strategy on Azure.
- **Support plans (examples named):** Basic, Developer, Standard, Professional Direct, Premier.

---

## Quick review checklist

- [ ] Zonal vs zone-redundant
- [ ] Governance hierarchy and inheritance
- [ ] RBAC vs Policy vs Budget vs Locks
- [ ] ARM declarative vs imperative
- [ ] Control plane vs data plane
- [ ] IaaS vs PaaS examples
- [ ] VNet vs subnet default connectivity
- [ ] Storage redundancy letters (LRS/ZRS/GRS/GZRS)
