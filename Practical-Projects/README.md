# Practical Projects — Evidence Index

**M9: Cloud Operations and Management | MSc Cybersecurity | University of Essex Online | October 2026**

## Purpose

This index records seven hands-on cloud and security project reports developed during the module. It highlights implementation, testing, troubleshooting, measured outcomes and limitations. Separate technical repositories provide project-specific implementation evidence where linked below.

> **Access and attribution:** The seven original Word reports are retained unchanged in the private university OneDrive workspace. This public index summarises the work; it does not publish the full reports, embedded screenshots, keys, tenant/subscription identifiers, third-party materials or credentials. Linked technical repositories should be checked independently before assessment submission.

## Project overview

| Unit / context | Practical project | Principal demonstrated outcome |
|:--|:--|:--|
| 04 | **Azure Bash Automation** | Azure CLI/Bash provisioned a resource group, VNet, NSG, Ubuntu VM and Nginx; public HTTP reachability was verified after quota and region troubleshooting. |
| 07 | **Docker Container Security Audit** | Docker web workload scanned with OpenVAS/Greenbone: 14 scan results and two Low information-disclosure findings selected under the applied filter. |
| Cross-unit | **Azure AKS Container Security Hardening** | AKS, Terraform, Ansible and Trivy used to harden a container workload; Kubernetes configuration failures decreased from 11 to 2 Low, and NetworkPolicy enforcement was tested. |
| 08 | **Azure Disaster Recovery with Restic** | Bicep rebuilt an Azure VM; an encrypted Restic snapshot was restored from Azure Blob using managed identity and RBAC, and restored data/repository were checked. |
| 09 | **Secure MySQL Migration to Azure** | Oracle MySQL 8.4 in Docker migrated to private Azure Database for MySQL Flexible Server using offline DMS, S2S IPsec VPN and TLS; both tables and records were verified. |
| 10 | **OpenFaaS Serverless Migration and CI/CD** | Python function deployed to local Docker Desktop Kubernetes via OpenFaaS; GitHub Actions automated pytest, build and GHCR image publication. |
| 11 | **TensorFlow Image Recognition on Azure** | CIFAR-10 CNN (66.71% test accuracy) served via FastAPI, Docker and Azure Container Apps; HTTPS ship-image inference succeeded (0.9247 confidence), with scale-to-zero/from-zero observed. |

## Evidence records

### 1. Azure Bash Automation — Unit 04

- **Original private report:** `Unit04_Azure_Bash_Automation_Report_GitHub_SAFE.docx`
- **Evidence of work:** Azure CLI/Bash provisioned a resource group, VNet, NSG, Ubuntu VM and Nginx; public HTTP reachability was verified after quota and region troubleshooting.
- **Scope / limitation:** Controlled HTTP-only proof of concept; imperative scripting, not production-ready declarative IaC.
- **Related project repository:** [Open technical project](https://github.com/pg25304/Azure-Bash-Automation-PoC)

### 2. Docker Container Security Audit — Unit 07

- **Original private report:** `Docker_Container_Security_Audit_Report.docx`
- **Evidence of work:** Docker web workload scanned with OpenVAS/Greenbone: 14 scan results and two Low information-disclosure findings selected under the applied filter.
- **Scope / limitation:** Network-based, unauthenticated scan; not a complete image/runtime assessment.
- **Related project repository:** [Open technical project](https://github.com/pg25304/Docker-Container-Security-Audit)

### 3. Azure AKS Container Security Hardening — Cross-unit

- **Original private report:** `Azure_AKS_Container_Security_Hardening_Report.docx`
- **Evidence of work:** AKS, Terraform, Ansible and Trivy used to harden a container workload; Kubernetes configuration failures decreased from 11 to 2 Low, and NetworkPolicy enforcement was tested.
- **Scope / limitation:** HTTP without TLS remained; not a full production security assessment or ISO certification.
- **Related project repository:** No individual link supplied in this index; report retained privately.

### 4. Azure Disaster Recovery with Restic — Unit 08

- **Original private report:** `01_GITHUB_COMPLETE_PROJECT_Azure_Disaster_Recovery_with_Restic.docx`
- **Evidence of work:** Bicep rebuilt an Azure VM; an encrypted Restic snapshot was restored from Azure Blob using managed identity and RBAC, and restored data/repository were checked.
- **Scope / limitation:** RTO/RPO targets were defined, but exact end-to-end measurements were not captured; regional failover was not tested.
- **Related project repository:** [Open technical project](https://github.com/pg25304/Azure-Disaster-Recovery-with-Restic)

### 5. Secure MySQL Migration to Azure — Unit 09

- **Original private report:** `GitHub_Azure_MySQL_Migration_FINAL_v2.docx`
- **Evidence of work:** Oracle MySQL 8.4 in Docker migrated to private Azure Database for MySQL Flexible Server using offline DMS, S2S IPsec VPN and TLS; both tables and records were verified.
- **Scope / limitation:** Final migrated source was Oracle MySQL, not the earlier MariaDB test; offline migration, not near-zero downtime.
- **Related project repository:** [Open technical project](https://github.com/pg25304/azure-mysql-secure-migration)

### 6. OpenFaaS Serverless Migration and CI/CD — Unit 10

- **Original private report:** `OpenFaaS_Technical_Report_Revised (2)(1).docx`
- **Evidence of work:** Python function deployed to local Docker Desktop Kubernetes via OpenFaaS; GitHub Actions automated pytest, build and GHCR image publication.
- **Scope / limitation:** Local deployment remained manual; monitoring worked but autoscaling was not demonstrated.
- **Related project repository:** [Open technical project](https://github.com/pg25304/openfaas-serverless-migration)

### 7. TensorFlow Image Recognition on Azure — Unit 11

- **Original private report:** `TensorFlow_Image_Recognition_GitHub_Report_Upgraded.docx`
- **Evidence of work:** CIFAR-10 CNN (66.71% test accuracy) served via FastAPI, Docker and Azure Container Apps; HTTPS ship-image inference succeeded (0.9247 confidence), with scale-to-zero/from-zero observed.
- **Scope / limitation:** Educational classifier and one sample prediction, not production model validation.
- **Related project repository:** [Open technical project](https://github.com/pg25304/tensorflow-image-recognition-azure)

## How the evidence is used

- **Public GitHub:** This index provides an overview and links to separate technical repositories where recorded. It does not duplicate the seven original reports.
- **Private university OneDrive:** The seven source Word reports, including their embedded figures and detailed troubleshooting, remain unchanged in `Assessments/e-Portfolio/GitHub-Collection/Practical Projects/`.
- **Tutor review:** A restricted, view-only link to the private evidence collection can be provided as part of the assessed e-Portfolio when submitted, subject to the university requirements.
- **Publication safeguards:** Before making any individual full report or screenshot public, review licences/ownership, screenshots, account identifiers, IP addresses, secrets, private keys and temporary lab credentials. The recorded public repository links should be opened and checked before final publication.

**Scope note:** These are seven selected project reports, not a claim that every unit required or produced a practical project. Completed tests, targets and future intentions are distinguished above.
