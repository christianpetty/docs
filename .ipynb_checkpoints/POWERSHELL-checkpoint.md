[Official PowerShell Documentation](https://github.com/PowerShell/PowerShell/tree/master/docs/learning-powershell)

# Create a profile
```
new-item $profile -itemtype file -force
```

# Use tab-completion
```
Set-PSReadlineKeyHandler -Key Tab -Function Complete
```

# Use bash-like tab-completion
```
Set-PSReadlineKeyHandler -Key Tab -Function MenuComplete
```

