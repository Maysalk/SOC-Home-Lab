# Windows 10 Virtual Machine

## Overview

A Windows 10 virtual machine was deployed to simulate a corporate endpoint within the SOC Home Lab environment. This machine serves as the primary target for monitoring, log collection, attack simulation, and incident investigation.

Throughout the project, Windows 10 will generate security events that are collected by Wazuh and enriched with Sysmon telemetry to support detection engineering and Blue Team operations.

---

## Purpose

The Windows 10 virtual machine is used to:

* Simulate an enterprise workstation.
* Generate Windows Security Event Logs.
* Collect endpoint telemetry through Sysmon.
* Send security logs to the Wazuh SIEM.
* Act as the target during attack simulations.
* Support detection engineering and incident response exercises.

---

## Virtual Machine Specifications

| Component        | Value                           |
| ---------------- | ------------------------------- |
| Operating System | Windows 10                      |
| Role             | Victim Endpoint                 |
| CPU              | *(Update)*                      |
| Memory (RAM)     | *(Update)*                      |
| Disk Size        | *(Update)*                      |
| Network Adapter  | *(To be configured in Phase 2)* |

---

## Installation Summary

A Windows 10 virtual machine was created using VMware Workstation Pro. The operating system was installed successfully and configured for use within the SOC Home Lab environment.

Following the installation, the virtual machine was verified to boot correctly and was prepared for future network configuration, endpoint monitoring, and attack simulation.

---

## Planned Configuration

The following configurations will be completed during the next phases of the project:

* Configure virtual networking.
* Install the Wazuh Agent.
* Deploy Sysmon.
* Forward endpoint logs to the Wazuh server.
* Validate log collection.
* Perform attack simulations from the Kali Linux virtual machine.

---

## Validation

The installation was verified by confirming the following:

* Windows 10 booted successfully.
* VMware recognized the virtual machine.
* The operating system was functioning normally.
* The virtual machine was ready for additional configuration.

---

## Screenshots

### Windows 10 Desktop


---


## Next Steps

The next step is to configure networking between the Windows 10 endpoint, the Ubuntu Server hosting Wazuh, and the Kali Linux attacker machine. Once connectivity has been established, the Windows endpoint will be enrolled into Wazuh for centralized monitoring.

