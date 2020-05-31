# debian-customize

etcher + iso debian 

https://www.debian.org/distrib/
A larger complete installation image: contains more packages, making it easier to install machines without an Internet connection. 
https://cdimage.debian.org/debian-cd/current/amd64/iso-cd/
debian-10.4.0-amd64-netinst.iso

brancher un cable ethernet
su root
nano /etc/apt/sources.list

deb http://deb.debian.org/debian/ buster main contrib non-free
deb-src http://deb.debian.org/debian/ buster main contrib non-free

deb http://security.debian.org/debian-security buster/updates main contrib non-free
deb-src http://security.debian.org/debian-security buster/updates main contrib non-free

# buster-updates, previously known as 'volatile'
deb http://deb.debian.org/debian/ buster-updates main contrib non-free
deb-src http://deb.debian.org/debian/ buster-updates main contrib non-free

sudo apt-get update && apt-get upgrade && apt-get dist-upgrade
lspci | grep -i wire
# 05:00.0 Network controller: Intel Corporation Wireless 3160 (rev 83)
apt-get install network-manager-gnome
apt-get install wpasupplicant
apt-get install wireless-tools
apt install firmware-iwlwifi

apt install firmware-iwlwifi or reboot (/usr/sbin/shutdown -r now)

# WIFI OK HERE
================

sudo apt-get install mate-desktop-environment-extras

======
nano /etc/sudoers

# User privilege specification
root	ALL=(ALL:ALL) ALL
badwolf	ALL=(ALL:ALL) ALL

dpkg-reconfigure lightdm
sudo apt-get install arc-theme
sudo apt-get install gnome-icon-theme

metacity --replace

sudo apt install lightdm-gtk-greeter-settings
Once it’s installed, go to System -> Control Center and search for LightDM GTK+ Greeter.

https://www.mate-look.org/s/Mate/p/1012430

Flat-Remix-Blue-Dark
Material-Black-Blueberry-Numix
Arc-Darkest-Numix or Arc-Darkest-Numix-FLAT

MB-Blueberry-Suru-GLOW panel icon
Black-Slate-Numix icon menu + directory
Suru++Aspromauros and Flat-Remix-Blue-Dark remaining

https://github.com/lah7/ubuntu-mate-colours

Flat-Remix-Blue-Dark

https://www.ravefinity.com/p/vibrancy-colors-gtk-icon-theme.html?m=1
=======

TODO maximize/minimize + home directories style -> vibrancy
MATE problem resizing window (one pixel) -> use metacity

After:
https://www.debian.org/security/
https://www.debian.org/security/audit/tools
https://security-team.debian.org/security_tracker.html

