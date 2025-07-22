# Insider Threat detection lab with Splunk

This project shows a real world insider htreat senario in Splunk. It detects suspicious user actions such as data exfilteration Via email/USB, unauthorized file deletion, and unusual access patterns — all visualized through custom SPL queries and a dark-themed Splunk dashboard.

---
## Objectives

- Simulate internal threat with a custom audit log
- Detect exfiltration, deletion, and misuse of sensitive data
- Build SPL queries and visualise results in splunk
- Align detection with MITRE ATT&CK techniques

---

# Dashboard Panels 

- File Exfilteration Events- detects upload and email
- User Action Summary- Stats count by user, action
- Timeline of Events-Sorted_time for misuse analysis


# MITRE ATT&CK Mapping 

- USB/email exfiltrationc - Technique: Exfiltration over physical media, ID: T1052.001
- File deletion - Technique: Indicator removal on host, ID: T1070.004
- Sensitive file access - Technique: Data from local system, ID: T1005

# How to run 
1 Open Splunk at http://localhost:8000
2 Upload audit_log_simulated.log via Add Data
3 set sourcetype: custom_audit
4 Use default index: main
5 Import insider_dashboard.xml under classic dashboards
6 set time Range to All Time to see results

# Skills Shown:

Splunk,Insider Threat Analysis, MITRE ATT&CK mapping , SOC-level detection skills

