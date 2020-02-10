# cmdUtiles


### Find the password for the currently connected wireless network:

sudo grep -r '^psk=' /etc/NetworkManager/system-connections/

### Kazam(video recorder)

start recording: Super + Control + r
pause recording: Super + Control + p
finish recording: Super + Control + f
show Kazam: Super + Control + s
quit Kazam: Super + Control + q

Note: "Super" is usually this "Windows logo" key.


## Removing evaluation key bash script for Linux:
#!/bin/bash

echo "removeing evaluation key"
rm  -rf ~/.PhpStorm*/config/eval

rm -rf ~/.java/.userPrefs/jetbrains/webstorm

echo "resetting evalsprt in other.xml"
sed -i '/evlsprt/d' ~/.PhpStorm*/config/options/other.xml

echo "resetting evalsprt in prefs.xml"
sed -i '/evlsprt/d' ~/.java/.userPrefs/prefs.xml

echo "change date file"
find ~/.PhpStorm* -type d -exec touch -t $(date +"%Y%m%d%H%M") {} +;
find ~/.PhpStorm* -type f -exec touch -t $(date +"%Y%m%d%H%M") {} +;
