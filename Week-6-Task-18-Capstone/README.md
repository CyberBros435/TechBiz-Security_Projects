# Week 6 — Task 18: Capstone Incident Investigation

## Full Incident Investigation & SOC Incident Report

**Intern:** Mudasir Zia  
**Task:** Week 6 — Task 18  
**Project Type:** Cybersecurity Capstone / SOC Incident Investigation  
**Scenario:** Suspicious / Obfuscated PowerShell Execution  
**Platform:** LetsDefend  
**Investigation Focus:** PowerShell Script Analysis, Evidence Review, MITRE ATT&CK Mapping, Incident Response

---

## Project Overview

This capstone project demonstrates an end-to-end SOC incident investigation based on a simulated suspicious PowerShell activity scenario.

The investigation focused on a PowerShell script containing Base64-encoded content and followed a structured incident-response workflow including:

- Detection and initial triage
- Evidence review
- Investigation timeline
- Suspicious PowerShell analysis
- Root cause assessment
- Impact assessment
- MITRE ATT&CK mapping
- Incident response recommendations
- Professional SOC incident reporting

The project was completed using the LetsDefend PowerShell Script challenge.

---

## Investigation Scenario

The scenario involved a suspicious PowerShell script containing Base64-encoded content.

Encoded PowerShell commands can conceal their actual functionality and may be used by attackers to execute commands while making initial analysis more difficult.

The investigation therefore focused on identifying the security significance of the PowerShell activity, understanding the obfuscation technique, determining relevant MITRE ATT&CK techniques, and defining appropriate SOC response actions.

---

## Investigation Objectives

The main objectives of this capstone were:

1. Investigate the suspicious PowerShell activity.
2. Identify the use of encoded/obfuscated content.
3. Review the available evidence.
4. Establish an investigation timeline.
5. Assess the potential root cause.
6. Assess potential security impact.
7. Map observed behavior to MITRE ATT&CK.
8. Develop containment and remediation recommendations.
9. Document the investigation in a professional SOC incident report.

---

## Tools & Platforms

- LetsDefend
- PowerShell
- CyberChef
- MITRE ATT&CK
- SOC investigation methodology
- Windows security telemetry concepts

---

## MITRE ATT&CK Mapping

| Technique ID | Technique | Relevance |
|---|---|---|
| T1059.001 | Command and Scripting Interpreter: PowerShell | The investigation scenario centers on PowerShell execution. |
| T1027 | Obfuscated/Compressed Files and Information | The script contains Base64-encoded content. |
| T1140 | Deobfuscate/Decode Files or Information | Decoding the Base64 content is required to reveal the concealed script content. |

---

## Investigation Workflow

```text
Detection
   ↓
Initial Triage
   ↓
Evidence Review
   ↓
PowerShell / Base64 Analysis
   ↓
Timeline Construction
   ↓
Root Cause Assessment
   ↓
Impact Assessment
   ↓
MITRE ATT&CK Mapping
   ↓
Containment & Remediation
   ↓
Final Incident Report