# Flush DNS
`ipconfig /flushdns`

# Disable Bing
1. Run regedit
2. Navigate to `Computer\HKEY_CURRENT_USER\SOFTWARE\Policies\Microsoft\Windows\Explorer`
3. Create a 32 bit DWORD `DisableSearchBoxSuggestions` with value `1`
