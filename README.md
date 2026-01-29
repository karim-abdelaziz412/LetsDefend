# SOC Investigation Reports: Phishing Analysis (LetsDefend)

## Project Overview
This repository contains technical documentation and incident response reports for real-world phishing alerts analyzed on the LetsDefend platform. Each case follows a structured investigation lifecycle: detection, technical analysis, log correlation, and remediation.

---

## Technical Skills Applied
- **Email Security:** Identifying spoofed senders, header analysis, and malicious SMTP relays.
- **Malware Analysis:** Analyzing suspicious attachments and URLs using VirusTotal and AnyRun.
- **SIEM & Log Correlation:** Searching log management systems to confirm user interaction.
- **Incident Response:** Performing containment actions such as host isolation and email deletion.

---

## Investigated Cases

### [Event ID 59: Scam/Extortion Attempt](SOC101%20-%20Phishing%20Mail%20Detected%20-%20EventID%2059.md)
- **Summary:** Analysis of an extortion-based phishing email.
- **Outcome:** True Positive. No malicious payloads found; threat mitigated by system blocks.

### [Event ID 34: Netflix Phishing/Infection](SOC101%20-%20Phishing%20Mail%20Detected%20-%20EventID%2034.md)
- **Summary:** Investigation into a spoofed Netflix domain leading to a malicious IP.
- **Outcome:** True Positive. User interaction confirmed via logs; device isolated.

### [Event ID 27: Malicious Link Detection](SOC101%20-%20Phishing%20Mail%20Detected%20-%20EventID%2027.md)
- **Summary:** Triage of a phishing email containing a malicious URL.
- **Outcome:** True Positive. Mail was delivered but not opened; email deleted.

### [Event ID 08: Malicious File Analysis](SOC101%20-%20Phishing%20Mail%20Detected%20-%20EventID%208.md)
- **Summary:** Deep dive into a phishing email with a malicious file attachment.
- **Outcome:** True Positive. Infection confirmed via AnyRun and logs; device contained.

---

## Investigation Methodology
Every case in this repository followed these strict standards:
1. **Evidence Collection:** Every step is documented with screenshots.
2. **IOC Verification:** All IP addresses and domains were cross-referenced with VirusTotal or AnyRun.
3. **Log Analysis:** Verification of user interaction was performed by correlating internal traffic with external malicious IPs.
4. **Remediation:** Actions included email deletion and host isolation via the Endpoint Security tab.

---
*Note: All data within these reports is based on simulated environments provided by LetsDefend for training purposes.*
