# rock-4se-kali
A Kali Linux ARM image for the RADXA Rock Pi 4 SE - rk3399t
"If it doesn't exist, create it yourself." Daniel Wieczorek


-------------------
1.) REAL KALI LINUX            (kernel 6.1.0-kali7-arm64)
-------------------
---------------------------------------------------------------
This is a kali build from the bottom of a kali root filesystem
---------------------------------------------------------------

The image is 15.7 GB and therefore a 32 GB SD card is recommended(if you want to install software). 

login:_________kali

password:____kali

-----------------------------------------------------
!!! YOU MUST MANUALLY RESIZE YOUR ROOT PARTITION !!!
-----------------------------------------------------

Download at <a href="https://drive.google.com/file/d/1QoC4TYqMhqN2ZGgexg_mCqpXTqODOYb7/view?usp=sharing">Kali-Linux-XFCE-wifi-bluetooth-2023-05-06.img.xz</a> (3.1 GB)

ISSUES:

BLACK SCREEN:

If you have a black screen after a boot-time of 1 minute and 5 seconds you moust mount the root filesystem on your Linux-Machine and edit /etc/X11/xorg.conf.d/10-monitor.conf and set the right Screenresolution(e.g.: 1920x1080).

CORRUPT ZSH_HISTORY FILE:
-----------------------------------------------------
cd ~
-----------------------------------------------------
-----------------------------------------------------
mv .zsh_history .zsh_history_bad
-----------------------------------------------------
-----------------------------------------------------
strings -eS .zsh_history_bad > .zsh_history
-----------------------------------------------------
-----------------------------------------------------
fc -R .zsh_history
-----------------------------------------------------


!! DO NOT OVERCLOCK WITH 'rsetup' !!

#################################################################################
#################################################################################


---------------------
2.) KALI LINUX DEBIAN          (build on Debian with kernel 6.1.0-kali7-rt-arm64)
---------------------
It's build on Debian but works fine

The image needs 1-2 minutes to boot the desktop but runs stable with a kali linux kernel.

The image is 14.2 GB and therefore at least a 16 GB SD card is required.
This is kali linux default without kingphisher.

Username: kali
Password: kali

!! DO NOT OVERCLOCK WITH 'rsetup' !!

Download at <a href="https://drive.google.com/file/d/1sig3IbY23cuAeM2c20aRQESbx57z_mBA/view?usp=sharing">rock4se-kali-linux-default-2023-W15-xfce.img.xz</a> (3.9GB)
