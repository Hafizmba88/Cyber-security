# Security Analyst Study Notes

Concise, study-ready notes covering transferable and technical skills for security analysts. Use this as review material, flashcards, or to build labs.

## Overview
- Security analysts combine communication and collaboration skills with technical abilities (scripting, SIEM, forensics) to detect, investigate, and remediate threats while explaining risk to stakeholders.

## Transferable Skills

### Communication
- Explain threats, risks, and remediation steps to technical and non-technical audiences.
- Write clear incident summaries, tickets, and post-incident reports.
- Practice: Write a 1-paragraph executive summary for a simulated incident.
- Tip: Use the "so what / now what" format — state the impact, then the recommended action.

### Collaboration
- Coordinate with engineers, forensic teams, legal, and ops during incidents and projects.
- Assign and document ownership for containment and remediation tasks.
- Practice: Run a table-top incident response exercise and document roles.

### Analysis & Problem-Solving
- Triage alerts, form hypotheses, run tests, and determine root cause.
- Recommend automation, detection tuning, and process improvements.
- Practice: For an alert, list hypotheses, validation steps, and remediation steps.

## Technical Skills

### Programming (Python, SQL)
- Automate log parsing, enrichment, alerting, and ticket creation.
- Key topics: regex, file I/O, pandas for analysis, parameterized SQL queries.
- Practice: Build a Python script that ingests logs, filters suspicious activity, and outputs results.

### SIEM Tools
- Centralize telemetry, normalize logs, create correlation rules, and hunt for threats.
- Key topics: ingestion, parsing/normalization, correlation rules, dashboards, alert tuning.
- Practice: Import sample logs into Elastic SIEM or Splunk and create a detection for repeated failed logins.

### Computer Forensics
- Preserve and analyze evidence with proper chain-of-custody procedures.
- Key topics: disk/memory imaging, timeline analysis, artifact extraction (browser, OS logs), reporting.
- Practice: Use Autopsy or Volatility in a lab to create a timeline and short findings report.

## 4-Week Study Plan (adjustable)
- Week 1: Communication & Collaboration — write exec summary; run table-top IR.
- Week 2: Python for logs — parse logs, extract fields, script automations.
- Week 3: SQL + SIEM basics — practice SQL queries; create/tune SIEM detections.
- Week 4: Forensics basics — capture image/memory in a lab VM; analyze and report.

## Action Checklist
- [ ] Draft one incident executive summary
- [ ] Run a table-top incident response exercise
- [ ] Build a Python log parser (input → filter → output)
- [ ] Write 5 SQL queries for log analysis (top IPs, failed auths)
- [ ] Create and tune one SIEM detection rule
- [ ] Complete one small forensic lab (image + report)

## Study Resources
- Python: "Automate the Boring Stuff"; pandas docs
- SQL: Mode Analytics SQL tutorials, SQLite for practice
- SIEM: Elastic SIEM docs, Splunk tutorials
- Forensics: Autopsy, Volatility, SANS/DFIR blogs
- Practice: TryHackMe, Hack The Box, forensic CTF challenges

## Flashcards (Q/A)
- Q: Why is communication important for a security analyst?
  - A: To explain risk and remediation clearly to stakeholders and ensure correct action.
- Q: Name two scripting tasks a security analyst automates.
  - A: Log parsing for indicators; automated alert enrichment or ticket creation.
- Q: What is a SIEM used for?
  - A: Centralizing telemetry, correlating events, alerting on suspicious activity, and enabling threat hunting.
- Q: One quick way to reduce false positives in SIEM rules?
  - A: Add context/enrichment (asset owner, baseline behavior) and tune thresholds.
- Q: What is a key principle of digital forensics?
  - A: Preserve evidence integrity and maintain chain of custody.

## Quick Templates
- Executive summary (one-liner): "What happened: X. Impact: Y. Root cause: Z (if known). Containment: A. Next steps: B–C."
- Triage checklist (one-liner): "Validate → identify scope → capture artifacts → contain if needed → notify → remediate → document."

---

## Course 1 — Module 1: Terms & Definitions

- Cybersecurity (or security): The practice of ensuring confidentiality, integrity, and availability of information by protecting networks, devices, people, and data from unauthorized access or criminal exploitation.

- Cloud security: The process of ensuring that assets stored in the cloud are properly configured and access to those assets is limited to authorized users.

- Internal threat: A current or former employee, external vendor, or trusted partner who poses a security risk.

- Network security: The practice of keeping an organization's network infrastructure secure from unauthorized access.

- Personally identifiable information (PII): Any information used to infer an individual’s identity.

- Security posture: An organization’s ability to manage its defense of critical assets and data and react to change.

- Sensitive personally identifiable information (SPII): A specific type of PII that falls under stricter handling guidelines.

- Technical skills: Skills that require knowledge of specific tools, procedures, and policies.

- Threat: Any circumstance or event that can negatively impact assets.

- Threat actor: Any person or group who presents a security risk.

- Transferable skills: Skills from other areas that can apply to different careers.

---

Notes updated to include Course 1 Module 1 terms and definitions. Let me know if you want these moved to a separate file, shortened for flashcards, or turned into Anki export.
