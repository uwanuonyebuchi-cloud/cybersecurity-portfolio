# SQL Injection (SQLi) Authentication Bypass

## Overview

This lab demonstrates a **SQL Injection (SQLi) Authentication Bypass** attack against a deliberately vulnerable web application in a controlled lab environment. The objective was to understand how insecure input validation can allow attackers to bypass authentication and gain unauthorized access to an application.

> **Note:** This lab was performed in an authorized training environment for educational purposes only.

---

## Objective

The objective of this lab was to:

- Understand the fundamentals of SQL Injection.
- Identify a vulnerable login form.
- Demonstrate how improper input validation can lead to authentication bypass.
- Understand the risks associated with insecure SQL queries.
- Learn security best practices to prevent SQL Injection attacks.

---

## Lab Environment

- Kali Linux
- Firefox Web Browser
- Deliberately Vulnerable Web Application
- Localhost Web Server
- GitHub

---

## Scenario

A web application login page was intentionally configured with an insecure SQL query that did not properly validate user input. The goal was to demonstrate how SQL Injection can bypass authentication and why secure coding practices are essential.

---

## Activities Performed

- Accessed the vulnerable login page.
- Examined the authentication form.
- Tested the application for SQL Injection vulnerability.
- Successfully bypassed the login process in the lab environment.
- Verified unauthorized access to the protected application.
- Reviewed why the attack succeeded.
- Documented security recommendations.

---

## Vulnerability Identified

The application accepted unsanitized user input, allowing malicious SQL statements to modify the authentication query.

This vulnerability existed because:

- User input was not validated.
- SQL queries were not parameterized.
- Prepared statements were not implemented.

---

## Security Impact

A successful SQL Injection attack can allow an attacker to:

- Bypass authentication
- Access sensitive information
- Modify or delete database records
- Escalate privileges
- Execute unauthorized database queries
- Compromise application confidentiality, integrity, and availability

---

## Mitigation Strategies

Recommended security controls include:

- Use parameterized queries (Prepared Statements)
- Validate and sanitize user input
- Implement least privilege for database accounts
- Use stored procedures where appropriate
- Deploy a Web Application Firewall (WAF)
- Perform secure code reviews
- Conduct regular vulnerability assessments
- Monitor application logs for suspicious activity

---

## Skills Demonstrated

- Web Application Security
- SQL Injection Fundamentals
- Authentication Security
- Vulnerability Assessment
- Secure Coding Awareness
- OWASP Top 10 Concepts
- Cybersecurity Documentation
- Risk Analysis

---

## Key Takeaways

- Learned how SQL Injection vulnerabilities occur.
- Understood how poor input validation can lead to authentication bypass.
- Gained practical experience identifying SQL Injection risks in a controlled environment.
- Reinforced secure development practices that help prevent SQL Injection attacks.
- Improved understanding of one of the most common web application vulnerabilities.

---

## Screenshots

Include screenshots showing:

- Vulnerable login page
- Successful authentication bypass (lab environment)
- Application after successful login
- SQL Injection demonstration
- Lab results

---

## Outcome

This lab demonstrates practical knowledge of SQL Injection (SQLi) and authentication bypass techniques in a controlled training environment. It highlights an understanding of common web application vulnerabilities, the importance of secure input validation, and industry best practices for preventing SQL Injection attacks. These skills are relevant to Cybersecurity Analyst, SOC Analyst, Vulnerability Management, Application Security, and Penetration Testing roles.
