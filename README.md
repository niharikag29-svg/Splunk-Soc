# Splunk Firewall Log Monitoring Project

## Overview
Analyzed firewall CSV logs using Splunk to monitor blocked traffic and detect suspicious source IPs.

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
index=firewall action=block | stats count
index=firewall action=block | stats count by src_ip
index=firewall action=block | timechart count

## Outcome
Identified malicious IP addresses and visualized firewall security events using Splunk dashboards and alerts.

