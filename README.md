# Basic 32-bit Kernel

This project aims to create a bootable OS with a very minimalistic kernel. See my other project, [32_bit_kernel](https://github.com/jammel-yeboah/32_bit_kernel), which I'm currently working on, for a more robust and improved version of this kernel

### Booting the OS
The first thing you should do is set up a [GCC Cross-Compiler](https://wiki.osdev.org/GCC_Cross-Compiler) for i686-elf

After doing the above, you should have a cross compiler installed along with all the dependencies you would need to run this project

Run `make` to build the project

Install QEMU, then use the following command to start the operating system:

`qemu-system-i386 -cdrom myos.iso`

Additionally, QEMU supports booting multiboot kernels directly without bootable medium:

`qemu-system-i386 -kernel myos.bin`
