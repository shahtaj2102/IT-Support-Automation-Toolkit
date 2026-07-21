# IT Support Automation Toolkit

A small collection of PowerShell scripts automating real Help Desk and sysadmin tasks: user onboarding, offboarding, system health reporting, and log parsing.

## Why this exists

I'm a career-switcher moving from 7 years as a Mechanical Technician/Department Lead into IT, currently doing part-time IT support (Microsoft 365 admin, Active Directory) at my job. These scripts automate tasks I actually do there by hand: deploying and administering Microsoft 365 (licensing, provisioning), setting up and managing Active Directory, and handling offboarding and license reallocation. This toolkit is that real, on-the-job experience turned into repeatable automation, built alongside a focused hands-on study sprint (Active Directory labs, Microsoft 365 and Entra ID sandbox, PowerShell) in July 2026.

To be clear on originality: I learned the underlying Active Directory, Microsoft 365, and PowerShell concepts through structured courses and lab environments (Server Academy's AD course, Microsoft Learn's PowerShell and M365 modules) - that's how anyone learns a new stack. But every script here is my own design, written to automate real tasks from my actual job and IT support work, not copied from any tutorial or walkthrough. The courses taught the underlying concepts; the job gave the real use cases; the scripts themselves are original.

## Scripts

| Script | Purpose | Status |
|---|---|---|
| New-BulkADUsersFromCSV.ps1 | Bulk-create AD user accounts from a CSV file | Planned |
| Disable-OffboardingAccount.ps1 | Automated offboarding, disables AD account and removes M365 license | Planned |
| Get-DiskHealthReport.ps1 | Disk-space and system-health report generator | Planned |
| Parse-EventLog.ps1 | Basic Windows event log parser | Planned |

This table gets updated as each script actually ships; check commit history for real, current progress rather than relying on this status column alone.

## Environment used to build and test these

- Windows 11 Pro VM (VirtualBox), domain-joined to a lab Active Directory environment
- Microsoft 365 Developer Program E5 sandbox (Entra ID and M365 admin testing)
- PowerShell 7 with VS Code

## Usage

Each script will include its own header comment with parameters and a usage example once implemented. General pattern: .\ScriptName.ps1 -Param1 value -Param2 value
