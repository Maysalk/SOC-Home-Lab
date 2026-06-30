# Phase 1: Environment Setup

## Overview

This phase focuses on building the foundation of the SOC Home Lab by preparing the virtualization environment and deploying the systems required for security monitoring and attack simulation.

The lab consists of three virtual machines hosted on VMware Workstation Pro:

* **Windows 10** – Monitored endpoint
* **Kali Linux** – Attacker machine
* **Ubuntu Server** – Wazuh SIEM server

At the end of this phase, all virtual machines were successfully installed, verified, and prepared for network configuration.

---

## Objectives

* Install and configure VMware Workstation Pro.
* Deploy the required virtual machines.
* Prepare the Ubuntu Server for Wazuh.
* Deploy the Wazuh platform.
* Verify that all systems are operational.
* Prepare the environment for networking and endpoint monitoring.

---

## Environment

| Virtual Machine | Role              | Status      |
| --------------- | ----------------- | ----------- |
| Windows 10      | Victim Endpoint   | ✅ Completed |
| Kali Linux      | Attacker Machine  | ✅ Completed |
| Ubuntu Server   | Wazuh SIEM Server | ✅ Completed |

---

## Documentation

| Document                   | Description                                        |
| -------------------------- | -------------------------------------------------- |
| `vmware-workstation.md`    | VMware installation and virtualization environment |
| `windows-10-install.md`    | Windows 10 virtual machine deployment              |
| `kali-linux-install.md`    | Kali Linux virtual machine deployment              |
| `ubuntu-server-install.md` | Ubuntu Server deployment                           |
| `wazuh-deployment.md`      | Wazuh installation and verification                |

---

## Deliverables

During this phase, the following tasks were completed:

* VMware Workstation environment prepared.
* Windows 10 virtual machine deployed.
* Kali Linux virtual machine deployed.
* Ubuntu Server virtual machine deployed.
* Wazuh successfully installed and verified.
* Lab environment validated and ready for networking.

---

## Validation Checklist

* ✅ VMware Workstation installed
* ✅ Windows 10 operational
* ✅ Kali Linux operational
* ✅ Ubuntu Server operational
* ✅ Wazuh deployed
* ✅ Dashboard accessible
* ✅ SSH management verified

---

## Next Phase

The next phase focuses on configuring networking between all virtual machines.

Key activities include:

* Configuring VMware virtual networks
* Assigning static IP addresses
* Validating connectivity between systems
* Preparing the environment for endpoint enrollment

➡️ Continue to **Phase 2 – Network Configuration**
