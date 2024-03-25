### <ins>SSH keys</ins>

Set-Service -Name ssh-agent -StartupType Automatic

Set-Service -Name ssh-agent -Status Running ssh-keygen -f &lt;filename&gt; -t rsa -b 4096

Filename is optional

ssh-add &lt;path to private key&gt;

Or run from key directory

ssh -T git@bitbucket.org

git config --global core.sshCommand "'C:\\Windows\\System32\\OpenSSH\\ssh.exe'"

$pkg = "D:\\a\\test\\ultimate\\WindowsApplicationDriver_1.2.1.msi";

Start-Process msiexec "/i $pkg /qn";

Install msi silent in powershell

net use * [\\\nas\\share](file://nas/share) (mount a nas point on cmd line)

### <ins>Commands</ins>

- appwiz.cpl (control panel)
- msconfig (command arg to open boot and shortcuts)
- nslookup (ipaddress for domain and such)
- netstat -an (all of your network connections/ports)
- mmc (as admin to open MS cert store)
- gpedit.msc (opens group policy editor)
- gpresult /h gp.htm (will show all the group policies on your computer)
- shutdown /r /f /t 0 /m [\\\servername](file://servername/)
- certutil -dspublish -f &lt;filename&gt; NTAUTHCA
- certutil -viewstore -enterprise NTAUTH
- certutil –pulse (triggers auto-enrool and downloads chain certificates)
- certutil -scinfo (print smartcard data)
- qwinsta /server: <computername>(query who is logged in the comp)</computername>
- rwinsta &lt;ID from above command&gt; /server: <computername>(log the person off)</computername>
- Get-PSDrive -PSProvider FileSystem (List Drives on the system)

### <ins>Mix</ins>

https://<exchange-server>/owa (access mailboxes of users online)