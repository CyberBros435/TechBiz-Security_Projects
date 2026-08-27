# Week 2 — Task 4: Linux Basics + Log Files (/var/log)

![Cyber Security](https://img.shields.io/badge/Domain-Cyber%20Security-red)
![Task](https://img.shields.io/badge/Internship-Week%202%20%7C%20Task%204-blue)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## Project Overview

This project covers foundational Linux knowledge and log analysis from a **defender/SOC analyst perspective**.

The internship task required:

- Practicing basic Linux commands
- Navigating the Linux file system
- Exploring `/var/log`
- Viewing log files with `cat`
- Inspecting recent events with `tail`
- Understanding live log monitoring with `tail -f`
- Searching log content with `grep`
- Understanding failed-login searches
- Completing the required TryHackMe learning activities
- Documenting practical work with screenshot evidence

## Repository Structure

```text
Week-2-Task-4-Linux-Basics-Log-Files/
│
├── README.md
├── Week-2-Task-4-Linux-Basics-Log-Files.pdf
│
└── Report/
    ├── REPORT.md
    └── l1.png
    └── l2.png
    └── l3.png
    └── l4.png
    └── l5.png
    └── l6.png
    └── l7.png
    └── l8.png
    └── l9.png
    └── l10.png
    └── l11.png
    └── l12.png
    └── l13.png
    └── l14.png
    └── l15.png
    └── l16.png
    └── l17.png
    └── l18.png
```

The `Report/` folder contains the complete written report and the original evidence screenshots used in the final PDF.

## Practical Learning Completed

### TryHackMe Evidence

The following required learning activities were completed:

1. **Linux Fundamentals Part 1**
2. **Intro to Logs**

Screenshots documenting the completed learning and practical activities are included in the `Report/` folder.

## Core Linux Commands

The project covers the following commands:

```bash
pwd
ls
cd
cat
tail
tail -f
grep
```

### `/var/log`

The `/var/log` directory is an important Linux location for system and application logs.

From a SOC perspective, logs can provide evidence about:

- User activity
- Authentication events
- Failed login attempts
- Service activity
- Errors
- Commands and processes
- Suspicious behaviour

### `cat`

Used to display the contents of a file:

```bash
cat <log-file>
```

### `tail`

Used to inspect recent entries:

```bash
tail <log-file>
tail -n 20 <log-file>
```

### `tail -f`

Used to monitor new entries as they are written:

```bash
tail -f <log-file>
```

### `grep`

Used to search for specific patterns:

```bash
grep 'Failed' auth.log
```

## Defender Perspective

This project connects Linux fundamentals with practical SOC work.

The skills practiced are useful for:

- Security monitoring
- Log investigation
- Authentication analysis
- Incident response
- Threat hunting
- Troubleshooting
- SIEM and centralised logging

## Final Report

The complete internship report is:

Full report: [report/report.md](report/report.md)

The PDF version for submission is:

**`Week-2-Task-4-Linux-Basics-Log-Files.pdf`**

## Note

All screenshots in this repository are the original evidence files supplied for this project. No screenshot filenames were changed.
