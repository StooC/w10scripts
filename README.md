# Windows 10 Optimisation Scripts
These scripts based on various tweaks and scripts I've found around the internet with particular thanks to the following:
* https://github.com/ChrisTitusTech/win10script

## How the scripts are structured
These scripts are structured into 'levels' so that you can apply more or less opimisations depending on the intended use for the targeted machine. A description the levels (which can be run independently) is as follows:

Minimum: This is intended to have little to no feature loss to the intended user and so can be safely applied to any machine.

Medium: This is intended to be used where a more aggressive removal of bloat and unused features is required. This script can be of particular use on low end systems which benefit from removing as many unused processes as possible.

Techical-User: This script is intended to set settings often wanted by techincal users such as showing file extensions but may confuse or limit less techincal users. 

## How to Run
Paste this command into Powershell (admin):

### Minimum
```
iex ((New-Object System.Net.WebClient).DownloadString('https://github.com/StooC/w10scripts/minimum.ps1'))
```

### Medium
```
iex ((New-Object System.Net.WebClient).DownloadString('https://github.com/StooC/w10scripts/medium.ps1'))
```

### Techincal User
```
iex ((New-Object System.Net.WebClient).DownloadString('https://github.com/StooC/w10scripts/techincal-user.ps1'))
```

## How to Revert Changes
Currently there is **NO UNDO** scripts provided although this may change in future. However a restore point is created before each script makes changes so you can use this to revert these changes.

Alternatively as most changes are applied to the Windows registry creating a backup before running the script is another method of undoing most of the changes. 