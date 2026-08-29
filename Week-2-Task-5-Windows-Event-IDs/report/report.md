# Task 5 — Windows Logs & Event Viewer (Event IDs)

## Project Overview

This task focused on the fundamentals of Windows logging and Event Viewer from a SOC analyst perspective. The practical objective was to inspect Windows Security logs, filter events by Event ID, and understand how authentication activity can be investigated.

## Learning Resources

- TryHackMe — Windows Fundamentals 1
- TryHackMe — Investigating Windows

## Practical Work Performed

The following practical activities were documented:

1. Accessed the Windows environment used for investigation.
2. Opened **Windows Event Viewer**.
3. Navigated to **Windows Logs → Security**.
4. Filtered the Security log for **Event ID 4624**.
5. Reviewed the resulting successful-logon events.
6. Opened an Event ID 4624 record and inspected its properties.

### Evidence

![Windows Fundamentals 1](images/windows-fundamentals-1.png)

![Investigating Windows Environment](images/investigating-windows-machine.png)

![Event Viewer — Security Log Filtered for Event ID 4624](images/event-viewer-security-4624-filter.png)

![Event ID 4624 Details](images/event-id-4624-details.png)

## Five Important Windows Event IDs

| Event ID | Meaning | SOC Relevance |
|---|---|---|
| **4624** | Successful logon | Helps analysts establish normal authentication activity and investigate access. |
| **4625** | Failed logon | Can indicate incorrect credentials, password guessing, brute-force activity, or unauthorized access attempts. |
| **4688** | Process creation | Useful for identifying suspicious executables and reconstructing attacker activity. |
| **4720** | User account created | Important for detecting unauthorized account creation and persistence. |
| **4724** | Password reset attempt | Useful when investigating account manipulation and possible privilege abuse. |

## Event ID 4624 Analysis

**Event ID:** 4624  
**Category:** Logon  
**Meaning:** A logon was successfully completed.

The captured Event Viewer evidence shows the Security log filtered for Event ID 4624. The event details identify the record as a successful logon and include fields that can be useful during an investigation, including:

- Account information
- Security identifier
- Logon identifier
- Log source
- Event timestamp
- Computer name
- Audit keywords

### SOC Analyst Perspective

A successful logon is not automatically suspicious. A SOC analyst should compare the event against the expected user, time, workstation, logon type, and source information. A successful authentication may become suspicious when it occurs from an unusual location, at an unusual time, after multiple failed logons, or with an unexpected account.

## Event ID 4625 Investigation Methodology

**Important evidence note:** The uploaded screenshots document Event ID 4624 but do not contain a captured Event ID 4625 record. Therefore, this section describes the correct SOC investigation workflow and should not be interpreted as evidence of a specific captured failed-logon event.

When investigating Event ID 4625, the analyst should record:

| Field | Investigation Use |
|---|---|
| Event ID | Confirms the event is a failed logon (4625). |
| Time Created | Establishes when the authentication failure occurred. |
| Account Name | Identifies the account being targeted. |
| Logon Type | Shows the type of authentication attempt. |
| Failure Reason | Helps determine why authentication failed. |
| Workstation Name | Identifies the involved host when available. |
| Source Network Address | Helps identify the source of remote activity when available. |

### What a SOC Analyst Should Determine

1. **What happened?** — An authentication attempt failed.
2. **Which account was targeted?** — Review the account name in the event.
3. **When did it happen?** — Review the event timestamp.
4. **Why did it fail?** — Review the failure reason and status/sub-status fields.
5. **Is it suspicious?** — Compare the event with surrounding activity. Repeated failures, many targeted accounts, unusual sources, or failures followed by a successful logon may require escalation.

## Key Takeaways

- Windows Event Viewer is a core tool for reviewing endpoint activity.
- The Security log provides valuable authentication and account-related events.
- Event ID 4624 records successful logons.
- Event ID 4625 is important for detecting failed authentication activity and potential password attacks.
- Event IDs such as 4688 and 4720 can provide valuable evidence during threat investigations.

## Evidence Limitation

The current uploaded evidence supports the Event Viewer and Event ID 4624 practical work. A screenshot of an actual Event ID 4625 record is still required to fully satisfy the task's requested “one analyzed 4625 event” evidence requirement. Adding that screenshot and replacing the methodology section with the real event values would make the submission stronger and more complete.
