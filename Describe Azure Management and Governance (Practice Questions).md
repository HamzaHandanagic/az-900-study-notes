# AZ-900 — Describe Azure Management and Governance (Practice Questions)

## How to use this file
- Focus area: **Describe Azure management and governance**.
- Answer first, then verify with the answer key under each question.

---

## 1) Cost Management and SLAs

### Q1
Which pricing model lets you pay only for what you use?

- A. Fixed perpetual licensing  
- B. Consumption-based pricing  
- C. Capital-only procurement  
- D. Datacenter depreciation model

**Answer:** B

### Q2
What is a key purpose of Azure Reservations?

- A. Increase runtime memory of VMs  
- B. Reduce costs for predictable usage over time  
- C. Encrypt storage accounts  
- D. Replace RBAC roles

**Answer:** B

### Q3
Which tool helps estimate Azure costs before deployment?

- A. Azure Monitor  
- B. Pricing calculator  
- C. Azure Policy  
- D. Microsoft Purview

**Answer:** B

### Q4
Which tool helps compare on-premises TCO with Azure?

- A. Azure Advisor  
- B. Azure Migrate  
- C. TCO Calculator  
- D. Cost Management exports

**Answer:** C

### Q5
What does an SLA (Service Level Agreement) describe?

- A. Maximum VM size  
- B. Expected service uptime commitment  
- C. Subscription spending limit  
- D. Role assignment scope

**Answer:** B

### Q6
If two dependent services each have 99.9% SLA, combined availability is typically:

- A. Higher than 99.9%  
- B. Equal to 100%  
- C. Lower than 99.9%  
- D. Unchanged

**Answer:** C

---

## 2) Governance and Compliance

### Q7
What is Azure Policy used for?

- A. Authentication and sign-in  
- B. Enforcing standards and assessing compliance  
- C. Load balancing traffic  
- D. Container orchestration

**Answer:** B

### Q8
Which governance feature controls **who** can perform actions on resources?

- A. NSG  
- B. RBAC  
- C. Azure Firewall  
- D. Availability zones

**Answer:** B

### Q9
Which governance feature can prevent accidental deletion of resources?

- A. Tags  
- B. Resource Locks  
- C. Budgets  
- D. Service Health alerts

**Answer:** B

### Q10
What is true about resource locks?

- A. They apply only at resource level  
- B. They are inherited by child resources  
- C. They replace RBAC  
- D. They apply only to data plane actions

**Answer:** B

### Q11
Which lock type allows read and modify operations but prevents deletion?

- A. ReadOnly  
- B. CanNotDelete  
- C. DenyAssignment  
- D. NoDeleteAndRead

**Answer:** B

### Q12
What is the purpose of Azure tags?

- A. Enforce network routing  
- B. Provide metadata for organization, automation, and cost tracking  
- C. Replace subscriptions  
- D. Encrypt data at rest

**Answer:** B

### Q13
Are tags inherited automatically from resource group to all resources?

- A. Yes, always  
- B. No, not automatically  
- C. Only for VMs  
- D. Only for storage accounts

**Answer:** B

### Q14
At which scopes can Azure Policy be assigned?

- A. Only resource level  
- B. Only subscription level  
- C. Management group, subscription, resource group, and resource  
- D. Tenant root only

**Answer:** C

---

## 3) Resource Organization and Deployment

### Q15
What is the correct high-level governance hierarchy?

- A. Resource group > subscription > management group  
- B. Management group > subscription > resource group > resource  
- C. Subscription > management group > resource  
- D. Region > zone > VNet > resource group

**Answer:** B

### Q16
What is the primary benefit of management groups?

- A. Faster VM boot times  
- B. Organizing subscriptions and applying governance at scale  
- C. Lower latency in VNets  
- D. Automatic backup of all data

**Answer:** B

### Q17
What is true about Azure Resource Manager (ARM) templates?

- A. They are imperative scripts only  
- B. They define infrastructure declaratively in JSON  
- C. They are used only for monitoring dashboards  
- D. They cannot be reused

**Answer:** B

### Q18
Which statement best describes declarative deployment?

- A. It specifies exact step-by-step commands only  
- B. It defines the desired end state  
- C. It requires manual portal setup  
- D. It cannot be version controlled

**Answer:** B

### Q19
Which service can help recommend performance, security, and cost improvements?

- A. Azure Advisor  
- B. Azure DNS  
- C. Azure Bastion  
- D. Azure Arc-enabled servers

**Answer:** A

### Q20
Which deployment approach improves consistency and repeatability?

- A. Manual portal creation every time  
- B. Infrastructure as Code (IaC)  
- C. Local scripts without source control  
- D. One-time templates

**Answer:** B

---

## 4) Monitoring and Management Tools

### Q21
Which service collects telemetry and enables metrics, logs, and alerts?

- A. Azure Monitor  
- B. Azure Policy  
- C. Azure DevTest Labs  
- D. Azure Reservations

**Answer:** A

### Q22
Which service shows issues affecting Azure services in your region/subscription?

- A. Azure Service Health  
- B. Azure Arc  
- C. Azure Lighthouse  
- D. Azure Cost Management

**Answer:** A

### Q23
What does Azure Cost Management help with?

- A. VM patch scheduling  
- B. Cost analysis, budgeting, and spending control  
- C. DNS zone replication  
- D. Identity federation

**Answer:** B

### Q24
Which Azure tool is primarily for creating and managing resources through a web interface?

- A. Azure portal  
- B. Azure Stack Hub  
- C. Azure CLI extension host  
- D. Hyper-V Manager

**Answer:** A

### Q25
Which option is command-line based for Azure resource management?

- A. Azure CLI  
- B. Azure Policy Insights  
- C. Azure Databox  
- D. Azure Lighthouse only

**Answer:** A

---

## 5) Security and Governance Scenarios

### Q26
A company wants to ensure every resource has `CostCenter` tag. Which service is best?

- A. RBAC  
- B. Azure Policy  
- C. Azure Monitor  
- D. Service Health

**Answer:** B

### Q27
A team must ensure junior admins can view resources but cannot modify them. Which approach fits best?

- A. Assign Reader role via RBAC  
- B. Apply CanNotDelete lock  
- C. Increase budget alerts  
- D. Use availability zones

**Answer:** A

### Q28
A production resource must never be deleted accidentally but still requires updates. Which lock type should be used?

- A. ReadOnly  
- B. CanNotDelete  
- C. NoLock  
- D. Immutable

**Answer:** B

### Q29
You need to enforce allowed resource locations across many subscriptions. Best scope?

- A. Individual resource  
- B. Resource group in each subscription only  
- C. Management group  
- D. Region scope

**Answer:** C

### Q30
Which statement about budgets is correct?

- A. Budgets block all deployment actions automatically  
- B. Budgets track spend and can trigger alerts  
- C. Budgets replace invoices  
- D. Budgets configure NSG rules

**Answer:** B

---

## Quick True/False

### Q31
RBAC answers the question: “who can do what at which scope?”

**Answer:** True

### Q32
Azure Policy and RBAC are the same service.

**Answer:** False

### Q33
Resource locks can be applied at subscription or resource group scope and inherited.

**Answer:** True

### Q34
Infrastructure as Code helps with repeatable and auditable deployments.

**Answer:** True

---

## Mini Review Checklist
- [ ] I can explain SLAs, pricing calculator, TCO calculator, and reservations.
- [ ] I can differentiate RBAC, Policy, Locks, Tags, and Budgets.
- [ ] I can explain management groups, subscriptions, and resource groups.
- [ ] I can describe ARM templates and declarative IaC.
- [ ] I can identify Azure Monitor, Service Health, Advisor, and Cost Management usage.

