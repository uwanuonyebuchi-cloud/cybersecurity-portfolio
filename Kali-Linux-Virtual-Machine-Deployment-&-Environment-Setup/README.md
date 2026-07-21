# Kali Linux Virtual Machine Deployment & Environment Setup

## Overview

This lab demonstrates the deployment and initial configuration of a **Kali Linux Virtual Machine (VM)** using Oracle VirtualBox. The objective was to create a secure virtualized environment for cybersecurity training, penetration testing, network analysis, and hands-on security labs without affecting the host operating system.

---

## Objective

The objective of this lab was to:

- Install Oracle VirtualBox.
- Import and deploy the Kali Linux virtual machine.
- Configure virtual hardware settings.
- Configure networking for internet connectivity.
- Verify successful boot and login.
- Prepare the environment for future cybersecurity labs.

---

## Lab Environment

- Windows 11 (Host)
- Oracle VirtualBox
- Kali Linux Virtual Machine
- Bash Terminal
- GitHub

---

## Scenario

As a cybersecurity student, you need a safe and isolated environment to perform security testing and Linux administration tasks. In this lab, a Kali Linux virtual machine was deployed, configured, and verified to ensure it was ready for future networking, system administration, and cybersecurity exercises.

---

## Activities Performed

- Installed Oracle VirtualBox.
- Imported the Kali Linux virtual machine.
- Configured CPU and memory allocation.
- Configured virtual network settings.
- Started the virtual machine.
- Logged into Kali Linux.
- Verified internet connectivity.
- Updated the operating system.
- Verified terminal functionality.
- Confirmed the environment was ready for cybersecurity labs.

---

## Configuration

### Virtual Machine

- Hypervisor: Oracle VirtualBox
- Guest Operating System: Kali Linux
- Host Operating System: Windows 11

### Virtual Hardware

- RAM: 4 GB (or configured based on host resources)
- Virtual CPUs: 2
- Virtual Hard Disk: Kali Linux Virtual Disk
- Network Adapter: NAT (or Bridged Adapter)

---

## Commands Used

Update package repository:

```bash
sudo apt update
```

Upgrade installed packages:

```bash
sudo apt upgrade
```

Verify current user:

```bash
whoami
```

Display current directory:

```bash
pwd
```

Verify internet connectivity:

```bash
ping google.com
```

Display network interfaces:

```bash
ip addr
```

---

## Verification

The deployment was verified by:

- Successfully booting Kali Linux.
- Logging into the operating system.
- Opening the Bash terminal.
- Confirming internet connectivity.
- Running Linux commands successfully.
- Updating system packages without errors.

---

## Skills Demonstrated

- Virtual Machine Deployment
- Oracle VirtualBox
- Kali Linux Installation
- Linux Environment Setup
- Virtual Networking
- Linux System Administration
- Bash Terminal
- Cybersecurity Lab Preparation
- Operating System Configuration

---

## Key Takeaways

- Learned how to deploy Kali Linux in a virtualized environment.
- Configured virtual hardware and networking settings.
- Verified internet connectivity and system functionality.
- Prepared a dedicated environment for cybersecurity training.
- Built a reusable lab environment for networking, digital forensics, penetration testing, and SOC analyst exercises.

---

## Screenshots

Include screenshots showing:

- Oracle VirtualBox Manager
- Kali Linux virtual machine settings
- Kali Linux desktop
- Terminal window
- Successful login
- System update
- Internet connectivity test

---

## Outcome

This lab demonstrates practical experience deploying and configuring a Kali Linux virtual machine using Oracle VirtualBox. It showcases foundational virtualization, Linux administration, and environment setup skills that support IT Support, System Administration, SOC Analyst, Cybersecurity Analyst, Digital Forensics, and Penetration Testing roles.
