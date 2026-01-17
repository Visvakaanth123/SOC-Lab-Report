This repository contains a SOC lab simulation designed to demonstrate detection and monitoring of a full attack lifecycle in a controlled environment. The lab includes:

1.Ubuntu VM (target)

2.Kali Linux VM (attacker)

3.Splunk Enterprise (log aggregation and alerting)

The project simulates real-world attack scenarios such as port scanning, SSH brute force, data staging, and data exfiltration. Alerts and logs are collected to showcase how a SOC team detects and responds to malicious activity.


Attack Simulation Flow

Reconnaissance – Port Scanning

MITRE ATT&CK: T1046 – Network Service Discovery (Discovery)

Initial Access – SSH Brute Force

MITRE ATT&CK: T1110 – Brute Force (Credential Access)

T1021.004 – Remote Services: SSH (Initial Access)

MITRE ATT&CK: T1074 – Data Staged (Collection)

Data Exfiltration – SCP over SSH

MITRE ATT&CK: T1048 – Exfiltration Over Alternative Protocol (Exfiltration)
