# 🔐 Lab Setup — VirtualBox + Kali/Ubuntu + Windows Environment

![Cybersecurity](https://img.shields.io/badge/Domain-Cybersecurity-blue)
![VirtualBox](https://img.shields.io/badge/VirtualBox-Lab-blue)
![TryHackMe](https://img.shields.io/badge/Platform-TryHackMe-red)
![Splunk](https://img.shields.io/badge/SIEM-Splunk-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📌 Project Overview

This project was completed as part of **Week 1 · Task 3 — Lab Setup** during my Cyber Security internship.

The purpose of this task was to understand how a basic SOC lab environment is built using virtualization, Linux, Windows, networking, and security monitoring tools.

The task focused on creating the foundation required for future cybersecurity activities such as:

- Log collection
- SIEM monitoring
- Security investigations
- Network analysis
- Endpoint analysis
- Linux security testing

During this project, I completed the required **TryHackMe Windows Fundamentals 1** room, installed and configured **Oracle VirtualBox**, reviewed the existing Windows environment, prepared VM storage, and documented the practical setup process.

---
Full report: [report/report.md](report/report.md)

## 🎯 Task Objectives

The objectives of this project were:

- Install Oracle VirtualBox.
- Set up a Linux environment using Kali Linux or Ubuntu.
- Set up a Windows environment for analysis.
- Understand internal networking between lab machines.
- Test connectivity between systems.
- Complete the required TryHackMe learning activity.
- Collect screenshots as practical evidence.

---

## 🖥️ Lab Environment

| Component | Purpose |
|---|---|
| Windows Host | Main physical system used for the lab |
| Oracle VirtualBox | Virtualization platform |
| Kali Linux | Planned Linux cybersecurity environment |
| Windows VM | Planned analysis environment |
| Splunk Enterprise | Existing local SIEM environment |
| TryHackMe | Windows fundamentals learning |
| D: Drive | Prepared location for VM storage |

---

## 🏗️ Intended SOC Lab Architecture

```text
                    ┌─────────────────────┐
                    │    Windows Host     │
                    │                     │
                    │   Splunk Enterprise │
                    └──────────┬──────────┘
                               │
                    ┌──────────▼──────────┐
                    │     VirtualBox      │
                    └──────────┬──────────┘
                               │
              ┌────────────────┴────────────────┐
              │                                 │
     ┌────────▼────────┐               ┌────────▼────────┐
     │    Linux VM     │               │    Windows VM   │
     │ Kali / Ubuntu   │               │ Windows 10/11   │
     └─────────────────┘               └─────────────────┘