# Wazuh Deployment

## Overview

Wazuh was deployed as the central Security Information and Event Management (SIEM) platform for the SOC Home Lab. It provides centralized log collection, endpoint monitoring, security event correlation, threat detection, and incident investigation capabilities.

The Wazuh platform serves as the core of the lab by receiving telemetry from monitored endpoints and presenting security alerts through a web-based dashboard.

---

## Why Wazuh?

Wazuh was selected for this project because it is a powerful open-source SIEM and Extended Detection and Response (XDR) platform that is widely used for cybersecurity education and enterprise security monitoring.

Key features include:

* Centralized log collection
* Security event monitoring
* File Integrity Monitoring (FIM)
* Vulnerability Detection
* Security Configuration Assessment (SCA)
* MITRE ATT&CK mapping
* Custom detection rules
* Agent-based endpoint monitoring

---

## Deployment Environment

| Component         | Value                       |
| ----------------- | --------------------------- |
| Operating System  | Ubuntu Server LTS           |
| Deployment Type   | Single-node Deployment      |
| Platform          | VMware Workstation Pro      |
| Management Method | SSH from Host Machine       |
| Dashboard Access  | Web Browser on Host Machine |

---

## Wazuh Components

The deployment consists of the following core components:

| Component       | Purpose                                                                    |
| --------------- | -------------------------------------------------------------------------- |
| Wazuh Server    | Receives and analyzes security events from monitored endpoints.            |
| Wazuh Indexer   | Stores and indexes collected security data.                                |
| Wazuh Dashboard | Provides a web interface for monitoring, visualization, and investigation. |

---

## Deployment Summary

The Wazuh platform was successfully deployed on the Ubuntu Server virtual machine using the official installation method.

After installation, all required services were verified and the Wazuh Dashboard was successfully accessed from the host machine through a web browser.

The environment is now prepared for endpoint enrollment and centralized security monitoring.

---

## Validation

The deployment was validated by confirming the following:

* Ubuntu Server was operational.
* Wazuh services started successfully.
* The Wazuh Dashboard was accessible.
* Administrative access through SSH was functioning correctly.
* The environment was ready for agent enrollment.

---

## Screenshots

### Wazuh Dashboard Login

<img width="379" height="329" alt="image" src="https://github.com/user-attachments/assets/8ddc2133-679d-4a1b-9a31-b31f3e07b407" />


---

### Wazuh Dashboard

<img width="955" height="434" alt="image" src="https://github.com/user-attachments/assets/cdad3b81-77d2-476b-94db-4fb46be4c0b7" />

---

## Next Steps

The next phase focuses on configuring virtual networking between all lab machines, assigning static IP addresses, validating connectivity, and enrolling the Windows endpoint into the Wazuh platform for centralized monitoring.

