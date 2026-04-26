# SOC Home Lab with SIEM & Detection Engineering (Wazuh + Sysmon)

This project demonstrates the design and implementation of a Security Operations Center (SOC) Home Lab with SIEM-based detection engineering. The lab simulates real-world attacks, collects logs from endpoints, and builds custom detection rules to identify suspicious activity.

This project is designed to showcase skills, including log analysis, detection engineering, threat simulation, and alert investigation.


#  Lab Architecture

            ┌──────────────┐
            │   Kali Linux │
            │   (Attacker) │
            └──────┬───────┘
                   │
             Attack Simulation
                   │
                   ▼
          ┌──────────────────┐
          │   Windows 10     │
          │  Sysmon + Agent  │
          │   (Victim Host)  │
          └────────┬─────────┘
                   │ Logs
                   ▼
          ┌──────────────────┐
          │   Wazuh SIEM     │
          │ Ubuntu Server    │
          │ Detection Engine │
          └────────┬─────────┘
                   │
                   ▼
              Alerts & Dashboard

              
---

# Project Objectives

- Build a SOC monitoring environment
- Centralize endpoint logs using SIEM
- Implement Sysmon for detailed telemetry
- Simulate real-world attacks
- Create custom detection rules
- Investigate alerts
- Document detection engineering workflow

---

#  Lab Components

| Machine | Role | OS |

| SIEM Server | Log collection & detection | Ubuntu 22.04 |
| Windows Endpoint | Victim + log source | Windows 11 Enterprise |
| Attacker | Attack simulation | Kali Linux |

---

# Technologies Used

- Wazuh SIEM
- Elastic Stack
- Sysmon
- Kali Linux
- Windows Event Logs
- Ubuntu Server
- Nmap
- Hydra
- PowerShell
- MITRE ATT&CK

---

#  Setup Instructions

## Step 1 — Create Virtual Machines

Create three VMs:

### SIEM Server
- Ubuntu 22.04
- 8GB RAM (minimum 4GB)
- 2 CPU
- 60GB disk

### Windows Endpoint
- Windows 11
- 4GB RAM
- 64GB disk

### Attacker Machine
- Kali Linux
- 2GB RAM

