# <ins>Commands</ins>

- sc_auth unpair -u [username]
- sc_auth identities
- smartCardServices
- system_profiler SPSmartCardsDataType
- security list-smartcards
- sudo defaults delete /Library/Preferences/com.apple.security.smartcard DisabledTokens ?
- sudo defaults read /Library/Preferences/com.apple.security.smartcard
- sudo defaults write /Library/Preferences/com.apple.security.smartcard UserPairing -bool NO
- sudo -u _securityagent /Applications/HostApp.app/Contents/MacOS/HostApp

# <ins>Notes</ins>
- /usr/local/libexec/SmartCardServices/drivers/ifd.bundle