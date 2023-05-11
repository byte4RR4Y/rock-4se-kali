# Kali Linux XFCE for Radxa Rock Pi 4 SE
__________________________________________________________________________________________________
A Kali Linux ARM image for the RADXA Rock Pi 4 SE - rk3399t

It's a Rolling release, so you can do: 
-------------------------
    apt update && apt upgrade && apt full-upgrade && apt dist-upgrade
-------------------------
to be up to date!

"If it doesn't exist, create it yourself." Daniel Wieczorek

----------------
REAL KALI LINUX
----------------

This is a kali build from the bottom of a kali root filesystem
The image is 16.7 GB and therefore a 32 GB SD card is required. 
----------------------------
    login:_______kali
    password:____kali
    ----------------------
    Desktop: XFCE4
    Kernel: 6.1.0
    Build Date: 2023/05/09
----------------------------

------------------------------------------------------------------------------
! FIRST BOOT TAKES 2 MINUTES AND 12 SECONDS FOR RESIZING THE ROOT FILESYSTEM !
------------------------------------------------------------------------------



ISSUES:

1.)BLACK SCREEN:

If you have a black screen after a boot-time of 1 minute and 5 seconds you must

mount the root filesystem on your Linux-Machine and edit /etc/X11/xorg.conf.d/10-monitor.conf

and set the right Screenresolution(e.g.: 1920x1080).

-----------------------------------------------------
    Section "Monitor"
         Identifier "HDMI-1"
         Option "PreferredMode" "1920x1080"
    EndSection
-----------------------------------------------------



# DO NOT OVERCLOCK WITH "rsetup" 

____________________________________________________________________________
# DOWNLOADS:
-----------

SD-Card Image: <a href="https://drive.google.com/file/d/13V7PaB7aY-MwC5Vn2QP0vCoSea7RujDL/view?usp=sharing">kali-final-2023-05-09.img.xz</a> (3.5 GB)

SD-Card Image alternative download: <a href="https://archive.org/download/kali-final-2023-05-09.img/kali-final-2023-05-09.img.xz">kali-final-2023-05-09.img.xz</a> (3.5 GB)

Root Filesystem: <a href="https://drive.google.com/file/d/1QcKa8FkMXnw676MyZa_9ly5d3Svdw6pl/view?usp=sharing">kali-final-2023-05-09-rootfs.tar.xz</a> (3.2 GB)

Dockerimage: <a href="https://hub.docker.com/r/byte4rr4y/kalilinux-rock4se">Dockerimage</a> (5.0 GB)
