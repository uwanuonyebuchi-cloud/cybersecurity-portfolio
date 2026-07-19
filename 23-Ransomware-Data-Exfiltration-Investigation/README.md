# Lab 23 – Ransomware Data Exfiltration Investigation

## Overview
This lab simulates a Security Operations Center (SOC) investigation into a suspected ransomware attack. The objective was to analyze system logs and indicators of compromise (IOCs) to determine whether data exfiltration occurred, identify the destination IP address, and assess the likely ransomware family involved.

---

## Scenario

A workstation generated several suspicious security alerts indicating possible ransomware activity. Network logs, process information, and ransomware indicators were reviewed to determine:

- Whether data was exfiltrated
- Which IP address received the outbound data
- The likely ransomware family
- Appropriate incident response actions

---

## Objectives

- Analyze security logs
- Identify Indicators of Compromise (IOCs)
- Detect evidence of data exfiltration
- Identify suspicious outbound connections
- Determine the likely ransomware family
- Recommend containment and remediation actions
- Document findings in an incident report

---

## Tools Used

- ChatGPT (Log Analysis)
- Windows
- Microsoft Word
- GitHub

---

## Indicators of Compromise (IOCs)

- Suspicious executable:
  - `/tmp/lockbit_enc`

- Encrypted file extension:
  - `.HLJkNskOq`

- Ransom note:
  - `README.txt`

- Suspicious outbound IP:
  - `185.216.71.200`

- High outbound HTTPS traffic over TCP 443

---

## Investigation Steps

1. Reviewed network log timeline.
2. Identified unusual outbound traffic.
3. Examined the suspicious process.
4. Reviewed ransomware indicators.
5. Correlated network activity with process execution.
6. Determined whether data exfiltration occurred.
7. Identified the destination IP address.
8. Assessed the probable ransomware family.
9. Documented findings.
10. Recommended incident response actions.

---

## Investigation Findings

### Evidence of Data Exfiltration

Evidence strongly suggested that data was transmitted shortly after the ransomware process executed.

Observed indicators included:

- High outbound packet count
- Approximately 2 MB transferred
- Encrypted HTTPS communication
- Outbound connection immediately following ransomware execution

---

### Destination IP

**185.216.71.200**

This IP address was identified as the most likely destination for the exfiltrated data.

---

### Probable Ransomware Family

Based on the collected indicators, the activity was most consistent with:

**LockBit 3.0 / LockBit Black**

Confidence Level:

**Moderate to High**

Supporting evidence included:

- LockBit-style executable name
- Randomized encrypted file extension
- Generic LockBit ransom note
- Data exfiltration behavior
- Double-extortion characteristics

---

## Recommended Incident Response

- Isolate the affected endpoint
- Block communication with the malicious IP
- Preserve logs and forensic evidence
- Search other systems for matching IOCs
- Reset compromised credentials
- Begin malware eradication procedures
- Perform threat hunting across the environment
- Restore affected systems from clean backups if necessary

---

## Skills Demonstrated

- Security Log Analysis
- Incident Response
- Threat Hunting
- Network Traffic Analysis
- IOC Identification
- Ransomware Investigation
- Data Exfiltration Detection
- Digital Forensics
- Cybersecurity Documentation
- Security Reporting

---

## Key Takeaways

- Identified evidence of ransomware-related data exfiltration.
- Correlated process execution with network activity.
- Determined the likely exfiltration destination.
- Assessed the probable ransomware family using multiple indicators.
- Produced a structured incident investigation report.

---

## Screenshots

Add screenshots demonstrating:

- Log timeline analysis
- Indicators of compromise
- Data exfiltration findings
- Destination IP identification
- LockBit attribution analysis
- Incident response recommendations

---

## Outcome

This lab demonstrates practical SOC analyst skills by investigating a ransomware incident, identifying indicators of compromise, detecting likely data exfiltration, attributing the attack to the LockBit ransomware family with moderate-to-high confidence, and documenting recommended containment and remediation actions.
