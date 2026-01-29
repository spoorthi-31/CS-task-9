Network Vulnerability Scanning Using Nmap
Overview

This project demonstrates network vulnerability scanning using Nmap, a widely used open-source network scanning tool. 
The goal of the project is to identify active devices, open ports, running services, operating systems, and potential vulnerabilities within a network.
By performing these scans, one can assess the security posture of a network and take necessary actions to mitigate risks.

Features

Scan local network to identify active devices

Detect open TCP and UDP ports

Identify running services and versions

Detect the operating system of target devices

Perform vulnerability analysis using Nmap scripts

Save scan results for reporting and analysis

Tools & Technologies

Tool: Nmap (Network Mapper)

OS: Windows / Linux

Languages: Bash / Command Line

Objectives

Discover all devices on the local network

Identify open ports and associated services

Detect operating systems of target devices

Analyze vulnerabilities and assess risk

Document findings for network security improvement

Methodology

Network Discovery: Scan the network to identify active hosts.

Port Scanning: Detect open TCP and UDP ports.

Service Detection: Identify running services and their versions.

OS Detection: Determine the operating system of each host.

Vulnerability Analysis: Run Nmap scripts to check for known vulnerabilities.

Report Generation: Save scan results in text or XML format for documentation.

Nmap Commands Used

Some of the common commands used in this project:

# Discover active hosts in the network
nmap -sn 192.168.1.0/24

# TCP SYN Scan
nmap -sS 192.168.1.1

# Service detection with version info
nmap -sV 192.168.1.1

# Operating system detection
nmap -O 192.168.1.1

# Vulnerability scanning using Nmap scripts
nmap --script vuln 192.168.1.1

Sample Results
Host	Port	Service	State	Risk Level
192.168.1.1	22	SSH	Open	Medium
192.168.1.1	80	HTTP	Open	High
192.168.1.2	443	HTTPS	Open	Low

Screenshots of actual Nmap scan outputs can be added in the Screenshots/ folder.

Risk Analysis

Open ports can be exploited if left unprotected

Outdated services are vulnerable to known exploits

Unnecessary services increase the attack surface

Recommendations:

Close unused ports

Update services regularly


Implement firewalls and access restrictions

Use strong authentication mechanisms

Conclusion

This project demonstrates how Nmap can be effectively used to analyze a network’s security posture.
By identifying vulnerabilities early, organizations and individuals can take proactive measures to strengthen network security. 
Regular scanning and monitoring are key to maintaining a secure network.
