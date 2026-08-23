
---

# 2. `Report/REPORT.md`

Copy this entire file inside the **Report folder**:

```markdown
# 🔐 Week 1 · Task 3 — Lab Setup Report

## VirtualBox + Kali/Ubuntu + Windows Environment

---

# 📌 1. Introduction

This report documents the practical work completed for **Week 1 · Task 3 — Lab Setup**.

The purpose of this task was to understand and begin building a basic Security Operations Center (SOC) laboratory environment using virtualization.

A SOC lab is useful because it provides a controlled environment where security professionals can practice:

- System administration
- Networking
- Log analysis
- Security monitoring
- SIEM operations
- Incident investigation

The assigned task required VirtualBox, a Linux environment, a Windows environment, internal networking, connectivity testing, and completion of the TryHackMe Windows Fundamentals 1 room.

---

# 🎯 2. Task Objectives

The objectives of this project were:

1. Install Oracle VirtualBox.
2. Prepare a Kali Linux or Ubuntu environment.
3. Prepare a Windows environment for analysis.
4. Configure an internal network.
5. Test connectivity between lab systems.
6. Complete TryHackMe Windows Fundamentals 1.
7. Document the practical work with screenshots.

---

# 🎓 3. TryHackMe — Windows Fundamentals 1

The required TryHackMe room was completed as part of this project.

The room provided learning related to Windows fundamentals and concepts relevant to cybersecurity and security operations.

## Screenshot Evidence

### TryHackMe Evidence 1

![TryHackMe Screenshot 1](t1.png)

### TryHackMe Evidence 2

![TryHackMe Screenshot 2](t2.png)

### TryHackMe Evidence 3

![TryHackMe Screenshot 3](t3.png)

### TryHackMe Evidence 4

![TryHackMe Screenshot 4](t4.png)

### TryHackMe Evidence 5

![TryHackMe Screenshot 5](t5.png)

### TryHackMe Evidence 6

![TryHackMe Screenshot 6](t6.png)

---

# 🖥️ 4. VirtualBox Installation

Oracle VirtualBox was installed on the Windows host system.

VirtualBox provides a virtualization platform that allows multiple operating systems to run as virtual machines on the same physical computer.

This is important for cybersecurity because security professionals often require separate environments for:

- Linux security tools
- Windows analysis
- Malware analysis
- Network testing
- Log generation
- SOC monitoring

## Screenshot Evidence

### VirtualBox Installation

![VirtualBox Evidence](t7.png)

### VirtualBox Setup

![VirtualBox Evidence](t8.png)

---

# 💾 5. Virtual Machine Storage Preparation

The system had limited available storage on the main C: drive.

Because of this limitation, the VirtualBox machine storage location was prepared on the D: drive.

This helps prevent virtual machine files from consuming the limited free space available on the Windows system drive.

## Screenshot Evidence

### VirtualBox Storage Configuration

![Storage Configuration](t10.png)

### Virtual Machine Storage Preparation

![Storage Preparation](t11.png)

### Additional VirtualBox Configuration Evidence

![VirtualBox Configuration](t12.png)

### Additional Evidence

![VirtualBox Evidence](t15.png)

---

# 🌐 6. Windows Network Information

The Windows host network configuration was reviewed using the following command:

```cmd
ipconfig
