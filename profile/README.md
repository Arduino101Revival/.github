## Welcome to the Arduino/Genuino 101 Revival Project!

We are aiming to modernize the Arduino 101 software stack. Currently planned things include:
- Organize the scattered and mostly abandoned repositories into something neater.
- Update the compiler/toolchain to the latest gcc releases. (Synopsys maintains a downstream gcc compiler for ARC cores [here](https://github.com/foss-for-synopsys-dwc-arc-processors/toolchain), upstream gcc should be usable for the x86 core.)
- Port to latest Zephyr. Support for the board seems to have been removed in version 1.14.0.

We want to keep backward compatibility (not as in ABI compatibility, recompiling might be necessary) with existing code as much as possible.
