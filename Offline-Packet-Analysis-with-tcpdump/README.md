# Offline Packet Analysis with tcpdump

## Overview

This lab demonstrates how to use **tcpdump**, a command-line packet analyzer, to perform offline network traffic analysis using previously captured packet capture (PCAP) files. The objective was to inspect network traffic, identify network protocols, investigate suspicious communications, and extract useful information for troubleshooting and incident response.

---

## Objective

The objective of this lab was to:

- Analyze packet capture (PCAP) files using tcpdump.
- Interpret network traffic from the command line.
- Identify common network protocols.
- Filter traffic based on IP addresses, ports, and protocols.
- Develop foundational packet analysis skills used in cybersecurity investigations.

---

## Lab Environment

- Kali Linux
- tcpdump
- Terminal
- Windows 11 (Host)
- GitHub

---

## Scenario

A packet capture (PCAP) file containing network traffic was provided for analysis. As a cybersecurity analyst, the goal was to examine the traffic using tcpdump, identify communication between hosts, inspect protocols, and determine whether any suspicious activity was present.

---

## Activities Performed

- Opened a PCAP file using tcpdump.
- Displayed packet summaries.
- Examined source and destination IP addresses.
- Identified network protocols.
- Filtered packets by protocol and host.
- Reviewed TCP and UDP communications.
- Documented investigation findings.

---

## Commands Used

Examples of commands used during the lab:

```bash
tcpdump -r capture.pcap
```

```bash
tcpdump -nn -r capture.pcap
```

```bash
tcpdump -r capture.pcap tcp
```

```bash
tcpdump -r capture.pcap udp
```

```bash
tcpdump -r capture.pcap port 80
```

```bash
tcpdump -r capture.pcap host 192.168.1.10
```

---

## Network Information Analyzed

The investigation focused on:

- Source IP addresses
- Destination IP addresses
- Source ports
- Destination ports
- TCP connections
- UDP traffic
- DNS queries
- HTTP traffic
- Packet timestamps
- Protocol usage

---

## Protocols Identified

The following protocols were analyzed:

- TCP
- UDP
- DNS
- HTTP
- HTTPS
- ICMP
- ARP

---

## Investigation Findings

The packet analysis allowed identification of:

- Network communication between hosts.
- Active network protocols.
- Source and destination devices.
- Network conversations.
- Traffic patterns.
- Potential abnormal or suspicious activity.

---

## Skills Demonstrated

- tcpdump Packet Analysis
- Offline Network Forensics
- Network Traffic Analysis
- Linux Command Line
- TCP/IP Analysis
- Protocol Analysis
- Cybersecurity Investigation
- Incident Response Fundamentals
- Cybersecurity Documentation

---

## Key Takeaways

- Learned how to analyze packet captures using tcpdump.
- Improved understanding of command-line packet analysis.
- Practiced filtering traffic by protocol, host, and port.
- Developed foundational skills used in network forensics and incident response.
- Reinforced knowledge of common network protocols and communication patterns.

---

## Screenshots

Include screenshots showing:

- tcpdump commands executed
- Terminal output
- Packet summaries
- Protocol analysis
- Source and destination IP addresses
- Filtered packet results

---

## Outcome

This lab demonstrates practical experience using **tcpdump** to perform offline packet analysis of PCAP files. It highlights foundational skills in network forensics, protocol analysis, and command-line packet inspection that are valuable for IT Support, SOC Analyst, Cybersecurity Analyst, Incident Response, and Digital Forensics roles.
