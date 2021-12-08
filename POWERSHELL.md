[Official PowerShell Documentation](https://github.com/PowerShell/PowerShell/tree/master/docs/learning-powershell)

# List of modules to check out
* ImportExcel

# Install module
```powershell
Install-Module -Name {MODULE NAME}
```

# Create a profile
```powershell
New-Item $profile -itemtype file -force
```

# Use tab-completion
```powershell
Set-PSReadlineKeyHandler -Key Tab -Function Complete
```

# Use bash-like tab-completion
```powershell
Set-PSReadlineKeyHandler -Key Tab -Function MenuComplete
```

# Use light theme
```powershell
Set-ItemProperty -Path HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Themes\Personalize -Name SystemUsesLightTheme -Value 1
Set-ItemProperty -Path HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Themes\Personalize -Name AppsUseLightTheme -Value 1
```

# Use dark theme
```powershell
Set-ItemProperty -Path HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Themes\Personalize -Name SystemUsesLightTheme -Value 0
Set-ItemProperty -Path HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Themes\Personalize -Name AppsUseLightTheme -Value 0
```

# List unique file extensions in a directory recursively
```powershell
Get-ChildItem -Recurse -File | Select-Object DirectoryName, Extension -Unique
```

# Add module to profile
```powershell
$env:PSModulePath += ";C:\Users\Christian\Documents\GitHub\PSTools"
```

# Export list of installed programs to txt file
```powershell
Get-ItemProperty HKLM:\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Uninstall\* | Select-Object DisplayName | Format-Table > <FILENAME>
```

# Connect to Exchange Online
```powershell
Import-Module ExchangeOnlineManagement
Connect-ExchangeOnline -UserPrincipalName <USERNAME>
```