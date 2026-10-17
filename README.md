# Cohesity Sizing Tool

## Description

Cohesity Sizing Tool is a PowerShell script that connects to supported cloud services and collects usage data for various workloads. The size of the data calculated by the script aligns with data backed up by:

- Cohesity DataProtect
- Cohesity Cloud Services
- Cohesity Alta SaaS Protection

At the end of the script, all collected information is exported to a CSV file.

## Supported cloud services

1. **Microsoft 365** Exchange Online, SharePoint Online, OneDrive, Teams Chat  
2. **Google Workspace** Gmail, Google Drive  
3. **Salesforce** Active users, data and file storage  

## Documentation

- [Microsoft 365 Sizing](docs/m365.md)
- [Google Workspace Sizing](docs/google-workspace.md)
- [Salesforce Sizing](docs/salesforce.md)

## Requirements (summary)

- **Windows PowerShell 5.1**
- Network access for the target cloud APIs
- Service-specific PowerShell modules and permissions

## Outputs

| Artifact | Location | Pattern |
|----------|----------|---------|
| Report CSV | Same folder as the script | `Cohesity-Sizing-YYYYMMDD-HHMMSS.csv` |
| Log file | Same folder as the script | `Cohesity-Sizing-Tool-YYYYMMDD-HHMMSS.log` |


