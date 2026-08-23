# 🔐 Lab Setup — VirtualBox + Kali/Ubuntu + Windows Environment

![Cybersecurity](https://img.shields.io/badge/Domain-Cybersecurity-blue)
![VirtualBox](https://img.shields.io/badge/Tool-VirtualBox-blue)
![TryHackMe](https://img.shields.io/badge/Platform-TryHackMe-red)
![Splunk](https://img.shields.io/badge/SIEM-Splunk-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📌 Project Overview

This project was completed as part of **Week 1 · Task 3** of a Cyber Security internship.

The purpose of this task was to understand how to build a basic SOC lab environment using VirtualBox, Linux, Windows, networking, and security monitoring tools.

The project included:

- Installing Oracle VirtualBox
- Preparing a Linux virtual machine environment
- Understanding the role of a Windows analysis environment
- Preparing VM storage on a secondary drive
- Reviewing networking requirements for an isolated SOC lab
- Completing TryHackMe — Windows Fundamentals 1
- Documenting the practical setup process with screenshots
- Reviewing the existing local Splunk SIEM environment

---

## 🎯 Objectives

The main objectives of this project were:

1. Install Oracle VirtualBox.
2. Prepare a Linux environment for cybersecurity practice.
3. Understand the role of a Windows environment in a SOC lab.
4. Prepare the system for isolated virtual networking.
5. Understand how connectivity testing would be performed between systems.
6. Complete the required TryHackMe learning activity.
7. Collect practical evidence through screenshots.

---

## 🖥️ Lab Environment

The available lab environment consisted of:

| Component | Purpose |
|---|---|
| Windows Host | Primary workstation and analysis environment |
| Splunk Enterprise | Local SIEM and security monitoring environment |
| Oracle VirtualBox | Virtualization platform |
| Kali Linux Preparation | Linux cybersecurity environment |
| TryHackMe | Windows Fundamentals learning |
| D: Drive | Prepared for VM storage |

---

## 🏗️ Intended SOC Lab Architecture

```text
                    ┌─────────────────────┐
                    │    Windows Host     │
                    │                     │
                    │  ┌───────────────┐  │
                    │  │    Splunk     │  │
                    │  │     SIEM      │  │
                    │  └───────────────┘  │
                    └──────────┬──────────┘
                               │
                               │
                    ┌──────────▼──────────┐
                    │     VirtualBox      │
                    └──────────┬──────────┘
                               │
                    ┌──────────▼──────────┐
                    │      Linux VM       │
                    │    Kali / Ubuntu    │
                    └─────────────────────┘