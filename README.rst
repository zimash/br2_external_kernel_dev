==========
README.rst
==========

Using
=====

Clone mainstream Buildroot and make with external tree defconfig.
.. code-block:: bash
$ git clone https://git.busybox.net/buildroot
$ git clone https://github.com/zimash/br2_external_kernel-dev
$ cd buildroot
$ make BR2_EXTERNAL=../br2_external_kernel_dev qemu_x86_64_dev_defconfig
$ make menuconfig # If we want to change Buildroot options
$ make linux-menuconfig # If we want to change Linux Kernel options
$ make # Build it
