## Welcome to the Arduino/Genuino 101 Revival Project!

We are aiming to modernize the Arduino 101 software stack. Currently planned things include:
- Organize the scattered and mostly abandoned repositories into something neater.
- Update the compiler/toolchain to the latest gcc releases. (Synopsys maintains a downstream gcc compiler for ARC cores [here](https://github.com/foss-for-synopsys-dwc-arc-processors/toolchain), upstream gcc should be usable for the x86 core.)
- Port to latest Zephyr. Support for the board seems to have been removed in version 1.14.0.
- Attempt to free up RAM and storage. With the existing stack, only 24 KB RAM out of 80 KB and 196 KB storage out of 384 KB are available to the user. The rest is taken up by the RTOS or the bootloader.
- Enable easy code execution on the nRF51822 bluetooth controller built into the Curie module. It has its own ARM Cortex M0 core, 16 KB RAM and 256 KB of flash. Its datasheet and software stack seems to be available. More digging is necessary.

We want to keep backward compatibility (not as in ABI compatibility, recompiling might be necessary) with existing code as much as possible.
