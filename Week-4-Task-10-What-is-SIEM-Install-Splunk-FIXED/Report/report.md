# Week 4 — Task 10: What is SIEM? + Install Splunk / Wazuh

## 1. Project Overview

This project covers the fundamentals of Security Information and Event Management (SIEM) and demonstrates access to a working Splunk-based SIEM environment.

A SIEM centralizes security-relevant logs and events from multiple sources, normalizes the information, correlates related activity, applies detection logic, generates alerts, and provides dashboards for security monitoring and investigation.

For this task, an existing local Splunk environment was reused instead of installing Wazuh alongside it. This avoided unnecessary RAM and storage consumption while preserving the already configured security lab.

![Working Splunk SIEM Interface](./w1.png)

## 2. Objectives

- Understand what SIEM means.
- Understand centralized log collection.
- Understand log normalization.
- Understand event correlation.
- Understand SIEM detection and alerting.
- Understand dashboards and reporting.
- Complete the TryHackMe Introduction to SIEM room.
- Access and verify a working SIEM dashboard.
- Document the practical work with screenshots.

## 3. What is SIEM?

SIEM stands for **Security Information and Event Management**.

A SIEM is a security solution that collects logs from different sources, standardizes the data, correlates events, detects potentially malicious activity, generates alerts, and presents information through dashboards and search interfaces.

Common sources include Windows Event Logs, Sysmon, Linux logs, firewall logs, IDS/IPS logs, DNS logs, web server logs, authentication systems, endpoint security products, and cloud services.

## 4. Core SIEM Functions

### 4.1 Centralized Log Collection

SIEM collects logs from endpoints, servers, firewalls, network devices, applications, and other security sources into a central platform. Centralization allows analysts to search and investigate information without manually checking every individual system.

### 4.2 Log Normalization

Different log sources use different formats and field names. Normalization converts the information into a consistent structure so that events can be searched, filtered, compared, and correlated more effectively.

### 4.3 Log Correlation

Correlation connects events from different sources and identifies relationships between them. For example, multiple failed logins followed by a successful authentication, suspicious process execution, and an outbound connection can become more meaningful when investigated together.

### 4.4 Detection and Alerting

Detection rules evaluate event data for suspicious conditions. When a rule matches, an alert can be generated so that a SOC analyst can investigate the activity.

### 4.5 Dashboards and Reporting

Dashboards provide a summarized view of security activity. They can display alerts, event counts, failed logins, system notifications, rules triggered, domains visited, and other security metrics.

## 5. Three Benefits of SIEM

### Benefit 1 — Centralized Visibility

A SIEM provides a single location where security events from multiple systems can be searched and investigated.

### Benefit 2 — Faster Threat Detection

Correlation and detection rules allow suspicious patterns to be identified more efficiently than manually reviewing separate log sources.

### Benefit 3 — Better Investigation and Reporting

Searchable event data, alerts, and dashboards provide analysts with evidence that can support investigation, escalation, incident response, and reporting.

## 6. Practical SIEM Used

### Splunk

Splunk was used as the SIEM platform for this practical task. An existing local Splunk environment was already installed and configured with security telemetry. Because available system resources were limited, a second SIEM installation was intentionally avoided.

This was a practical lab decision: the objective was to demonstrate a working SIEM rather than install two resource-intensive platforms simultaneously.

## 7. Setup and Verification

### Step 1 — Open the Existing Splunk Environment

The existing Splunk installation was opened in the browser.

### Step 2 — Access the Splunk Interface

The Splunk web interface loaded successfully and displayed the administrator interface.

### Step 3 — Verify the Working Dashboard

The Splunk interface was accessible and operational, providing evidence that the SIEM environment was working.

![Splunk Dashboard / Working Interface](./w1.png)

### Result

The Splunk SIEM environment was successfully accessed and verified without installing Wazuh or modifying the existing lab setup.

## 8. TryHackMe — Introduction to SIEM

The required TryHackMe Introduction to SIEM room was completed. The learning activity covered SIEM fundamentals, including log sources, centralized collection, normalization, correlation, alerting, dashboards, ingestion, and alert investigation.

![TryHackMe Introduction to SIEM — Evidence 1](./w2.png)

![TryHackMe Introduction to SIEM — Evidence 2](./w3.png)

The supplied screenshots show the room at 100% completion.

## 9. SIEM Workflow

```text
Log Sources
    ↓
Collection / Ingestion
    ↓
Parsing / Normalization
    ↓
Correlation
    ↓
Detection Rules
    ↓
Alert Generation
    ↓
SOC Analyst Investigation
    ↓
Response / Escalation
```

Each stage contributes to the SOC investigation process.

## 10. SOC Analyst Use Cases

A SOC analyst can use a SIEM to investigate:

- Failed authentication attempts
- Successful logins after repeated failures
- Suspicious process execution
- Malware indicators
- Privilege escalation
- Persistence activity
- Suspicious DNS requests
- Unusual network connections
- Possible data exfiltration
- Unauthorized administrative activity

SIEM data is most useful when events from multiple sources are correlated and investigated in context.

## 11. Practical Skills Demonstrated

| Skill | Demonstration |
|---|---|
| SIEM Fundamentals | Explained SIEM purpose and capabilities |
| Log Collection | Understood centralized ingestion of security logs |
| Normalization | Understood conversion of different log formats into consistent fields |
| Correlation | Understood relationships between events from multiple sources |
| Alerting | Understood how detection rules trigger alerts |
| Dashboard Usage | Accessed the working Splunk interface |
| SOC Investigation | Connected SIEM capabilities to practical analyst workflows |
| Documentation | Produced screenshots and a structured technical report |

## 12. Evidence Summary

The following evidence files are included with this report:

- `w1.png` — Working Splunk SIEM interface/dashboard.
- `w2.png` — TryHackMe Introduction to SIEM evidence.
- `w3.png` — TryHackMe Introduction to SIEM completion evidence.

## 13. Repository Structure

```text
Week-4-Task-10-What-is-SIEM-Install-Splunk/
│
├── README.md
├── Week-4-Task-10-What-is-SIEM-Install-Splunk.pdf
│
└── Report/
    ├── report.md
    ├── w1.png
    ├── w2.png
    └── w3.png
```

## 14. Resource-Constrained Lab Decision

Wazuh was not installed alongside the existing Splunk environment because the system did not have sufficient resources to safely operate another SIEM at the same time.

Instead, the already working Splunk environment was retained and used for the practical demonstration. This avoided deleting or rebuilding the existing SIEM configuration and reduced the risk of breaking the established lab.

This is a realistic lab-management decision: a SOC analyst should work with available infrastructure and avoid unnecessary changes to a functioning monitoring environment.

## 15. Conclusion

This project established the fundamentals of SIEM and demonstrated a working Splunk environment. The key concepts covered were centralized log collection, normalization, correlation, detection rules, alerting, dashboards, and SOC investigation.

The practical work also demonstrated how an existing SIEM installation can be reused when system resources are limited instead of deploying multiple SIEM platforms simultaneously.

## 16. Final Status

**Project:** Week 4 — Task 10: What is SIEM? + Install Splunk / Wazuh  
**Status:** Completed  
**SIEM Platform:** Splunk  
**Learning Activity:** TryHackMe — Introduction to SIEM  
**Practical Evidence:** Working Splunk interface + TryHackMe completion screenshots
