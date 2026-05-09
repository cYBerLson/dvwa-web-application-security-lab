# DVWA Web Application Security Lab

![Platform](https://img.shields.io/badge/Platform-Kali%20Linux-blue)
![Target](https://img.shields.io/badge/Target-Metasploitable%202-red)
![Application](https://img.shields.io/badge/Application-DVWA-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## Project Overview

This project documents the setup of a vulnerable web application security lab using Kali Linux as the attacker machine and Metasploitable 2 as the victim machine. The objective was to access and configure DVWA (Damn Vulnerable Web Application) to create a controlled environment for practicing web penetration testing.

## Objective

The goal of this lab was to:

- Configure a Host-Only network between two virtual machines.
- Verify connectivity between the systems.
- Access DVWA from Kali Linux.
- Log in using default credentials.
- Change the DVWA security level to Low.
- Prepare the environment for future vulnerability testing.

## Lab Environment

| Component | Description |
|--------|--------|
| Virtualization Software | Oracle VM VirtualBox |
| Attacker Machine | Kali Linux |
| Victim Machine | Metasploitable 2 |
| Vulnerable Application | DVWA |
| Browser | Firefox |
| Network Mode | Host-Only Adapter |

## Network Configuration

| Machine | IP Address |
|--------|--------|
| Kali Linux | 192.168.169.5 |
| Metasploitable 2 | 192.168.169.6 |

## Tools Used

- VirtualBox
- Kali Linux
- Metasploitable 2
- DVWA
- Firefox Browser
- ifconfig
- ping

## Step-by-Step Procedure

### 1. Configure Host-Only Network

The network adapter for both virtual machines was configured to use Host-Only Adapter mode in VirtualBox. This ensured that the two systems could communicate directly.


![Host-Only Network]

---

### 2. Verify IP Addresses

The `ifconfig` command was used to confirm that both machines received IP addresses on the same subnet.

#### Kali Linux

```bash
ifconfig 
