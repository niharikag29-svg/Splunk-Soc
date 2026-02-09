# Splunk Firewall Log Monitoring

## Project Overview
Analyzed firewall CSV logs using Splunk to detect blocked traffic, identify suspicious IPs/ports, and build dashboards and alerts for proactive monitoring.

## Data Source
Firewall logs in CSV format.

## Features
- CSV log ingestion
- Blocked traffic analysis
- Top attacker identification
- Port and protocol analysis
- Dashboard visualization
- Alert creation for suspicious activity

## Sample Queries

## show blocked traffic
index=firewall action=block | stats count 
## count by source ip
index=firewall action=block | stats count by src
## Timechart of Attack Trend
index=firewall action=block | timechart count

## 📊 Screenshots & Results

### Blocked Traffic Detection
![Blocked Traffic](screenshots/01_blocked_events_search.png)

### Protocol Analysis
![Protocol Analysis](screenshots/02_blocked_by_protocol.png)

### Top Source IPs (Attackers)
![Top Source IPs](screenshots/03_top_source_ips.png)

### Target Ports Analysis
![Target Ports](screenshots/04_target_ports_analysis.png)

### Traffic Timeline
![Attack Timeline](screenshots/05_attack_timeline.png)

### Alerts Overview
![Alerts](screenshots/06_alerts_overview.png)

### Firewall Dashboard
![Dashboard](screenshots/07_firewall_dashboards.png)

### Firewall Dashboard
![Dashboard](screenshots/08_firewall_dashboard.png)


## Outcome
Identified malicious IP addresses and visualized firewall security events using Splunk dashboards and alerts.