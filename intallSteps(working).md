If You are having issues installing - do this - it worked for me:


1) Download the Google AIY image: https://dl.google.com/dl/aiyprojects/vision/aiyprojects-2018-01-03.img.xz
2) Flash it to an SD Card:
  --> Link to Freeware to Flash the Image File: https://etcher.io/
3) Put the SD Card into Your Pi 3 and plug it into a keyboard, monitor, and Internet - Power it on by plugging it in

4)Install git to get the MagicMirror code:

sudo apt-get install git

5)Install the missing packages:

sudo apt-get install libxss1 (Already be installed w/image?)

sudo apt-get install libnss3

6)Autohiding the Mouse Cursor with unclutter:

sudo apt-get install unclutter

7)Get and install MagicMirror with the Automatic Installer:

curl -sL https://raw.githubusercontent.com/MichMich/MagicMirror/master/installers/raspberry.sh | bash

8) Go to MagicMirror folder:

cd ~/MagicMirror

9)Install the app:

npm install (May be unneccessary)

10) Duplicate config/config.js.sample to config/config.js.

cp config/config.js.sample config/config.js

10) Go back to root:

cd ..
11) Rotating the screen and hide Rainbow colored cube:

sudo nano /boot/config.txt

Add the following line:

display_rotate=3

disable_splash=1

AutoStart - Jon Stuck here!!!!
