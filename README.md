# Azure Sentinel SOC Lab

This project demonstrates a cloud-based Security Operations Center (SOC) environment using Microsoft Sentinel in Azure.

## Lab Overview

In this lab I built a cloud SIEM environment capable of detecting authentication attacks.

Components used:

- Microsoft Sentinel (SIEM)
- Azure Virtual Machine
- Log Analytics Workspace
- Windows Security Event Logs

## Architecture

Azure VM → Log Analytics Workspace → Microsoft Sentinel → Security Incidents

## Attack Simulation

The following attack behaviors were simulated:

- Multiple failed login attempts (Event ID 4625)
- Suspicious authentication activity
- Security log ingestion from Windows VM

## Detection Rule

A Sentinel analytics rule was created to detect:

Failed login attempts greater than 5 within 5 minutes.

This triggers a security incident for investigation.

## Skills Demonstrated

- Cloud Security Monitoring
- SIEM Deployment
- Security Log Analysis
- Threat Detection
- Incident Investigation
- Microsoft Sentinel Administration

## Screenshots

### Sentinel Dashboard
![Sentinel](sentinel-dashboard.png)

### Failed Login Query
![Query](failed-login-query.png)

### Security Incident
![Incident](incident-alert.png)

### Data Connector
![Connector](data-connector.png)
