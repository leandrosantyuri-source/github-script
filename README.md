$WshShell = New-Object -ComObject WScript.Shell

$Shortcut = $WshShell.CreateShortcut("$env:USERPROFILE\Desktop\MeuPrograma.lnk")

$Shortcut.TargetPath = "C:\Program Files\Google\Chrome\Application\chrome.exe"

$Shortcut.WorkingDirectory = "C:\Program Files\Google\Chrome\Application"

$Shortcut.IconLocation = "C:\Program Files\Google\Chrome\Application\chrome.exe"

$Shortcut.Save()
