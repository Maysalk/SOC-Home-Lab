# Kali Linux Virtual Machine

## Overview

A Kali Linux virtual machine was deployed to simulate an attacker within the SOC Home Lab environment. Kali Linux provides a wide range of offensive security tools that will be used to generate realistic attack scenarios against the Windows endpoint.

The primary purpose of this machine is to emulate adversary behavior, allowing the Blue Team environment to detect, analyze, and respond to security events.

---

## Purpose

The Kali Linux virtual machine is used to:

* Simulate cyber attacks against the Windows endpoint.
* Perform reconnaissance and network scanning.
* Execute penetration testing tools.
* Generate security events for detection and analysis.
* Validate Wazuh detections and monitoring capabilities.
* Support Blue Team training and incident response exercises.

---

## Virtual Machine Specifications

| Component        | Value                           |
| ---------------- | ------------------------------- |
| Operating System | Kali Linux                      |
| Role             | Attacker Machine                |
| CPU              | *(4 vCPUs)*                      |
| Memory (RAM)     | *(7 GB)*                      |
| Disk Size        | *(50 GB)*                      |
| Network Adapter  | *(To be configured in Phase 2)* |

---

## Installation Summary

A Kali Linux virtual machine was created using VMware Workstation Pro and configured as the dedicated attacker system within the lab.

After installation, the operating system was updated and verified to function correctly. The virtual machine is ready to perform offensive security activities and interact with the isolated lab environment.

---

## Planned Activities

This virtual machine will be used throughout the project to perform:

* Network reconnaissance
* Port scanning
* Password attacks
* PowerShell abuse simulation
* Reverse shell execution
* Credential access techniques
* Privilege escalation testing
* Additional attack simulations

---

## Validation

The installation was verified by confirming the following:

* Kali Linux booted successfully.
* VMware recognized the virtual machine.
* The operating system was functioning normally.
* The terminal was operational.
* The virtual machine was ready for network configuration.

---

## Screenshots

### Kali Linux Desktop

<img width="1348" height="762" alt="image" src="https://github.com/user-attachments/assets/e0de45c3-9f3a-449d-8f12-1c4d265f1600" />


---

### Kali Linux Terminal

<img width="1347" height="760" alt="image" src="https://github.com/user-attachments/assets/649f4eae-7f8d-4f6a-84ef-8142287b0914" />

---


## Next Steps

The next phase will connect Kali Linux to the isolated lab network, enabling communication with both the Windows endpoint and the Wazuh server for attack simulation and security monitoring.

