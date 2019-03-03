# routerbootstrap
I'm using an x86_64 based Linux router that runs Debian. Periodically, I want
to re-install a clean image on the router that I can put on it using dd. This
allows for consistency and good automation. This is what routerbootstrap is
for: Based off a Debian netinst ISO image, it creates a QEmu VM and a clean
disk image, then modifies/remasters the ISO image to use automated
installation. It opens up a local webserver at which it serves the Debian
preseed file to the installer. After installation, it runs a couple of scripts
to finish up the system in the configuration that I want it to run at.

## Prerequisites
Python3, mkisofs, QEmu and a Debian Netinst ISO image.

## License
GNU GPL-3.
