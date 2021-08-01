# Rename photos based on date created 
```powershell
exiftool -d '%Y-%m-%d%%+3c.%%le' '-filename<CreateDate' .
```