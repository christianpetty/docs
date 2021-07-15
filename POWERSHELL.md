[Official PowerShell Documentation](https://github.com/PowerShell/PowerShell/tree/master/docs/learning-powershell)

# List of modules
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
