# Enterprise Infrastructure Deployment Implementation on Windows Server 2022

## Project Overview
This project demonstrates the deployment, configuration, and architectural design of a scalable corporate network infrastructure using **Windows Server 2022**. The primary objective was to establish a secure, centralized domain environment feauting dynamic network automation, resilient name resolution, and standardized security boundaries.
## Hardware & Virtulization Stack
* **Host Hardware:** Laptop Gigabyte G5 MF (Intel Core i5, 16GB RAM)
* **Hypervisor:** Oracle VM VirtualBox
* **Server OS:** Windows Server 2022 Datacenter (Domain Controller)
* **Client OS:** Windows 10 Pro (workstation Node)
## Core Infrastructure Roles Imlemented
### 1. Active Directory Domain Services (AD DS)
* **Domain Infrastructure:** Deploed a new forest root domain 'home.local'.
* **Organizational Units (OU):** Designed a clean hierarchical OU layout reflecting logical corporate structures ('IT_Departament','Sales','Workstations').
* **User Management:** Created and managed secure domain employee indentities (including user groups for granular access delegation).
### 2. Core Network Services Configuration
* **DHCP Server:** Automated network address allocation by defining dedicated scopes, configuring IP ranges, and managing lease durations.
* **DNS Server:** Configured forward and reverse lookup zones to guarantee reliable intranet name resolution and active Active Directory integration.
### 3. Group Policy Management (GPO)
* **Security Hardening:** Enforced strict enterprise policies including restricting unauthorized user access to critical system lools.
* **Targeted Application:** Linked customized GPO rules to specific OUs to standardize desktop environments and prevent policy drift on end-user workstations.
## Project Evidence & Validation
All configurations have been successfully tested and validated on client machines using standard network utilities ('ipconfig /all', policy propagation checks).
*Network architecture screens, DHCP scopes, Active Directory structures, and GPO policies are available as verified asset uploades inside this repository.*
