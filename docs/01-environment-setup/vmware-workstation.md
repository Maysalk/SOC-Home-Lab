# VMware Workstation

## Overview

VMware Workstation Pro was selected as the virtualization platform for this project to create an isolated and controlled Security Operations Center (SOC) laboratory. The environment allows multiple operating systems to run simultaneously on a single host machine while maintaining separation between the host and guest systems.

Using virtualization provides a safe environment for deploying security tools, generating attack traffic, and performing defensive analysis without impacting the host operating system or external networks.

---

## Why VMware Workstation?

VMware Workstation Pro was chosen for the following reasons:

* Supports multiple virtual machines running simultaneously.
* Provides reliable virtual networking (NAT, Host-Only, and Bridged).
* Supports snapshots for restoring previous lab states.
* Provides stable performance for cybersecurity and penetration testing laboratories.
* Enables realistic enterprise-style lab environments.

---

## Virtual Machines

The following virtual machines were created for the lab environment

| Virtual Machine | Role        | Purpose                                                                         |
| --------------- | ----------- | ------------------------------------------------------------------------------- |
| Windows 10      | Victim      | Generates Windows security events and serves as the monitored endpoint         |
| Kali Linux      | Attacker    | Simulates offensive security activities and attack scenarios                 |
| Ubuntu Server   | SIEM Server | Hosts the Wazuh platform for log collection, monitoring, and security analysis |

---

## Host Machine Specifications

The virtual machines are hosted on a personal workstation.

| Component        | Specification |
| ---------------- | ------------- |
| Processor        | *(11th Gen Intel(R) Core(TM) i7-1165G7)*    |
| Memory (RAM)     | *(12.0 GB)*    |
| Storage          | *(477 GB)*    |
| Operating System | *(Windows11)*    |

---

## Lab Design

The virtual lab consists of three virtual machines that emulate a small enterprise environment.

* Windows 10 acts as the monitored endpoint.
* Kali Linux acts as the attacker machine.
* Ubuntu Server hosts the Wazuh SIEM platform.

This architecture enables realistic attack simulation, log collection, detection engineering, and incident response exercises within an isolated environment.

---

## Verification

The environment was validated by confirming the following:

* VMware Workstation launched successfully.
* All virtual machines booted without errors.
* Windows 10 loaded successfully.
* Kali Linux loaded successfully.
* Ubuntu Server loaded successfully.
* Wazuh was successfully deployed on Ubuntu Server.
* All virtual machines were ready for network configuration.

---

## Screenshots
### VMware Workstation
<img width="634" height="496" alt="image" src="https://github.com/user-attachments/assets/c665d100-2a35-4839-9fcd-971843d7d9fc" />

---

### Virtual Machines
<img width="537" height="320" alt="image" src="https://github.com/user-attachments/assets/91c33e5a-7847-423d-8a2b-33b8bb8e46cc" />

---

## Next Steps

The next phase of the project focuses on configuring virtual networking between the three machines using VMware networking modes, assigning static IP addresses, and validating connectivity before deploying endpoint monitoring.

