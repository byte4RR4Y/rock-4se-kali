# rock-4se-kali
# A Kali Linux ARM image for the RADXA Rock Pi 4 SE - rk3399t

"If it doesn't exist, create it yourself." Daniel Wieczorek


Download docker image(it's more up to date)with the following command and build it on your own:

-----------------------------------------------------------------------------------------------
         docker pull byte4rr4y/kalilinux-rock4se
-----------------------------------------------------------------------------------------------

I've added a cllection of wallpapers.

----------------
REAL KALI LINUX         (kernel 6.1.0-kali7-arm64)
----------------

This is a kali build from the bottom of a kali root filesystem
----------------------------
   Desktop: XFCE4
   Kernel: 6.1.0
   Build Date: 2023/05/07
----------------------------

The image is 15.8 GB and therefore a 32 GB SD card is recommended(if you want to install software). 


login:_________kali

password:____kali


------------------------------------------------------------------------------
! FIRST BOOT TAKES 2 MINUTES AND 12 SECONDS FOR RESIZING THE ROOT FILESYSTEM !
------------------------------------------------------------------------------



ISSUES:

1.)BLACK SCREEN:

If you have a black screen after a boot-time of 1 minute and 5 seconds you moust mount the root filesystem on your Linux-Machine and edit /etc/X11/xorg.conf.d/10-monitor.conf and set the right Screenresolution(e.g.: 1920x1080).
-----------------------------------------------------
    Section "Monitor"
         Identifier "HDMI-1"
         Option "PreferredMode" "1920x1080"
    EndSection
-----------------------------------------------------



!! DO NOT OVERCLOCK WITH 'rsetup' !!





DOWNLOADS:
-----------

SD-Card Image: <a href="https://drive.google.com/file/d/1R5yjq9kJbd6lxPB7g_EjfIm-yuXF_8nW/view?usp=sharing">kali-final-2023-05-07.img.xz</a> (3.3 GB)

Root Filesystem: <a href="">kali-final-2023-05-08-rootfs.tar.xz</a> (X.X GB)

Dockerimage: <a href="https://hub.docker.com/r/byte4rr4y/kalilinux-rock4se">Dockerimage</a> (4.3 GB)
