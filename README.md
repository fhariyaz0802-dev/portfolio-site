
# Fhariyazunnisa Abdul

### Cybersecurity Portfolio | Aspiring SOC Analyst

**M.S. in Management Information Systems**  
Auburn University at Montgomery | May 2026

Welcome to my cybersecurity portfolio!

I am an aspiring SOC Analyst with a Master's degree in Management Information Systems and a strong interest in security operations, threat detection, incident investigation, and log analysis.

This portfolio showcases my hands-on cybersecurity projects, technical skills, investigation methodologies, and security documentation.

---

## Cybersecurity Projects

### 1. Splunk SOC Brute-Force Detection

**Tools:** Splunk Enterprise, SPL, Windows Authentication Logs

**Project Overview:**

Developed a hands-on SOC monitoring project focused on detecting suspicious authentication activity using Splunk.

**Key Activities:**
- Analyzed failed login events using Windows Event ID 4625.
- Investigated suspicious source IP addresses and targeted accounts.
- Developed SPL queries to identify repeated failed authentication attempts.
- Created a Splunk monitoring dashboard.
- Implemented a five-minute threshold-based detection.
- Documented investigation findings and detection results.

**Skills Demonstrated:**
- SIEM Monitoring
- Splunk Search Processing Language (SPL)
- Security Log Analysis
- Brute-Force Detection
- SOC Investigation

[View Splunk SOC Project](https://github.com/fhariyaz0802-dev/Splunk-SOC-Brute-Force-Detection)

---

### 2. Microsoft Sentinel SOC Monitoring & Brute-Force Detection

**Tools:** Microsoft Sentinel, Azure Log Analytics, Kusto Query Language (KQL), Simulated Windows Security Events

**Project Overview:**

Developed a hands-on SOC investigation project using Microsoft Sentinel and KQL to detect simulated brute-force authentication activity and investigate a successful login following multiple failed attempts.

**Key Activities:**
- Configured an Azure Log Analytics workspace and enabled Microsoft Sentinel.
- Created simulated Windows authentication events using KQL `datatable`.
- Analyzed failed authentication attempts using Windows Event ID 4625.
- Detected six failed login attempts targeting the `admin` account from IP address `192.0.2.10`.
- Investigated authentication timestamps and login patterns.
- Correlated failed authentication events with a successful login using Event ID 4624.
- Used KQL `join`, `summarize`, and time-based filtering to identify suspicious authentication sequences.
- Created a professional SOC incident investigation report.
- Documented detection queries and investigation screenshots on GitHub.

**Investigation Findings:**
- Affected Account: `admin`
- Source IP: `192.0.2.10` (test/documentation IP)
- Failed Login Attempts: 6
- First Failed Login: 10:00 UTC
- Last Failed Login: 10:05 UTC
- Successful Login: 10:06 UTC
- Assessment: Suspicious authentication pattern in simulated data; no actual compromise established.

**Skills Demonstrated:**
- Microsoft Sentinel
- Azure Log Analytics
- Kusto Query Language (KQL)
- SIEM Monitoring
- Authentication Event Correlation
- Brute-Force Pattern Detection
- Incident Investigation
- SOC Incident Reporting

**Project Deliverables:**
- KQL detection queries
- Microsoft Sentinel investigation screenshots
- SOC incident investigation report
- GitHub project documentation

[View Microsoft Sentinel SOC Project](https://github.com/fhariyaz0802-dev/Microsoft-Sentinel-SOC-Detection)

**Note:** This project uses simulated authentication events rather than live production security logs.

---

### 3. Windows Security Monitoring Lab

**Tools:** Windows 11, Sysmon, Windows Event Viewer

**Project Overview:**

Explored Windows security monitoring techniques to investigate system activity, authentication events, and suspicious processes.

**Key Activities:**
- Configured a Windows 11 virtual machine.
- Analyzed Windows security and Sysmon events.
- Investigated process creation and login activity.

**Skills Demonstrated:**
- Windows Event Viewer
- Endpoint Monitoring
- Sysmon
- Security Event Analysis

---

### 4. Threat Hunting with Wireshark

**Tools:** Wireshark, DNS, Packet Analysis

**Project Overview:**

Performed network traffic analysis to identify suspicious communication patterns and investigate potential security indicators.

**Key Activities:**
- Captured and analyzed network traffic.
- Investigated suspicious DNS query patterns.
- Examined network packets for unusual activity.
- Documented findings and potential security indicators.

**Skills Demonstrated:**
- Network Traffic Analysis
- Wireshark
- DNS Investigation
- Threat Hunting

---

### 5. Phishing Email Analysis

**Tools:** VirusTotal, SPF, DKIM, DMARC

**Project Overview:**

Investigated suspicious email characteristics to identify potential phishing indicators and email spoofing attempts.

**Key Activities:**
- Analyzed suspicious email headers.
- Identified spoofed sender domains.
- Investigated suspicious URLs and IP addresses.
- Documented indicators of compromise.

**Skills Demonstrated:**
- Phishing Investigation
- Email Security
- Threat Intelligence
- Indicator Analysis

---

### 6. Credit Card Fraud Detection

**Tools:** Python, Pandas, NumPy, Scikit-learn, Tkinter

**Project Overview:**

Co-developed a machine learning system designed to identify potentially fraudulent credit card transactions.

**Key Activities:**
- Analyzed over 284,000 anonymized transactions.
- Performed data preprocessing and exploratory analysis.
- Trained a Random Forest/CART classifier.
- Developed a Tkinter interface for predictions.

**Skills Demonstrated:**
- Python Programming
- Data Analysis
- Machine Learning
- Fraud Detection
- Scikit-learn

---

## Technical Skills

**SIEM & Security Monitoring**
- Microsoft Sentinel
- Splunk
- Kusto Query Language (KQL)
- Search Processing Language (SPL)
- Security Event Monitoring
- Authentication Log Analysis

**Cybersecurity & SOC**
- Security Operations Center (SOC) Fundamentals
- Threat Detection
- Brute-Force Pattern Detection
- Incident Investigation
- Security Event Correlation
- Incident Documentation
- Phishing Analysis

**Network Security**
- Wireshark
- DNS Analysis
- Network Traffic Analysis
- Packet Inspection
- Network Security Fundamentals

**Endpoint & Operating Systems**
- Windows Security Event Viewer
- Sysmon
- Windows Authentication Events
- Windows 11

**Cloud & Security Platforms**
- Microsoft Azure
- Azure Log Analytics
- Microsoft Sentinel

**Programming & Data Analysis**
- Python
- Pandas
- NumPy
- Scikit-learn
- SQL Fundamentals

**Documentation & Version Control**
- GitHub
- Markdown
- SOC Incident Reporting
- Technical Documentation

---

## Education

### Auburn University at Montgomery
**Master of Science in Management Information Systems**  
Graduated: May 2026

### SRK Institute of Technology
**Bachelor of Technology in Computer Science Engineering**  
Graduated: April 2023

---

## Career Objective

Seeking an entry-level SOC Analyst or Cybersecurity Analyst opportunity where I can apply my hands-on experience with SIEM monitoring, KQL, SPL, authentication log analysis, threat detection, and incident investigation.

I am committed to continuously developing practical cybersecurity skills through hands-on labs, security projects, and technical learning.

---

## Connect With Me

**LinkedIn:**  
[linkedin.com/in/fhariyazunnisa-abdul](https://www.linkedin.com/in/fhariyazunnisa-abdul)

**GitHub:**  
[github.com/fhariyaz0802-dev](https://github.com/fhariyaz0802-dev)

**Cybersecurity Portfolio Website:**  
[View My Portfolio](https://fhariyaz0802-dev.github.io/portfolio-site/)

---

*Thank you for visiting my cybersecurity portfolio!*




