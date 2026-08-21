# Week 1 — Task 2: Networking Basics for Defenders

![Cyber Security](https://img.shields.io/badge/Domain-Cyber%20Security-red)
![Task](https://img.shields.io/badge/Internship-Week%201%20%7C%20Task%202-blue)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## Project Overview

This project covers foundational networking knowledge from a **defender/SOC analyst perspective**.

The internship task required:

- Mapping the OSI 7-layer model and common protocols
- Creating a table of 10 common network ports
- Explaining the DNS resolution flow
- Comparing normal and suspicious traffic
- Completing the required networking learning activities with screenshot evidence

## Repository Structure

```text
Week-1-Task-2-Networking-Basics-for-Defenders/
│
├── README.md
├── Week-1-Task-2-Networking-Basics-for-Defenders.pdf
│
└── Report/
    ├── REPORT.md
    └── [all original screenshots]
```

The `Report/` folder contains the complete written report and the original evidence screenshots used in the final PDF.

## Practical Learning Completed

### TryHackMe Evidence

The required networking learning was completed using free-access material:

1. **What is Networking?** — completed.
2. **OSI Model requirement** — the listed OSI Model room was subscription-locked, so the free **Networking Concepts** room was used to study and complete the OSI model material.
3. **DNS requirement** — the listed DNS in Detail room was subscription-locked, so **Introductory Networking** was used for the DNS material, including the `dig`/DNS section.

Screenshots documenting both the completed learning and the subscription-lock situations are included in `Report/`.

## Core Topics

### OSI Model

The report maps all seven layers:

1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

### Common Ports

The report covers ten common ports, with special focus on:

- 22 — SSH
- 80 — HTTP
- 443 — HTTPS
- 53 — DNS
- 445 — SMB
- 3389 — RDP

### DNS

The report explains how a domain name is resolved through the DNS hierarchy, including the client, recursive resolver, root server, TLD server, and authoritative DNS server.

### Defender Perspective

The project connects networking concepts to defensive monitoring, including:

- IP addresses
- Ports
- TCP/UDP
- DNS
- HTTP/HTTPS
- SMB
- RDP
- Normal vs suspicious traffic

## Final Report

The complete internship report is:

**`Report/REPORT.md`**

The PDF version for submission is:

**`Week-1-Task-2-Networking-Basics-for-Defenders.pdf`**

## Note

All screenshots in this repository are the original evidence files supplied for this project. No screenshot filenames were changed.
