# rock-4se-kali
# A Kali Linux ARM image for the RADXA Rock Pi 4 SE - rk3399t

"If it doesn't exist, create it yourself." Daniel Wieczorek


Download docker image(it's more up to date)with the following command and build it on your own:

-----------------------------------------------------------------------------------------------
         docker pull byte4rr4y/kalilinux-rock4se:latest
-----------------------------------------------------------------------------------------------

I've added a cllection of wallpapers.

----------------
REAL KALI LINUX         (kernel 6.1.0-kali7-arm64)
----------------

This is a kali build from the bottom of a kali root filesystem

The image is 15.8 GB and therefore a 32 GB SD card is recommended(if you want to install software). 


login:_________kali

password:____kali


-----------------------------------------------------
!!! YOU MUST MANUALLY RESIZE YOUR ROOT PARTITION !!!
-----------------------------------------------------

Download at <a href="https://drive.google.com/file/d/1ThpTQD_hTV_XHnc50TdDmaR5FZ2aM5Li/view?usp=sharing">Kali-preview-2023-05-07.img.xz</a> (3.3 GB)



ISSUES:

1.)BLACK SCREEN:

If you have a black screen after a boot-time of 1 minute and 5 seconds you moust mount the root filesystem on your Linux-Machine and edit /etc/X11/xorg.conf.d/10-monitor.conf and set the right Screenresolution(e.g.: 1920x1080).



2.)CORRUPT ZSH_HISTORY FILE:

-----------------------------------------------------
          cd ~
          mv .zsh_history .zsh_history_bad
          strings -eS .zsh_history_bad > .zsh_history
          fc -R .zsh_history
-----------------------------------------------------


!! DO NOT OVERCLOCK WITH 'rsetup' !!
