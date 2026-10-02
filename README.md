# Black Box OS

A 64-bit operating system built from scratch for x86-64 systems.

Black Box OS is a long-term operating system development project focused on understanding and implementing the fundamental components of an operating system — from the boot process and kernel to memory management, processes, filesystems, device drivers, networking, and eventually a graphical desktop environment.

## Project Goal

The goal is to build a functional 64-bit operating system from the ground up and understand how each layer interacts with the hardware.

```text
Hardware
   ↓
Bootloader
   ↓
64-bit Kernel
   ↓
Hardware Drivers
   ↓
Memory / Process / File / Device Management
   ↓
System Calls
   ↓
User Space
   ↓
Shell / Applications
   ↓
Graphical Interface
   ↓
Networking
```

## Planned Features

* [ ] Boot process
* [ ] 64-bit kernel
* [ ] CPU management
* [ ] Interrupt handling
* [ ] Memory management
* [ ] Virtual memory and paging
* [ ] Process management
* [ ] CPU scheduling
* [ ] Multitasking
* [ ] System calls
* [ ] Keyboard driver
* [ ] Mouse driver
* [ ] Device management
* [ ] I/O management
* [ ] Filesystem
* [ ] Storage management
* [ ] Inter-process communication
* [ ] User management
* [ ] Security and protection
* [ ] Networking
* [ ] Shell
* [ ] Power management
* [ ] Logging and monitoring
* [ ] Graphical user interface
* [ ] Virtualization support

## Development Roadmap

### Phase 1 — Boot

```text
Power ON
   ↓
Firmware
   ↓
Bootloader
   ↓
64-bit Mode
   ↓
Black Box OS Kernel
```

### Phase 2 — Kernel

* Kernel entry
* GDT
* IDT
* Interrupts
* CPU initialization
* Basic kernel output
* Timer

### Phase 3 — Memory

* Physical memory manager
* Page-frame allocation
* Paging
* Virtual memory
* Kernel heap

### Phase 4 — Processes

* Processes
* Threads
* Context switching
* Scheduler
* Multitasking

### Phase 5 — Filesystem

* Disk access
* Filesystem
* Files
* Directories
* File descriptors
* Read/write operations

### Phase 6 — Drivers

* Keyboard
* Mouse
* Display
* Storage
* Other hardware devices

### Phase 7 — User Space

* System call interface
* Shell
* User programs
* Process isolation
* User permissions

### Phase 8 — Networking

* Network device driver
* Ethernet
* IP
* TCP/UDP
* Sockets
* Network applications

### Phase 9 — Graphical Interface

* Graphics subsystem
* Window management
* Input handling
* Desktop environment
* Applications

## Repository Structure

```text
BlackBoxOS/
│
├── boot/          # Bootloader and early boot code
├── kernel/        # Kernel source code
├── drivers/       # Hardware drivers
├── memory/        # Memory management
├── process/       # Process and thread management
├── fs/             # Filesystem implementation
├── net/            # Networking subsystem
├── user/           # User-space programs
├── include/        # Shared header files
└── scripts/        # Build and development scripts
```

## Development Environment

Black Box OS is currently developed and tested on Ubuntu.

### Tools

* GCC
* NASM
* GNU Make
* QEMU
* GRUB tools
* xorriso
* mtools
* Git

### Target Architecture

```text
Architecture: x86-64
Boot target:  PC / x86-64
Testing:      QEMU
Language:     C + x86-64 Assembly
```

## Development Philosophy

Black Box OS is developed incrementally.

Each subsystem will be implemented, tested, and understood before moving to the next major subsystem.

The project prioritizes understanding how an operating system works internally rather than simply assembling existing operating-system components.

## Current Status

**Stage: Project Initialization**

The repository structure and development environment have been created.

### Current milestone

```text
[✓] Project repository created
[✓] Directory structure created
[✓] Git initialized
[✓] Development tools installed
[ ] First boot
[ ] Kernel startup
[ ] Keyboard input
[ ] Shell
[ ] Filesystem
[ ] Multitasking
[ ] GUI
[ ] Networking
```

## Long-Term Vision

The final goal is a complete operating system capable of:

```text
Booting
   ↓
Running the kernel
   ↓
Managing CPU and memory
   ↓
Running multiple programs
   ↓
Managing files
   ↓
Controlling hardware
   ↓
Providing system calls
   ↓
Providing a shell
   ↓
Supporting networking
   ↓
Providing a graphical desktop
```

## Project

**Black Box OS**

Built from scratch.
Built to understand the machine from the ground up.
