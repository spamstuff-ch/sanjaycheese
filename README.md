# SjCheese
Take webcam shots from target just sending a malicious link

# How it works?
<p>The tool generates a malicious HTTPS page using Serveo or Ngrok Port Forwarding methods, and a javascript code to cam requests using MediaDevices.getUserMedia. </p>

<p>The MediaDevices.getUserMedia() method prompts the user for permission to use a media input which produces a MediaStream with tracks containing the requested types of media. That stream can include, for example, a video track (produced by either a hardware or virtual video source such as a camera, video recording device, screen sharing service, and so forth), an audio track (similarly, produced by a physical or virtual audio source like a microphone, A/D converter, or the like), and possibly other track types. </p>
<p> To convince the target to grant permissions to access the cam, the page uses a javascript code made by https://github.com/wybiral that turns the favicon into a cam stream.</p>



## Installing (Termux):

```
for begineer download termux form the playstore
Give the storage permissions to termux application.(settings/manageapp/termux/permissions)
update termux by command (  apt update && apt upgrade  )
install git by command (   apt install git   )
next (  git clone https://github.com/spamstuff-ch/sj.git    )
use ls command to show directory ( ls )
enter into the Directory by ( cd sj  )
again see whats inside sj directory ( ls )
you will find some elements
to get those all elements in executable format use (   chmod +x *   )
some additional packages to be installed to run these script so use ( apt install php && pkg install wget )
run the shell command by (  ./sjcheese.sh  )
choose option 2 for ngrok
In termux turn on your mobile hotspot to generate link with ngrok ( with internet )
Send the generated link to the victim 
if victim grant permission you will get the snaps of the victim
to kill the process press (  ctrl + c )
All camfiles will be stored in the same directory
move the camfiles to the sdcard by (  mv <name of camfile eg:cam.....> /sdcard)
open your file manager to see the snaps
```

## Installing (Kali Linux):

```
git clone https://github.com/spamstuff-ch/sj.git
cd sjcheese
bash sjcheese.sh (or) ./sjcheese.sh
```