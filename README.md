#Feature
For the Serial Console
You can input commands in the serial console.
For the emulated environment
ARMware now can emulate the ARM architecture version 4 Instruction Set.
Add a dynamic compiler.
Add a threaded code optimization technology.


#Brief Introduction
ARMware, like VMware or Bochs, is an emulator for a hardware platform. Opposite to the x86 platform which VMware or Bochs want to emulate, ARMware provides an emulation environment for the ARM platform. It can emulate Intel StrongARM SA-1110 as the core for now (The support for Intel Xscale is been developping). The whole emulated environment which ARMware provides is like HP iPaq H3600 (The future emulation environment for the Intel Xscale will be like HP iPaq H5500).

The hardware components that ARMware can emulate for now are:

ARM architecture version 4 core
Supports all kinds of ARM instruction set (but does not support Thumb instruction set)
Supports all processor mode:
User mode
Fast Interrupt mode
Interrupt mode
Supervisor mode
Abort mode
Undefined Instruction mode
System mode
ARM standard system coprocessor (CP15)
Memory Management Unit (MMU)
Supports all kinds of address translation:
Section translation
Large page translation
Small page translation
Tiny page translation
Supports all kinds of MMU fault:
Translation fault
Domain fault
Access permission fault
Alignemnt fault
Translation Lookaside Buffer (TLB)
In order to increase the performance, I use a hash table and fully associated TLB.
LCD Controller
DMA Controller
EGPIO
Operation System Timer
Reset Controller
Real Time Clock (RTC)
GPIO Controll Block
Interrupt Controller
Power Management
Supports idle mode
Serial Port 1
Connects to Atmel micro-controller
Serial Port 3
Connects to Serial console
Intel StrataFlash J3 Flash ROM
Fully supports Common Flash Interface (CFI)
Fully supports Write State Machine (WSM), including
read array
read ID codes
block lock
block unlock
read status register
read block register
byte/word program
write to buffer
block erase
Using GNU dbm as the ROM file database
Using XML as the ROM file database
Atmel micro-controller
Partially supports, including
Get version information
Get and Set LCD back light
LCD screen
Using Qt
Using Gtk
Touch panel
