### <ins>Profile Creation</ins>

Test-Path $PROFILE

New-Item -Type File -Path $PROFILE -Force

notepad.exe $PROFILE

Set-Alias -Name l -Value Get-ChildItem

. $PROFILE

Set-ExecutionPolicy Unrestricted (may need to do this to run scripts)

\# This is a comment and will not be executed

<#

This is a multi-line

comment block

#>

### <ins>Contents for $PROFILE</ins>

Set-Location "C:\\Users\\sgreen"

Set-Alias -Name np -Value notepad.exe  
Set-Alias -Name sub -Value "C:\\Program Files\\Sublime Text 3\\sublime_text.exe"  
Set-Alias -Name l -Value ls  
Set-Alias -Name ubu -Value Connect-Ubu  
Set-Alias -Name u -Value cdup

\# Load scripts from the following locations  
#$env:Path += ";D:\\SysAdmin\\scripts\\PowerShellBasics"

\# Set default variables  
#$adminUPN = "lazyadmin@lazydev.onmicrosoft.com"

function cdup {  
   param(  
      [int]$levels = 1  
   )

   \$path = '..\\' * $levels

   cd $path.TrimEnd('\\')  
}

function card {  
certutil.exe -scinfo  
}

function certs {  
Get-ChildItem -Path Cert:\CurrentUser\My\  
}

function sudo {  
Start-Process PowerShell -Verb RunAs  
}  
function ocsp ([string]$cert) {  
certutil -url \$cert  
}

function tailf([string]\$path) {  
Get-Content -Wait -Path \$path  
}

function findf([string]\$myFile) {  
Get-ChildItem -Path / -Recurse -ErrorAction SilentlyContinue -Force -Filter \$myFile  
}

function touch(\$file) {  
"" | Out-File \$file -Encoding ASCII  
}

function df {  
Get-Volume  
}

function sed(\$file, \$find, \$replace){  
(Get-Content \$file).replace("\$find", \$replace) | Set-Content \$file  
}

function Connect-Ubu {
ssh sgreen@172.18.10.44
}