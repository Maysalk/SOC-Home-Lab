# Architecture Summary

## Overview

The SOC Home Lab consists of three virtual machines running on VMware Workstation Pro. Each machine performs a dedicated role that collectively simulates a small enterprise security environment.

The architecture is intentionally simple while providing sufficient functionality for security monitoring, attack simulation, and incident response exercises.

---

## Lab Architecture

```text
                    Host Machine
                         │
              VMware Workstation Pro
                         │
     ┌───────────────────┼───────────────────┐
     │                   │                   │
 Windows 10         Kali Linux        Ubuntu Server
 (Victim)          (Attacker)        (Wazuh SIEM)
```

---

## Components

### Windows 10

Acts as the monitored endpoint where security events are generated. This system will be monitored using Sysmon and the Wazuh Agent.

---

### Kali Linux

Acts as the attacker machine responsible for generating realistic attack scenarios throughout the project.

---

### Ubuntu Server

Hosts the Wazuh platform, which collects, indexes, analyzes, and visualizes security events from monitored systems.

---

## Communication Flow

The Windows endpoint forwards security telemetry to the Wazuh server through the Wazuh Agent.

Kali Linux generates attack traffic against the Windows endpoint, allowing Wazuh to detect, analyze, and generate alerts based on observed activity.

The Ubuntu Server is managed remotely through SSH, while the Wazuh Dashboard is accessed from the host machine using a web browser.

---

## Next Phase

With the architecture established, the next phase focuses on configuring the virtual network, assigning static IP addresses, validating connectivity, and preparing the environment for endpoint enrollment.

