# 🔐 Task 5 — Windows Logs & Event Viewer (Event IDs)

![Windows](https://img.shields.io/badge/Platform-Windows-blue?logo=windows)
![SOC](https://img.shields.io/badge/Domain-SOC%20Analysis-red)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![TryHackMe](https://img.shields.io/badge/Learning-TryHackMe-black?logo=tryhackme)

## 📌 Project Overview

This project documents practical learning related to Windows Event Viewer and Windows Security Event IDs. The work focuses on reviewing Security logs, filtering authentication events, and understanding how a SOC analyst investigates Windows logging activity.

## 🎯 Practical Learning Completed

- Explored Windows logging concepts.
- Accessed Windows Event Viewer.
- Navigated to **Windows Logs → Security**.
- Filtered Security events for **Event ID 4624**.
- Reviewed successful-logon event details.
- Studied important SOC-related Windows Event IDs.
- Documented the investigation workflow for Event ID 4625.

## 🧠 Core Topics

- Windows Event Viewer
- Windows Security Logs
- Event ID 4624 — Successful Logon
- Event ID 4625 — Failed Logon
- Event ID 4688 — Process Creation
- Event ID 4720 — User Account Created
- Event ID 4724 — Password Reset Attempt
- Authentication Event Analysis
- SOC Investigation Methodology

## 📂 Repository Structure

```text
Task5_Windows_Logs_Event_Viewer/
│
├── README.md
│
└── report/
    ├── report.md
    └── images/
        ├── windows-fundamentals-1.png
        ├── investigating-windows-machine.png
        ├── event-viewer-security-4624-filter.png
        └── event-id-4624-details.png
```

## 📊 Key Event IDs

| Event ID | Meaning |
|---|---|
| 4624 | Successful Logon |
| 4625 | Failed Logon |
| 4688 | Process Creation |
| 4720 | User Account Created |
| 4724 | Password Reset Attempt |

## 📝 Final Report

Full report: [report/report.md](report/report.md)

## ⚠️ Evidence Note

The current evidence documents Event Viewer and Event ID 4624 practical work. The task also requests analysis of an actual Event ID 4625 event; a captured 4625 screenshot should be added before final submission for the strongest possible grading evidence.
