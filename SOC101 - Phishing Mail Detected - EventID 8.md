# SOC Investigation Report: Phishing Mail Detected (Event ID: 59)

## 1. Executive Summary
- **Case ID:** 59
- **Date/Time:** February 14, 2021, 03:00 AM
- **Severity:** Low
- **Verdict:** True Positive (TP)

This report covers the investigation of a suspicious email alert. The analysis confirmed that the email was a scam attempt targeting an internal user. The threat was successfully identified and handled by the email security system.

---

## 2. Detection Phase
The investigation began with an automated alert in the SIEM monitoring tab.

### Initial Alert Details:
- **Event Time:** 14/2/2021 3:00 AM
- **SMTP Address:** 27.128.173.81
- **Source Address:** `hahaha@ihackedyourcomputer.com`
- **Destination Address:** `mark@letsdefend.io`

> ![alert](screenshots/Screenshot1)

---

## 3. Investigation & Analysis
Following the detection, I performed a deep dive into the email security logs to retrieve the actual message sent to the user.

### Email Security Search
I navigated to the **Email Security** tab and performed a search using the SMTP address `27.128.173.81`. This search successfully located the email in question.

> ![email](screenshots/Screenshot2)

### Content Inspection
I reviewed the raw content of the email to determine the sender's intent:
- **Is the content suspicious?** Yes. The sender's address and the language used were characteristic of a scam.
- **Attachments:** None found.
- **URLs/Links:** None found.

Despite the lack of a technical payload (malicious link or file), the email body itself was malicious in nature, representing a "scam" or "extortion" attempt.

---

## 4. Final Verdict & Conclusion
Based on the investigation, the alert is classified as a **True Positive**.

### Reasoning:
The email was a clearly identified scam. The investigation confirmed that the email security system properly flagged the message, preventing any potential social engineering impact on the user.

### Artifacts Identified:
| Type | Value |
| :--- | :--- |
| **Sender IP (SMTP)** | 27.128.173.81 |
| **Sender Email** | hahaha@ihackedyourcomputer.com |
| **Recipient** | mark@letsdefend.io |

---
