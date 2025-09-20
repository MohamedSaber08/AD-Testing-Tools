# AD-Testing-Tools

decode the file back into an executable : 
$content = Get-Content -Path "mimikatz.b64" -Raw
$bytes = [System.Convert]::FromBase64String($content)
[System.IO.File]::WriteAllBytes("mimikatz.exe", $bytes)
