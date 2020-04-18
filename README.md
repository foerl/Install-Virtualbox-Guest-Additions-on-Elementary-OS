# Install-Virtualbox-Guest-Additions-on-Elementary-OS


sudo apt-get update;sudo apt-get upgrade;sudo apt-get dist-upgrade

sudo apt-get install build-essential module-assistant

# Prepare your system for building kernel module

sudo m-a prepare

# insert Devices > Insert Guest Additions CD image.

blkid

sudo mkdir /media/cdrom

sudo mount /dev/sr0 /media/cdrom

cd /media/cdrom

sudo sh VBoxLinuxAdditions.run

sudo reboot
