# Network Packet Capture with tcpdump

## Overview

This lab demonstrates the use of **tcpdump** to capture live network traffic from a network interface. The objective was to monitor network communications, capture packets for analysis, and gain hands-on experience using a command-line packet capture tool commonly used by network administrators, SOC analysts, and incident responders.

---

## Objective

The objective of this lab was to:

- Capture live network traffic using tcpdump.
- Monitor network activity from a Linux terminal.
- Save captured packets to a PCAP file.
- Analyze network communications.
- Develop practical packet capture skills for troubleshooting and security investigations.

---

## Lab Environment

- Kali Linux
- tcpdump
- Linux Terminal
- Windows 11 (Host)
- VirtualBox
- GitHub

---

## Scenario

As a cybersecurity analyst, the task was to capture live network traffic from a network interface. The captured packets were saved for later analysis to identify network communications, troubleshoot connectivity issues, and support security investigations.

---

## Activities Performed

- Identified available network interfaces.
- Selected the appropriate interface for packet capture.
- Captured live network traffic.
- Monitored packets in real time.
- Saved captured traffic to a PCAP file.
- Stopped the capture after collecting sufficient data.
- Verified the capture file for future analysis.

---

## Commands Used

Examples of commands used during the lab:

```bash
ip addr
```

```bash
tcpdump -D
```

```bash
sudo tcpdump -i eth0
```

```bash
sudo tcpdump -i eth0 -c 100
```

```bash
sudo tcpdump -i eth0 -w capture.pcap
```

```bash
tcpdump -r capture.pcap
```

> **Note:** The network interface name (e.g., `eth0`, `ens33`, or `wlan0`) may vary depending on the system configuration.

---

## Information Captured

The packet capture included:

- Source IP addresses
- Destination IP addresses
- Source and destination ports
- TCP packets
- UDP packets
- DNS queries
- ICMP traffic
- Packet timestamps
- Network protocols

---

## Skills Demonstrated

- Live Packet Capture
- tcpdump
- Linux Command Line
- Network Traffic Monitoring
- TCP/IP Fundamentals
- Packet Capture (PCAP)
- Network Troubleshooting
- Cybersecurity Documentation

---

## Key Takeaways

- Learned how to capture live network traffic using tcpdump.
- Gained experience monitoring network communications from the command line.
- Practiced saving packet captures for later forensic analysis.
- Improved understanding of network protocols and packet flow.
- Developed foundational skills used in SOC operations, network administration, and incident response.

---

## Screenshots

Include screenshots showing:

- Terminal with tcpdump commands
- Live packet capture
- Network interface selection
- Packet capture saved to a PCAP file
- Terminal output displaying captured packets

---

## Outcome

This lab demonstrates practical experience using **tcpdump** to capture live network traffic, monitor network communications, and create packet capture (PCAP) files for further analysis. It showcases foundational networking and cybersecurity skills applicable to IT Support, Network Administrator, SOC Analyst, Cybersecurity Analyst, and Incident Response roles.
