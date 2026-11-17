# Splunk SOC Monitoring & Brute-Force Detection

## Project Overview

This project demonstrates a hands-on Security Operations Center (SOC) monitoring workflow using Splunk Enterprise.

The objective was to analyze Windows authentication logs, identify suspicious failed login activity, investigate potential brute-force attacks, and create a security monitoring dashboard.

**Project Type:** Cybersecurity Home Lab  
**Platform:** Splunk Enterprise 10.6.1  
**Log Source:** CSV-based Windows authentication event dataset  
**Focus:** SOC Monitoring, Log Analysis, Threat Detection, Incident Investigation

## Tools and Technologies

- Splunk Enterprise
- Splunk Search Processing Language (SPL)
- Windows Security Event ID 4625
- CSV Log Analysis
- Security Dashboard Visualization
- Brute-Force Detection

## Project Objectives

1. Import and analyze Windows authentication logs.
2. Identify failed login attempts using Event ID 4625.
3. Investigate suspicious source IP addresses.
4. Analyze failed login activity over time.
5. Compare successful and failed login events.
6. Identify potential brute-force attack patterns.
7. Create a centralized SOC monitoring dashboard.

## SPL Queries Used

### 1. Investigate Failed Login Events

```spl
index=main sourcetype=csv EventCode=4625
| table _time Account_Name Source_Network_Address Login_Status ComputerName
```

This query displays authentication event timestamps, usernames, source IP addresses, login status, and affected computers.

### 2. Identify Source IPs with Failed Login Attempts

```spl
index=main sourcetype=csv EventCode=4625
| stats count as Failed_Attempts by Source_Network_Address
| sort - Failed_Attempts
```

**Results:**

| Source IP | Failed Attempts |
|---|---:|
| 192.168.1.50 | 12 |
| 192.168.1.77 | 8 |
| 192.168.1.88 | 6 |
| 192.168.1.60 | 5 |

The IP address `192.168.1.50` generated the highest number of failed login attempts.

### 3. Analyze Failed Login Attempts Over Time

```spl
index=main sourcetype=csv EventCode=4625
| timechart span=5m count as Failed_Logins
```

This query visualizes failed authentication events in five-minute intervals to identify suspicious spikes.

### 4. Detect Potential Brute-Force Activity

```spl
index=main sourcetype=csv EventCode=4625
| bin _time span=5m
| stats count as Failed_Attempts by _time Source_Network_Address Account_Name
| where Failed_Attempts >= 5
| sort - Failed_Attempts
```

The query identifies source IP and account combinations generating five or more failed login attempts within a five-minute interval.

This threshold is a demonstration detection rule and should be tuned for real environments.

## SOC Security Monitoring Dashboard

The dashboard contains four security monitoring panels:

- **Failed Login Attempts by Source IP:** Identifies IP addresses generating repeated authentication failures.
- **Failed Login Attempts Over Time:** Visualizes authentication failure spikes.
- **Successful vs Failed Login Attempts:** Compares authentication outcomes.
- **Potential Brute-Force Attack Detection:** Displays suspicious authentication patterns meeting the configured threshold.

### Dashboard Screenshot

![SOC Monitoring Dashboard](SOC%20Dashboard.png)

### Failed Login Events

![Failed Login Events](01-Failed-Login-Events.png)

### Failed Logins by Source IP

![Failed Logins by IP](02-Failed-Logins-By-IP.png)

### Failed Login Visualization

![Failed Login Bar Chart](03-Failed-Login-Bar-Chart.png)

### Brute-Force Investigation

![Brute-Force Investigation](brute%20force%20investigation.png)

## Security Investigation Findings

The dataset contained 31 failed authentication events associated with four source IP addresses.

The highest number of failures originated from `192.168.1.50`, which attempted authentication against the `admin` account.

The event data also showed a successful authentication for the `admin` account following repeated failures from the same source IP.

This pattern warrants additional investigation because repeated authentication failures followed by success can be consistent with password-guessing activity.

However, the available evidence alone does not establish that an actual account compromise occurred.

## Recommended SOC Response

1. Review the affected account's authentication history.
2. Investigate the source IP address and associated endpoint.
3. Correlate successful login events with preceding failures.
4. Review endpoint and authentication logs for additional suspicious activity.
5. Escalate suspicious findings according to incident response procedures.
6. Document investigation results and recommended actions.

## Skills Demonstrated

- Security Event Monitoring
- SIEM Log Analysis
- Splunk SPL Queries
- Windows Authentication Log Investigation
- Brute-Force Detection Logic
- Source IP Analysis
- Security Dashboard Development
- SOC Incident Triage
- Security Investigation Documentation

## Project Outcome

Created a Splunk SOC monitoring dashboard to analyze authentication events, visualize failed login trends, and identify potential brute-force activity.

This hands-on project demonstrates foundational SOC Analyst Level 1 skills in security monitoring, event investigation, detection engineering, and incident documentation.


