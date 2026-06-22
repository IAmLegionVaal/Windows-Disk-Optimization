# Windows Disk Optimization

> **Testing note:** This was tested by me to be working. User experience may vary.

Included script: `Optimize-WindowsDisk.ps1`

```powershell
.\Optimize-WindowsDisk.ps1
.\Optimize-WindowsDisk.ps1 -Optimize
.\Optimize-WindowsDisk.ps1 -ComponentCleanup
```

The default mode reports volumes, physical-disk health, TRIM status and component-store analysis. Optional optimisation actions support `-WhatIf` and require an elevated PowerShell window.

Logs: `C:\ProgramData\WindowsDiskOptimization\Logs`

Exit codes: `0` success, `1` fatal error, `2` warnings.

Use at your own risk. Maintain backups and allow storage operations to complete without interruption.

MIT License.
