RaspberryPiJive
=============

Setting Up a Raspberry Pi with Jivelite as a stand-alone Player

Instructions in the Wiki at https://github.com/ggalt/RaspberryArch/wiki/How-To-Make-a-RaspberryPi-Jive-Player

Instructions for a wall-mounted USB display Jivelite player at: 
http://www.instructables.com/id/Wall-Mounted-SqueezePlayer-with-Raspberry-Pi/

The stock Arch kernel supports the standard Mimo 720F DisplayLink through the framebuffer.
You will need to install xf86-video-fbdev and the rest of the standard xorg installation
(see the Arch Linux Beginner Guide at https://wiki.archlinux.org/index.php/Beginners%27_Guide).
There is no longer a need to install any special framebuffers or usb drivers.
Adjust the configuration file in this repository to reflect your configuration (make sure the
touchscreen is listed as the same device, and that the framebuffer is located at the same device)
and copy it to /etc/X11/xorg.conf.d/20-displaylink.conf

