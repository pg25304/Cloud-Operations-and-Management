# Unit 6 Group Project — Evidence Index

**M9: Cloud Operations and Management | MSc Cybersecurity | University of Essex Online | October 2026**

## Purpose and attribution

This index identifies four records connected with the **Group C Cloud Infrastructure and Framework Report**. It distinguishes an individual draft design and hands-on Azure Bicep proof of concept (PoC) from the **collaborative group report**. The index is a navigation and evidence summary, not a claim that one student authored all group work.

> **Access and attribution:** The original Word documents, diagrams and Azure screenshots are retained in the private university OneDrive workspace. They are not published through this index. The group report is collaborative work; permission and privacy checks are needed before any full report or group material is published openly. Read-only access can be provided to the tutor as appropriate for assessment.

## Evidence register

| Record | Contribution and evidence | Status |
|:--|:--|:--|
| `Unit_6_Infrastructure_Design_Payman_Draft.docx` | Individual **draft architecture** prepared for team discussion: ARM/Bicep, networking, IaaS/PaaS, storage, security, monitoring and recovery options. | Draft proposal; **not a deployed system** |
| `azure-infrastructure-poc.bicep` | Declarative Azure infrastructure code defining a Virtual Network (`vnet-cloud-poc`) and application subnet (`subnet-app`). | PoC implementation source |
| `Azure_Bicep_PoC_Implementation_Evidence.docx` | **12 screenshot figures** across eight pages recording Cloud Shell preparation, region-policy troubleshooting, successful validation and Virtual Network deployment. | Completed small-scale PoC evidence |
| `Group_C_Unit_6_Cloud_Infrastructure_and_Framework_Report.docx` | Collaborative Group C report covering ARM/Bicep, cloud service and deployment models, proposed architecture, a real-world example, and selected PoC evidence in its appendix. | **Group-authored** report; private original |

## What the Azure proof of concept actually demonstrated

- **Deployed:** The Bicep source specifies `vnet-cloud-poc` with the address space `10.0.0.0/16` and `subnet-app` with the prefix `10.0.1.0/24`. Its deployment location is parameterised from the resource-group location.
- **Troubleshooting:** An initial validation encountered a regional restriction under the Azure for Students policy. The permitted regions were checked and the deployment was validated again in an approved location.
- **Outcome:** The implementation evidence records successful Bicep validation, a **Succeeded** provisioning result and the Virtual Network appearing in Azure Resource Manager.
- **Not claimed as deployed:** The fuller conceptual architecture—web-server VMs, load balancer, App Service, storage, NSGs, Azure Monitor, WAF and multi-region disaster recovery—was discussed and illustrated as a proposed design. The small PoC evidence does not establish that these additional components were provisioned.

## Learning and relationship to the assignment

The evidence traces a practical sequence: **individual design proposal → Bicep implementation → deployment-policy troubleshooting → validated Virtual Network deployment → evidence incorporated into the group report**. It demonstrates repeatable Infrastructure as Code at a deliberately limited scale, and the difference between an architecture proposal and a working cloud deployment.

## How the evidence is organised

- **Private originals:** `Assessments/e-Portfolio/GitHub-Collection/Group Project Evidence/` in the university OneDrive workspace. These filenames are references to private study records, **not public download links**.
- **Public GitHub:** This `Group-Project-Evidence/README.md` index may be published as a navigation record. The four original files are **not** included automatically.
- **Tutor review:** The student can provide a separate restricted, view-only OneDrive link to the originals when appropriate for the assessed e-Portfolio.
- **If the Bicep code is published later:** Review the file and repository for credentials, subscription identifiers and other sensitive data before uploading. Keep any collaborative report or third-party material private unless publication is authorised.

**Scope note:** This index covers the four records supplied for the Unit 6 group project. It is not a comprehensive activity log for every module unit.
