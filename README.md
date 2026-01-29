# SOC Investigation Reports: Phishing Analysis (LetsDefend)

## 🔍 Project Overview
[span_2](start_span)This repository contains technical documentation and incident response reports for real-world phishing alerts analyzed on the **LetsDefend** platform[span_2](end_span). Each case follows a structured investigation lifecycle: detection, technical analysis, log correlation, and remediation.

---

## 🛠️ Technical Skills Applied
- **[span_3](start_span)Email Security:** Identifying spoofed senders, header analysis, and malicious SMTP relays[span_3](end_span).
- **[span_4](start_span)Malware Analysis:** Analyzing suspicious attachments and URLs using VirusTotal and AnyRun[span_4](end_span).
- **[span_5](start_span)SIEM & Log Correlation:** Searching log management systems to confirm user interaction (clicks/downloads)[span_5](end_span).
- **[span_6](start_span)Incident Response:** Performing containment actions such as host isolation and email deletion[span_6](end_span).

---

## 📁 Investigated Cases
[span_7](start_span)This repository documents the investigation of the following four Exchange phishing alerts[span_7](end_span):

### 📧 [Event ID 59: Scam/Extortion Attempt](./SOC101%20-%20Phishing%20Mail%20Detected%20-%20EventID%2059.md)
- **[span_8](start_span)Summary:** Analysis of an extortion-based phishing email[span_8](end_span).
- **Outcome:** True Positive. No malicious payloads found; threat mitigated by system blocks.

### 📧 [Event ID 34: Netflix Phishing/Infection](./SOC101%20-%20Phishing%20Mail%20Detected%20-%20EventID%2034.md)
- **[span_9](start_span)Summary:** Investigation into a spoofed Netflix domain leading to a malicious IP[span_9](end_span).
- **Outcome:** True Positive. User interaction confirmed; device isolated.

### 📧 [Event ID 27: Malicious Link Detection](./SOC101%20-%20Phishing%20Mail%20Detected%20-%20EventID%2027.md)
- **[span_10](start_span)Summary:** Triage of a phishing email containing a malicious URL[span_10](end_span).
- **Outcome:** True Positive. Mail was delivered but not opened; email deleted.

### 📧 [Event ID 08: Malicious File Analysis](./SOC101%20-%20Phishing%20Mail%20Detected%20-%20EventID%2008.md)
- **[span_11](start_span)Summary:** Deep dive into a phishing email with a malicious file attachment[span_11](end_span).
- **Outcome:** True Positive. Infection confirmed via AnyRun and logs; device contained.

---

## 🛡️ Investigation Methodology
Every case in this repository followed these strict standards:
1. **[span_12](start_span)Evidence Collection:** Every step—from initial alert to final action—is documented with screenshots[span_12](end_span).
2. **[span_13](start_span)IOC Verification:** All IP addresses and domains were cross-referenced with VirusTotal or AnyRun[span_13](end_span).
3. **[span_14](start_span)Log Analysis:** Verification of user interaction was performed by correlating internal traffic with external malicious IPs[span_14](end_span).
4. **[span_15](start_span)Remediation:** Actions included email deletion and host isolation via the Endpoint Security tab[span_15](end_span).

---
*[span_16](start_span)Note: All data within these reports is based on simulated environments provided by LetsDefend for training purposes[span_16](end_span).*
