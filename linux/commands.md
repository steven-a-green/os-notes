# <ins>Commands</ins>

- **nm** (shows symbols in .o and .so files)
- **strace** (follows the program running)
- **du** (display disk usage information)
- **df** (display file usage information)
- **xdg-open** (pdf viewer in Linux)
- **pstree** (shows tree view of processes)
- **usb-devices** (prints a bunch of info of all the usb sockets)
- **lsblk** (shows you devices on system)
- **blkid** (good one too)
- **whereis** (located the commands)
- **at** (will schedule a batch job at this time)
- **nl** (outputs a file with line numbers)
- **mtr** (ping and traceroute )
- **| xclip -selection c** (clipboard)
- **onboard** (virtual keyboard)
- **env** (shows the entire configuration)
- **dos2unix** (converts a windows made code to Unix)
- **cat /proc/cpuinfo** (cpu information)
- **cat /etc/os-release** (operating system information)
- **git clone -c http.sslverify=false [https://myserver/&lt;user&gt;/&lt;project&gt;.git](https://myserver/%3Cuser%3E/%3Cproject%3E.git)**
- **wget –no-check-certificate**
- **xxd filename** (hex dump)
- **ssh-keyscan 192.168.11.141** (scans ssh keys on remote system to add to known-hosts)
- **ssh-keygen -R 192.168.3.10** (removed cached ssh known ssh keys keys)
- **last** (show last logged in users)
- **nmcli** (networkmanager command line interface)
- **grep -nir 'yourString\*' .** (rec search dir for string w/line #)
- **rg/ag** (better grep search)
- **tee** (direct output to stdout and also a file)

# <ins>Fun Commands</ins>

- **| lolcat** (colored output)
- **curl parrot.live** (dancing parrot)
- **sl** (does a train across screen)
- **yes** (w/ anything with echo forever)
- **banner** (w/ anything makes a banner)
- **fortune** (gives you a quote)
- **rev** (stdin or file as reverse)
- **cowsay** (makes a cow with a quote)
- **xcowsay** (graphical cow say)
- **cowthink** (cow with thought bubble)
- **cmatrix** (makes the matrix happen)
- **curl wttr.in/NewportBeach**
- **neofetch** (print system information)

# <ins>Control Commands</ins>

- **ctrl-r** (reverse search the history)
    
- **ctrl-s** (freezes the screen)
    
    - **ctrl-q** (unfreezes)
- **ctrl-a** (front of line)
    
- **ctrl-e** (end of line)
    

# <ins>RHEL repo subscription manager setup</ins>

subscription-manager register && subscription-manager list --available --all \\

&& subscription-manager attach --pool<poolid>
      (get pool id from previous cmd output and do it twice for the RHEL server and cert system)