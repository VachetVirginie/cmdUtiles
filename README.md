# cmdUtiles


### Find the password for the currently connected wireless network:

sudo grep -r '^psk=' /etc/NetworkManager/system-connections/

#Kazam(video recorder)

start recording: Super + Control + r
pause recording: Super + Control + p
finish recording: Super + Control + f
show Kazam: Super + Control + s
quit Kazam: Super + Control + q

Note: "Super" is usually this "Windows logo" key.


# Qwerty on Linux:
 sudo loadkeys fr 
# Git

## Cette commande supprimera toute les branches qui ont été mergé sur master :

git branch --merged | grep -v "\*" | grep -v master | xargs -n 1 git branch -d
