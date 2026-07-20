# Sensitive Information Exposure via Misconfigured Web Server

## Overview

This lab simulates a security assessment of a misconfigured web server that unintentionally exposes sensitive information. The objective was to identify publicly accessible confidential data, understand the security risks associated with improper server configurations, and recommend remediation measures to reduce the organization's attack surface.

---

## Objective

The objective of this lab was to:

- Identify sensitive information exposed by a misconfigured web server.
- Assess the security risks associated with information disclosure.
- Recognize common web server misconfigurations.
- Document findings and recommend corrective actions.
- Develop practical web security assessment skills.

---

## Lab Environment

- Kali Linux
- Web Browser
- Linux Terminal
- Windows 11 (Host)
- GitHub

---

## Scenario

During a routine security assessment, a web server was found to expose files and information that should not have been publicly accessible. The investigation focused on identifying exposed resources, determining the potential security impact, and recommending remediation to protect sensitive organizational data.

---

## Activities Performed

- Accessed the web server.
- Identified publicly accessible resources.
- Examined exposed directories and files.
- Reviewed HTTP responses.
- Documented sensitive information discovered.
- Assessed the potential security impact.
- Recommended remediation measures.

---

## Evidence Collected

Examples of exposed information included:

- Directory listings
- Configuration files
- Backup files
- Log files
- Server version information
- Application error messages
- Internal file paths
- Administrative resources

---

## Security Risks Identified

Potential risks associated with the exposure included:

- Information disclosure
- Unauthorized access
- Credential exposure
- Increased attack surface
- Server fingerprinting
- Reconnaissance opportunities
- Data leakage
- Privilege escalation opportunities

---

## Recommended Mitigation

- Disable directory listing.
- Remove unnecessary public files.
- Restrict access to sensitive directories.
- Secure configuration and backup files.
- Implement proper file permissions.
- Configure custom error pages.
- Keep web server software updated.
- Perform regular security assessments and vulnerability scans.

---

## Skills Demonstrated

- Web Security Assessment
- Information Disclosure Analysis
- Security Misconfiguration Identification
- Vulnerability Assessment
- Risk Analysis
- Cybersecurity Documentation
- Security Best Practices
- Incident Reporting

---

## Key Takeaways

- Learned how web server misconfigurations can expose sensitive information.
- Improved understanding of common information disclosure vulnerabilities.
- Practiced identifying exposed files and directories.
- Reinforced the importance of secure web server configuration and access controls.
- Developed practical skills applicable to web security assessments and vulnerability management.

---

## Screenshots

Include screenshots showing:

- Misconfigured web server
- Exposed directory listing
- Sensitive files or information discovered
- HTTP responses
- Investigation findings
- Recommended remediation

---

## Outcome

This lab demonstrates practical experience identifying sensitive information exposure caused by a misconfigured web server. It showcases foundational skills in web application security, vulnerability assessment, and risk analysis that are valuable for SOC Analyst, Cybersecurity Analyst, Penetration Tester, Vulnerability Management, and Security Engineer roles.
