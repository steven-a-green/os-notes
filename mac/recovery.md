# <ins>Option 1</ins>

- Restart and hold cmd-r on boot
- Choose terminal in utilies menu
- Enter resetpassword

# <ins>Option 2</ins>

- Restart and hold cmd-s on boot
- mount -uw /
- Now run cmd to load open directory
- launchctl load /System/Library/LaunchDaemons/com.applet.opendirectoryd.plist
- passwd username