
![](images/intro.png)

## Executive Summary

- This project is about a **Network** consisting of two servers, a penetration testing Kali VM and an ELK stack server.

- Initially, **Blue Team Defenses** are configured in **Kibana** to generate alerts in the setting of an attack, while analyzing 'beats' (filebeat, packetbeat, metricbeat) received from an ELK Stack server

- The two servers (Target 1, Target 2) are vulnerable and a **Red Team Penetration Testing** with Kali VM is performed to attack these two targets using the principals of engagement 
    - Information gathering
    - Scanning and enumeration
    - Exploitation
    - Post-Exploitation
    - Reporting

- While the Red Team Peneteration Attacks are in operation, the **Kibana software is monitored** in live stream to test the efficacy of Blue Team Defenses in setting off the appropriate alarms

- With all the new information about system wulnerabilities, a final **Purple Team Hardening** is performed against the vulnerabilities discovered during the Red Team penetration testing and the weaknesses identified in the Blue Team Defenses