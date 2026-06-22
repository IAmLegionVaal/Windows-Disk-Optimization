# Windows Disk Optimization

> **Testing note:** This was tested by me to be working. User experience may vary.

## One-click use

1. Download and extract the repository.
2. Double-click `Run-OneClick.bat`.
3. Approve the Windows administrator prompt.
4. The launcher runs Windows volume optimisation and component-store cleanup directly—there is no menu.
5. Allow all storage operations to finish, then review the exit code and logs in `C:\ProgramData\WindowsDiskOptimization\Logs`.

Included script: `Optimize-WindowsDisk.ps1`

## PowerShell usage

```powershell
.\Optimize-WindowsDisk.ps1
.\Optimize-WindowsDisk.ps1 -Optimize
.\Optimize-WindowsDisk.ps1 -ComponentCleanup
.\Optimize-WindowsDisk.ps1 -Optimize -ComponentCleanup -WhatIf
```

The default PowerShell mode reports volumes, physical-disk health, TRIM status and component-store analysis. Optional optimisation actions require elevation.

Exit codes: `0` success, `1` fatal error, `2` warnings.

Use at your own risk. Maintain backups and allow storage operations to complete without interruption.

MIT License.
