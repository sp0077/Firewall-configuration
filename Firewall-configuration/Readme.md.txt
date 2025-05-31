


This repository contains configurations, scripts, and documentation related to Windows Defender Firewall settings. The goal is to implement and test firewall rules for securing system access and blocking unwanted traffic.


- **Block Telnet (Port 23)** - Prevent unauthorized access via Telnet.
- **Custom Inbound/Outbound Rules** - Define traffic restrictions for specific applications.
- **Testing  Command Prompt** - Verify firewall behavior.


### 1. Applying Firewall Rules
To create a firewall rule using PowerShell, run:
```powershell
New-NetFirewallRule -DisplayName "Block Telnet" -Direction Inbound -Protocol TCP -LocalPort 23 -Action Block