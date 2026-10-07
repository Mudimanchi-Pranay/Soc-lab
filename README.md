# 🛡️ SOC Home Lab

A hands-on Security Operations Center (SOC) home lab focused on security
monitoring, log analysis, alert triage, threat detection, IOC investigation,
and incident-response workflows.

The purpose of this project is to build practical experience investigating
common security events across Windows endpoints and network infrastructure
within a controlled lab environment.

---

## 🎯 Project Objectives

The SOC Home Lab is designed to provide practical exposure to:

- Security monitoring and alert triage
- Windows Event Log analysis
- Sysmon telemetry analysis
- Network traffic investigation
- Firewall and network security monitoring
- IOC extraction and investigation
- Phishing investigation
- Brute-force detection
- Suspicious PowerShell activity detection
- Port-scanning investigation
- Malware activity investigation
- MITRE ATT&CK technique mapping
- Incident documentation and escalation
- Basic threat-hunting workflows

---

## 🏗️ Lab Architecture

```text
                         ┌──────────────────────┐
                         │       Attacker       │
                         │      Kali Linux      │
                         └──────────┬───────────┘
                                    │
                              Attack Traffic
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │       pfSense        │
                         │ Firewall / Network   │
                         │      Monitoring      │
                         └──────────┬───────────┘
                                    │
                           Network Activity
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │   Windows Endpoint   │
                         │                      │
                         │       Sysmon         │
                         │   Windows Event Logs │
                         └──────────┬───────────┘
                                    │
                              Security Events
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │      SOC Analyst     │
                         │                      │
                         │ Alert Triage         │
                         │ Log Analysis         │
                         │ IOC Investigation    │
                         │ Incident Response    │
                         └──────────────────────┘
