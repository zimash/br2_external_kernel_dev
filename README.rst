 .. To view this document in the terminal, you must use "rst2man README.rst | man -l -".

==========
README.rst
==========

Using
=====

Clone mainstream Buildroot, current repo and make with external tree defconfig. ::

  $ git clone https://git.busybox.net/buildroot
  $ git clone https://github.com/zimash/br2_external_kernel_dev
  $ cd buildroot
  $ make BR2_EXTERNAL=../br2_external_kernel_dev qemu_x86_64_dev_defconfig
  $ make menuconfig # If we want to change Buildroot options
  $ make linux-menuconfig # If we want to change Linux Kernel options
  $ make # Build it

The qemu/x86_64 configuration was taken as the basis for the current board and configs.
