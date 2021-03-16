This repo contains the script:

     preconfigure_grub

This script checks if the grub-pc package 'install_devices' item is
configured. If it is, it exits and disables itself (i.e. chmod -x).

If the grub-pc package 'install_devices' item is not configured, it will
attempt to discover which devices grub is actually installed to.

If it is able to determine where grub is installed, it configures the
grub-pc package 'install_devices' item. It then disables itself and
exits.

If it is not able to determine where grub is installed, it notes that
and exits.
