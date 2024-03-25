### <ins>Handy Aliases</ins>

- alias home="cd /mnt/c/Users/sgreen"
- alias np="/mnt/c/Program\\ Files/Notepad++/notepad++.exe"
- alias fire="/mnt/c/Program\\ Files/Mozilla\\ Firefox/firefox.exe"
- alias spot="/mnt/c/Users/sgreen/Application\\ Data/Spotify/Spotify.exe"
- alias host="sudo vim /mnt/c/Windows/System32/drivers/etc/hosts"

### <ins>Name resolvement issues on WSL</ins>
```bash
sudo rm /etc/resolv.conf # Remove the symlinked file  
echo "nameserver 8.8.8.8" | sudo tee /etc/resolv.conf

sudo echo -e "[network] \\ generateResolvConf = false" > /etc/wsl.conf
exit 
wsl --shutdown 
wsl
```