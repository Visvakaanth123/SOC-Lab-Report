This repository contains a SOC lab simulation designed to demonstrate detection and monitoring of a full attack lifecycle in a controlled environment. The lab includes:

1.Ubuntu VM (target)

2.Kali Linux VM (attacker)

3.Splunk Enterprise (log aggregation and alerting)

The project simulates real-world attack scenarios such as port scanning, SSH brute force, data staging, and data exfiltration. Alerts and logs are collected to showcase how a SOC team detects and responds to malicious activity.


Attack Simulation Flow

Reconnaissance – Port Scanning

MITRE ATT&CK: T1046 – Network Service Discovery (Discovery)

A custom Python script scans for open ports on the Ubuntu VM. Alerts triggered in Splunk.

Initial Access – SSH Brute Force

MITRE ATT&CK:

T1110 – Brute Force (Credential Access)

T1021.004 – Remote Services: SSH (Initial Access)

Attacker uses repeated SSH login attempts to gain access. Brute force alerts captured in Splunk.

Post-Exploitation – Data Staging

MITRE ATT&CK: T1074 – Data Staged (Collection)

Files of interest are aggregated into a staging directory on the compromised system. Activity captured through host-based audit logs.

Data Exfiltration – SCP over SSH

MITRE ATT&CK: T1048 – Exfiltration Over Alternative Protocol (Exfiltration)

Aggregated files are transferred to the attacker VM using SCP over SSH. Logs indicate exfiltration activity.
