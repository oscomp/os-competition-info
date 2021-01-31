## 与比赛相关的一些硬件，OS相关的实例/教程的参考信息

### RISC-V 硬件文档
- [Kendryte（基于K210芯片）硬件技术规格说明文档](https://github.com/kendryte/kendryte-doc-datasheet/blob/master/zh-Hans/SUMMARY.md)
- [Sipeed MAIX Dock开发板硬件说明文档](https://cn.maixpy.sipeed.com/zh/develop_kit_board/maix_dock.html)
- [RISC-V 硬件中文手册](http://crva.ict.ac.cn/documents/RISC-V-Reader-Chinese-v2p1.pdf)
- [K210 开发板相关问题](https://rcore-os.github.io/rCore-Tutorial-Book-v3/chapter0/6hardware.html#k210)（吴一凡维护）
  - [K210 入门相关资料](https://github.com/wyfcyx/osnotes/blob/master/book/K210相关资料.md)（吴一凡维护）

这里列出了一些可以在基于[K210 CPU](https://github.com/kendryte/kendryte-doc-datasheet)的[Sipeed MAIX Dock开发板](https://item.taobao.com/item.htm?spm=a1z10.1-c-s.w4004-21410578015.7.5a6752b1xJE3v2&id=591616120470)或QEMU(rv64)上运行的开源OS：
- [nommu linux 0.11](https://github.com/lizhirui/K210-Linux0.11)
- [C lang based xv6 kernel](https://github.com/SKTT1Ryze/xv6-k210)
- [Rust lang based xv6 kernel(uncompleted)](https://github.com/Jaic1/xv6-riscv-rust)
- [Rust based rcore tutorial kernel](https://github.com/wyfcyx/rCore-Tutorial/tree/multicore)
- [C lang based uCore kernel](https://github.com/NKU-EmbeddedSystem/riscv64-ucore)
- [RT-Thread/K210 with SMP](https://github.com/RT-Thread/rt-thread/tree/master/bsp/k210)

### Tutorial of developing OS in Rust
- [Writing an OS in Rust (x86)](https://os.phil-opp.com/)
- [The Adventures of OS: Making a RISC-V Operating System using Rust](https://osblog.stephenmarz.com/)
- [rCore-Tutorial-Book 第三版 中文](https://rcore-os.github.io/rCore-Tutorial-Book-v3/)
- [Operating System development tutorials in Rust on the Raspberry Pi](https://github.com/rust-embedded/rust-raspberrypi-OS-tutorials)
- [Book of Drone RTOS in Rust](https://book.drone-os.com/)
  - [Drone OS: An Embedded Operating System written in Rust](https://github.com/drone-os)

### 下面是一些教学用的开源OS：
- [C lang based xv6 on x86](https://github.com/mit-pdos/xv6-public)
- [C lang based xv6 on risc-v](https://github.com/mit-pdos/xv6-riscv)
- [Rust based blogos on x86](https://github.com/phil-opp/blog_os)
- [Rust based osblog on x86](https://github.com/sgmarz/osblog)
- [C/Rust based os kernel lab](https://github.com/chyyuu/os_kernel_lab)
- [rCore-Tutorial-v3](https://github.com/rcore-os/rCore-Tutorial-v3)

### 开发OS相关的信息
- [OSDEV 讨论如何开发OS的WIKI社区](https://wiki.osdev.org/Main_Page)

### 固件（Firmware）：Bootloader/BIOS/UEFI/OpenSBI等相关
- 符合OpenSBI接口的开源固件
  - [Rust based SBI](https://github.com/luojia65/rustsbi)


### RISC-V 系统功能级模拟器（支持运行OS kernel）
- [qemu](https://www.qemu.org/)
- [Spike RISC-V ISA Simulator](https://github.com/riscv/riscv-isa-sim)
- [rvemu](https://github.com/d0iasm/rvemu): simple, on web
  - [Eng Book: Writing a RISC-V Emulator in Rust](https://book.rvemu.app/)
  - [Made a RISC-V Emulator Running Xv6 in Eng](https://d0iasm.github.io/blog/risc-v/2020/04/03/xv6-on-my-riscv-emulator.html)
- [riscv-rust](https://github.com/takahirox/riscv-rust): on web, with debug
- [TinyEMU](https://bellard.org/tinyemu/): simple
  - [MARSS-RISCV: Cycle-level Micro-Architectural System Simulator for RISC-V on top of TinyEMU](https://github.com/bucaps/marss-riscv)
- [rv8](https://github.com/rv8-io/rv8): fast
- [terminus](https://github.com/shady831213/terminus)：multicore,virtio-net/disk/mouse/console...
- [Rips](https://github.com/mortbopet/Ripes) ： with nice gui interface...
- [MARSS-RISCV (Micro-ARchitectural System Simulator - RISCV)](https://github.com/bucaps/marss-riscv)
  - MARSS-RISCV is an open-source, cycle-level single-core full-system (Linux) micro-architectural simulator for the RISC-V ISA 

### 其他RISC-V模拟器
- [Web界面时钟周期级的RISC-V CPU](http://x.dii.unisi.it:8098/~giorgi/WebRISC-V/index.php)
