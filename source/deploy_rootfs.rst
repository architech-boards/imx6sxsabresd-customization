.. warning::

 The following instruction will make you overwrite your SD card content, it will be lost forever!
 If you have important data on it, make sure you do a backup of your data on the SD card before
 catching up with the next steps.

An SD card image provides the full system to boot with U-Boot and kernel. To flash an SD card image, run the following
command:


.. host::

 | sudo dd if=core-image-minimal-@board-alias@-dev.sdcard of=/dev/sd<partition> bs=1M


.. important::

 sudo password is **@user-password@**

Make sure everything has been written on the SD card:

.. host::

 | sync

and unmount the SD card from your system.

