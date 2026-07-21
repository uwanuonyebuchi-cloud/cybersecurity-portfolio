#  Snort Intrusion Detection System (IDS)

## Overview

This lab demonstrates the installation, configuration, and operation of **Snort**, an open-source Network Intrusion Detection System (IDS). The objective was to monitor network traffic, analyze packets in real time, and understand how Snort detects suspicious network activity using rule-based detection.

---

## Objective

The objective of this lab was to:

- Install and configure Snort.
- Understand the role of an Intrusion Detection System (IDS).
- Monitor live network traffic.
- Analyze packets in real time.
- Learn how Snort processes and inspects network traffic.
- Prepare the environment for creating custom detection rules.

---

## Lab Environment

- Kali Linux
- Snort IDS
- Linux Terminal
- VirtualBox
- GitHub

---

## Scenario

As a Security Operations Center (SOC) analyst, you are responsible for monitoring network traffic for suspicious or malicious activity. In this lab, Snort was configured to inspect network packets in real time, providing visibility into network communications and preparing the environment for intrusion detection.

---

## Activities Performed

- Verified Snort installation.
- Reviewed the Snort configuration file (`snort.conf`).
- Configured Snort to monitor the appropriate network interface.
- Started Snort in Intrusion Detection mode.
- Monitored live network traffic.
- Observed packet inspection and protocol analysis.
- Verified Snort successfully processed incoming and outgoing traffic.

---

## Tools Used

- Snort IDS
- Kali Linux
- Linux Terminal

---

## Example Commands

Verify Snort version:

```bash
snort -V
```

Run Snort in IDS mode:

```bash
sudo snort -A console -q -c /etc/snort/snort.conf -i eth0
```

Test Snort configuration:

```bash
sudo snort -T -c /etc/snort/snort.conf
```

---

## Network Traffic Observed

During the lab, Snort monitored:

- TCP traffic
- UDP traffic
- ICMP packets
- ARP traffic
- DNS requests
- HTTP traffic

---

## Investigation Findings

The monitoring session confirmed that:

- Snort initialized successfully.
- Configuration loaded without errors.
- Network packets were inspected in real time.
- Multiple network protocols were analyzed.
- The IDS environment was successfully prepared for signature-based detection.

---

## Skills Demonstrated

- Intrusion Detection Systems (IDS)
- Snort Configuration
- Network Traffic Monitoring
- Packet Inspection
- Linux Administration
- Network Security
- Protocol Analysis
- Cybersecurity Documentation

---

## Key Takeaways

- Learned how an Intrusion Detection System monitors network traffic.
- Gained hands-on experience configuring Snort.
- Improved understanding of signature-based intrusion detection.
- Practiced monitoring live network communications.
- Built a foundation for creating and testing custom Snort detection rules.

---

## Screenshots

Include screenshots showing:

- Snort installation
- Snort configuration
- Terminal running Snort
- Live packet monitoring
- Configuration validation
- Network traffic inspection

---

## Outcome

This lab demonstrates practical experience deploying and operating the Snort Intrusion Detection System (IDS) to monitor live network traffic. It highlights foundational skills in network monitoring, packet inspection, and intrusion detection that are applicable to SOC Analyst, Cybersecurity Analyst, Network Security Analyst, and Incident Response roles.
