# Task 17 — Hands-on Investigation Report

**Student:** Mudasir Zia  
**Task:** Task 17 — Hands-on Investigation (LetsDefend / CyberDefenders)  
**Focus:** SOC alert investigation, Windows investigation, blue-team practice  
**Evidence date:** September 24, 2026  
**Submission format:** PDF

---

## 1. Objective

The objective of this task was to perform practical blue-team/SOC investigation work using a platform such as LetsDefend or CyberDefenders, investigate logs/indicators/timeline information, reach an alert verdict, and document the work. The task also required completion of at least one compulsory free TryHackMe blue-team room.

This submission documents the hands-on work for which screenshot evidence was supplied.

---

## 2. Platforms and Tools

- **LetsDefend** — SOC monitoring and blue-team challenge practice.
- **TryHackMe** — Investigating Windows room.
- **Windows investigation concepts** — event/log investigation and attacker activity analysis.
- **PowerShell analysis concepts** — Base64-encoded script analysis.

---

## 3. LetsDefend Monitoring Evidence

The LetsDefend Monitoring page was accessed successfully.

The captured screenshot shows:

- Main Channel
- Investigation Channel
- Closed Alerts
- Alert severity
- Alert dates/timestamps
- Rule names
- Event IDs
- Alert types
- Investigation/action controls

Examples visible in the supplied screenshot include alerts relating to EDR tampering, a WinRAR vulnerability, privilege escalation, Apache Tomcat exploitation, Windows shortcut exploitation, phishing, and other security events.

**Evidence:** `Report/Screenshots/letsdefend.png`

> Note: The screenshot is evidence of the monitoring queue/interface. It does not by itself prove that a particular alert was opened, investigated to completion, or assigned a final verdict.

---

## 4. TryHackMe — Investigating Windows

The compulsory blue-team practice requirement was completed using the **Investigating Windows** room.

The supplied screenshot shows:

- Room title: **Investigating Windows**
- Room completion: **100%**
- Task 1 marked as completed
- The room's Windows investigation scenario

The room teaches investigation of a compromised Windows machine and focuses on finding clues about attacker activity.

**Evidence:** `Report/Screenshots/letsdefend1.png`

---

## 5. LetsDefend — PowerShell Script Challenge

An additional LetsDefend blue-team challenge was completed:

**Challenge:** PowerShell Script

The challenge description states that the analyst encounters a Base64-encoded PowerShell script that appears suspicious and must dissect and analyze it to understand its true nature and potential risks.

The screenshot confirms:

- Challenge name: **PowerShell Script**
- Required tool: CyberChef
- Challenge file path shown by the platform
- The challenge was completed successfully.

**Evidence:** `Report/Screenshots/letsdefend2.png`  
**Completion proof:** `Report/Screenshots/letsdefend3.png`

---

## 6. Investigation Methodology

A practical SOC analyst would normally investigate an alert using the following workflow:

1. **Validate the alert**
   - Identify the detection rule.
   - Check severity and alert type.
   - Confirm the affected host/user.

2. **Collect evidence**
   - Review Windows/SIEM logs.
   - Extract source and destination IPs.
   - Identify usernames, processes, files, domains, and hashes.
   - Record timestamps.

3. **Build a timeline**
   - Establish the first observed event.
   - Correlate related events before and after the detection.
   - Look for authentication, process execution, persistence, and network activity.

4. **Investigate IOCs**
   - Check IP addresses, domains, URLs, hashes, filenames, and processes.
   - Compare indicators with threat-intelligence sources when available.

5. **Determine impact**
   - Identify the affected endpoint/account.
   - Determine whether malicious activity actually occurred.
   - Identify evidence of persistence, privilege escalation, lateral movement, or data access.

6. **Make a verdict**
   - **True Positive:** evidence supports genuine malicious/suspicious activity.
   - **False Positive:** the detection was triggered by legitimate/benign activity.
   - **Escalate:** additional investigation or higher-tier response is required.

7. **Document and close**
   - Record evidence and reasoning.
   - Apply the appropriate containment/remediation action when required.
   - Close or escalate the case.

---

## 7. Evidence-Based Findings

| Area | Verified finding |
|---|---|
| LetsDefend access | Monitoring interface was accessed and screenshot captured. |
| SOC alerts | Multiple alert records are visible in the Monitoring queue. |
| TryHackMe | Investigating Windows room shows 100% completion. |
| LetsDefend challenge | PowerShell Script challenge was completed. |
| PowerShell analysis | Challenge involved investigation of a Base64-encoded PowerShell script. |
| Individual alert investigation | Not visible in supplied screenshots. |
| Alert IOC list | Not captured in supplied screenshots. |
| Alert timeline | Not captured in supplied screenshots. |
| Final TP/FP verdict | Not captured in supplied screenshots. |

---

## 8. Verdict / Case Disposition

### Evidence status

The supplied evidence is sufficient to verify platform access, blue-team practice, TryHackMe completion, and LetsDefend PowerShell challenge completion.

However, the supplied screenshots do **not** contain the detailed investigation page for one specific LetsDefend alert or the final True Positive/False Positive decision.

For accuracy, **no unsupported True Positive or False Positive verdict is fabricated in this report**.

### Correct SOC handling

For a real alert, the analyst should only close the case after reviewing the underlying logs/IOCs and documenting the evidence supporting the verdict. If the available evidence is insufficient, the appropriate operational action is to continue investigation or escalate rather than guess.

---

## 9. Practical Skills Demonstrated

This task provided hands-on exposure to:

- SOC monitoring interfaces
- Alert severity and categorization
- Event ID awareness
- Windows investigation workflow
- Blue-team challenge environments
- PowerShell security analysis
- Base64 decoding/analysis concepts
- Evidence collection
- Timeline-based investigation methodology
- True Positive / False Positive decision criteria
- SOC documentation and escalation concepts

---

## 10. Evidence Index

### Screenshot 1 — LetsDefend Monitoring

`Report/Screenshots/letsdefend.png`

Shows the LetsDefend SOC Monitoring queue and visible alert records.

### Screenshot 2 — TryHackMe Investigating Windows

`Report/Screenshots/letsdefend1.png`

Shows the Investigating Windows room at 100% completion.

### Screenshot 3 — LetsDefend PowerShell Script

`Report/Screenshots/letsdefend2.png`

Shows the PowerShell Script challenge and its investigation instructions.

### Screenshot 4 — PowerShell Script Completion

`Report/Screenshots/letsdefend3.png`

Shows completion of the PowerShell Script challenge on September 24, 2026.

---

## 11. Conclusion

Task 17 provided practical exposure to SOC and blue-team investigation environments. The completed evidence demonstrates use of LetsDefend, completion of the compulsory Investigating Windows practice room, and completion of an additional LetsDefend PowerShell analysis challenge.

The report intentionally distinguishes between **verified evidence** and **missing evidence**. A SOC investigation should never invent an IOC, timeline, or verdict when the underlying evidence has not been captured.

---

**Full report prepared for Task 17 submission.**
