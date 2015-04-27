Linux Kernel
============

Like we saw for the :ref:`bootloader <bsp_bootloader_label>`, the first thing you need is: sources.
Get them from *Bitbake* build directory (if you built the kernel with it) or get them from the Internet.

*Bitbake* will place the sources under directory:

.. host::

 | /path/to/build/tmp/work/imx6sxsabresd-poky-linux-gnueabi/linux-imx/3.14.28-r0/git


If you are working with the virtual machine, you will find them under directory:

.. host::

 | /home/@user@/architech_sdk/architech/@board-alias@/yocto/build/tmp/work/imx6sxsabresd-poky-linux-gnueabi/linux-xlnx/3.14.28-r0/git


We suggest you to **don't work under Bitbake build directory**, you will pay a speed penalty and you could
have troubles syncronizing the all thing. Just copy them some place else and do what you have to do.

If you didn't build them already with *Bitbake* or you just want to do make every step by hand, you can
always get them from the Internet by cloning the proper repository and checking out the proper commit.
Check `IMXLINUX: Embedded Linux for i.MX Applications Processors <http://www.freescale.com/webapp/sps/site/prod_summary.jsp?code=IMXLINUX&fsrch=1>`_
