# Red Team: Summary of Operations

## Table of Contents
- Exposed Services
- Critical Vulnerabilities
- Exploitation

### Exposed Services

Nmap scan results for each machine reveal the below services and OS details:

```bash
nmap -sS -A 192.168.1.110

```
  ![](../images/nmap-a1.png)
  ![](../images/nmap-a2.png)


This scan identifies the services below as potential points of entry:

- **Target 1**

- Open port 22 dedicated to SSH services
- Open port 80 dedicated to HTTP services
- Apache http version 2.4.1.0
- OS version Windows 6.1 (Smba 4.2)


  

_TODO: Fill out the list below. Include severity, and CVE numbers, if possible._

The following vulnerabilities were identified on each target:
- Target 1
  - List of
  - Critical
  - Vulnerabilities

_TODO: Include vulnerability scan results to prove the identified vulnerabilities._

### Exploitation


The Red Team was able to penetrate `Target 1` and retrieve the following confidential data:
- Target 1
  - `flag1.txt`: _TODO: Insert `flag1.txt` hash value_
    - **Exploit Used**
      - Remote SSH connection after identifying a user with wpscan. One of the users identified was michael
     - ` wpscan --url http://192.168.1.110/wordpress -eu`
     
     - Brute forcing the pssword for michael wiht hydra
     - 


      - Using gobuster to identify web directories and exploring them during scanning and enumeration 
      - Inspecting the source code for the service page and identified the flag in comments under the code for the html footer
      - _TODO: Include the command run_
  - `flag2.txt`: _TODO: Insert `flag2.txt` hash value_
    - **Exploit Used**
      - _TODO: Identify the exploit used_
      - _TODO: Include the command run_