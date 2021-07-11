[Official PowerShell Documentation](https://github.com/PowerShell/PowerShell/tree/master/docs/learning-powershell)

# Create a profile
```powershell
new-item $profile -itemtype file -force
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
New-ItemProperty -Path HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Themes\Personalize -Name SystemUsesLightTheme -Value 1 -Type Dword -Force
New-ItemProperty -Path HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Themes\Personalize -Name AppsUseLightTheme -Value 1 -Type Dword -Force
```

# Use dark theme
```powershell
New-ItemProperty -Path HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Themes\Personalize -Name SystemUsesLightTheme -Value 0 -Type Dword -Force
New-ItemProperty -Path HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Themes\Personalize -Name AppsUseLightTheme -Value 0 -Type Dword -Force
```
