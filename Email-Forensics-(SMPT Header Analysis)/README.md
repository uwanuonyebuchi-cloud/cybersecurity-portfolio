# Email Forensics (SMTP Header Analysis)

## Overview

This lab demonstrates the analysis of **SMTP email headers** to investigate a suspected phishing email. Using publicly available email forensic tools, the objective was to determine whether the email was legitimate, identify the originating mail server, verify sender authentication, and trace the source IP address.

---

## Objective

The objective of this lab was to:

- Analyze SMTP email headers.
- Identify the true sender of an email.
- Verify SPF authentication results.
- Trace the originating IP address.
- Determine whether an email is legitimate or malicious.
- Develop foundational email forensic investigation skills.

---

## Lab Environment

- MXToolbox Email Header Analyzer
- WhatIsMyIPAddress
- Web Browser
- Windows 11
- GitHub

---

## Scenario

A user reported receiving a suspicious email claiming to be from Facebook. As a cybersecurity analyst, the task was to analyze the email headers, determine whether the message was authentic, identify the source of the email, and document the investigation findings.

---

## Activities Performed

- Copied the complete SMTP email header.
- Uploaded the header to MXToolbox Email Header Analyzer.
- Reviewed the email routing path.
- Examined SPF authentication results.
- Identified the originating SMTP server.
- Traced the source IP address.
- Performed IP geolocation.
- Compared the sender address with the Reply-To address.
- Documented indicators of phishing.

---

## Tools Used

- MXToolbox Email Header Analyzer
- WhatIsMyIPAddress
- Windows 11
- Web Browser

---

## Investigation Findings

### Email Subject

```
Someone tried to log in To Your Account, User ID : Victim 1001
```

### Claimed Sender

```
support@facebook.com
```

### Reply-To Address

```
secureinternationalalerts10@gmail.com
```

### Originating IP Address

```
89.144.21.170
```

### Source Location

- Country: Germany
- State: Bayern
- City: Soden
- ISP: GHOSTnet GmbH

### SPF Result

```
SPF = None / Failed
```

The sending server was **not authorized** to send email on behalf of the claimed domain.

---

## Indicators of Compromise (IOCs)

The investigation identified several phishing indicators:

- Suspicious Reply-To address
- SPF authentication failure
- Source IP unrelated to Facebook
- External SMTP server
- Social engineering subject line
- Attempt to impersonate Facebook

---

## Conclusion

The email was determined to be **malicious** and likely part of a phishing campaign because:

- The Reply-To address did not belong to Facebook.
- SPF validation failed.
- The source SMTP server was unrelated to Facebook's infrastructure.
- The originating IP address was associated with an external host.
- Multiple indicators suggested sender spoofing.

---

## Recommended Mitigation

- Do not click links or download attachments.
- Block the sender and originating IP where appropriate.
- Report the email as phishing.
- Verify sender authenticity before responding.
- Enable SPF, DKIM, and DMARC validation.
- Conduct user awareness training on phishing attacks.

---

## Skills Demonstrated

- Email Forensics
- SMTP Header Analysis
- Phishing Investigation
- Email Authentication
- SPF Validation
- IP Address Attribution
- Geolocation Analysis
- Threat Intelligence
- Indicator of Compromise (IOC) Identification
- Cybersecurity Documentation

---

## Key Takeaways

- Learned how SMTP headers reveal the true origin of an email.
- Identified phishing indicators using email header analysis.
- Verified sender authentication through SPF results.
- Traced the originating IP address using publicly available tools.
- Developed practical skills used in SOC operations, incident response, and email security investigations.

---

## Screenshots

Include screenshots showing:

- Original email
- SMTP header
- MXToolbox analysis
- SPF results
- IP geolocation lookup
- Investigation findings
- Phishing indicators

---

## Outcome

This lab demonstrates practical experience investigating suspicious emails using SMTP header analysis. It showcases foundational email forensics, phishing detection, email authentication validation, and threat investigation skills applicable to SOC Analyst, Cybersecurity Analyst, Incident Responder, and Digital Forensics roles.
