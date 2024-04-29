# Minimalist 32-bit Kernel

The first thing you should do is set up a [GCC Cross-Compiler](https://wiki.osdev.org/GCC_Cross-Compiler) for i686-elf

After doing the above, you should have a cross compiler installed along with all the dependencies you would need to run this project

Run `make` to build the project

Install QEMU, then use the following command to start the operating system:

`qemu-system-i386 -cdrom myos.iso`

Additionally, QEMU supports booting multiboot kernels directly without bootable medium:

`qemu-system-i386 -kernel myos.bin`

