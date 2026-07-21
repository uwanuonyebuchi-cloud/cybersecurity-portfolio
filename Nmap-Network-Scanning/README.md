#  Nmap Network Scanning

## Overview

This lab demonstrates the use of **Nmap (Network Mapper)** to perform network reconnaissance and identify active hosts, open ports, and running services within a controlled lab environment. Nmap is one of the most widely used tools by network administrators, penetration testers, and Security Operations Center (SOC) analysts for network discovery and security auditing.

> **Note:** This lab was performed in a controlled home lab environment for educational and defensive security purposes only.

---

## Objective

The objective of this lab was to:

- Discover active hosts on a network.
- Identify open TCP ports.
- Detect running network services.
- Understand basic network reconnaissance techniques.
- Develop foundational network scanning skills used in cybersecurity.

---

## Lab Environment

- Kali Linux
- Nmap
- Linux Terminal
- VirtualBox
- Windows 11 (Host)
- GitHub

---

## Scenario

As a cybersecurity analyst, you were tasked with identifying services running on a target system within a controlled lab environment. Using Nmap, you performed a basic TCP scan to identify open ports and determine which services were available.

---

## Activities Performed

- Verified connectivity to the target host.
- Performed a basic TCP port scan.
- Identified open and closed ports.
- Detected active network services.
- Analyzed scan results.
- Documented network reconnaissance findings.

---

## Commands Used

Basic scan:

```bash
nmap 127.0.0.1
```

Targeted port scan:

```bash
nmap -p 21 172.17.0.2
```

Service version detection (optional):

```bash
nmap -sV 127.0.0.1
```

---

## Scan Results

The scan identified:

- Target Host: **127.0.0.1 (localhost)**
- Host Status: **Up**
- Open Port:
  - **3306/tcp – MySQL**
- Closed Ports:
  - **999 closed TCP ports**

Additional scans were performed against a Docker-hosted target to validate IDS detection and network connectivity.

---

## Services Identified

Examples of services discovered:

- MySQL (Port 3306)
- FTP (Port 21 during testing)
- TCP Services
- Localhost services

---

## Skills Demonstrated

- Network Reconnaissance
- Network Scanning
- Port Enumeration
- Service Identification
- Nmap
- TCP/IP Fundamentals
- Linux Command Line
- Cybersecurity Documentation

---

## Key Takeaways

- Learned how to use Nmap for host discovery and network reconnaissance.
- Identified open ports and running services on a target system.
- Gained experience interpreting Nmap scan results.
- Reinforced the importance of minimizing exposed services to reduce the attack surface.
- Developed foundational skills used in vulnerability assessments, penetration testing, and SOC investigations.

---

## Screenshots

Include screenshots showing:

- Nmap command execution
- Terminal output
- Open port identification
- Service detection results
- Target host information

---

## Outcome

This lab demonstrates practical experience using **Nmap** to perform network reconnaissance, identify active hosts, discover open ports, and detect running services in a controlled lab environment. It showcases foundational networking and cybersecurity skills applicable to IT Support, Network Administrator, SOC Analyst, Cybersecurity Analyst, Vulnerability Management, and Penetration Testing roles.
