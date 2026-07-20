# Deploying an Nginx Web Server

## Overview

This lab demonstrates the deployment and basic configuration of an **Nginx** web server on a Linux system. The objective was to install Nginx, verify that the web service was running, host a simple web page, and understand the fundamentals of web server administration.

---

## Objective

The objective of this lab was to:

- Install the Nginx web server.
- Start and manage the Nginx service.
- Verify web server functionality.
- Deploy a basic web page.
- Understand the role of Nginx in web hosting and network services.

---

## Lab Environment

- Kali Linux
- Nginx
- Linux Terminal
- Windows 11 (Host)
- VirtualBox
- GitHub

---

## Scenario

A new Linux server was provisioned to host an internal company website. As the system administrator, the task was to install and configure Nginx, verify that the service was operational, and deploy a simple webpage for users to access.

---

## Activities Performed

- Updated the system package repository.
- Installed the Nginx web server.
- Started the Nginx service.
- Enabled Nginx to start automatically on boot.
- Verified the service status.
- Accessed the default Nginx web page through a browser.
- Replaced the default page with a custom HTML page.
- Tested successful web page delivery.

---

## Commands Used

Examples of commands used during the lab:

```bash
sudo apt update
```

```bash
sudo apt install nginx
```

```bash
sudo systemctl start nginx
```

```bash
sudo systemctl enable nginx
```

```bash
sudo systemctl status nginx
```

```bash
curl http://localhost
```

```bash
sudo nano /var/www/html/index.html
```

---

## Verification

The deployment was verified by:

- Confirming the Nginx service was active.
- Accessing the default Nginx welcome page.
- Viewing the custom web page through a web browser.
- Confirming HTTP requests were successfully served.

---

## Skills Demonstrated

- Linux System Administration
- Nginx Installation and Configuration
- Web Server Deployment
- Linux Command Line
- Service Management
- Basic Web Hosting
- HTTP Fundamentals
- Cybersecurity Documentation

---

## Key Takeaways

- Learned how to deploy an Nginx web server on Linux.
- Gained experience managing services using `systemctl`.
- Understood the default web root directory and website hosting process.
- Practiced verifying service availability using browser and command-line tools.
- Developed foundational Linux administration skills applicable to server management.

---

## Screenshots

Include screenshots showing:

- Nginx installation
- Terminal commands
- Service status (`systemctl status nginx`)
- Default Nginx welcome page
- Custom web page
- Browser accessing the web server

---

## Outcome

This lab demonstrates practical experience deploying and managing an Nginx web server on Linux. It highlights foundational Linux administration, web server management, and networking skills applicable to IT Support, System Administrator, DevOps, Cybersecurity Analyst, and SOC Analyst roles.
