During, I tried to reset the package DB. These commands are available by
default (on TurnKey) and should hopefully do the trick::

    echo RESET grub-pc/install_devices | debconf-communicate grub-pc

Or::

   echo UNREGISTER grub-pc/install_devices | debconf-communicate grub-pc

Alternatively all questions realted to the package can be removed like
this::

   echo PURGE | debconf-communicate grub-pc
