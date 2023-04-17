## 与比赛相关的一些硬件，OS相关的实例/教程的参考信息

### RISC-V 硬件文档
- [Kendryte（基于K210芯片）硬件技术规格说明文档](https://github.com/kendryte/kendryte-doc-datasheet/blob/master/zh-Hans/SUMMARY.md)
- [Sipeed MAIX Dock开发板硬件说明文档](https://cn.maixpy.sipeed.com/zh/develop_kit_board/maix_dock.html)
- [RISC-V 硬件中文手册](http://crva.ict.ac.cn/documents/RISC-V-Reader-Chinese-v2p1.pdf)
- [K210 开发板相关问题](https://rcore-os.github.io/rCore-Tutorial-Book-v3/chapter0/6hardware.html#k210)（吴一凡维护）
  - [K210 入门相关资料](https://github.com/wyfcyx/osnotes/blob/master/book/K210相关资料.md)（吴一凡维护）
- [信息收集：与RISCV相关的在线课程](https://github.com/rcore-os/rCore/wiki/os-tutorial-summer-of-code#step-1-%E8%87%AA%E5%AD%A6risc-v%E7%B3%BB%E7%BB%9F%E7%BB%93%E6%9E%84%E5%A4%A7%E7%BA%A67%E5%A4%A9)
- [SDK in github](https://github.com/kendryte)
- [Kentryte Developer](https://canaan-creative.com/developer)
- [Bilibil演示视频](https://search.bilibili.com/all?keyword=K210)
- [Youtube演示视频](https://www.youtube.com/results?search_query=K210)

这里列出了一些可以在基于[K210 CPU](https://github.com/kendryte/kendryte-doc-datasheet)的[Sipeed MAIX Dock开发板](https://item.taobao.com/item.htm?spm=a1z10.1-c-s.w4004-21410578015.7.5a6752b1xJE3v2&id=591616120470)或QEMU(rv64)上运行的开源OS：
- [nommu linux 0.11](https://github.com/lizhirui/K210-Linux0.11)
- [C lang based xv6 kernel](https://github.com/SKTT1Ryze/xv6-k210)
- [Rust lang based xv6 kernel(uncompleted)](https://github.com/Jaic1/xv6-riscv-rust)
- [Rust based rcore tutorial kernel](https://github.com/wyfcyx/rCore-Tutorial/tree/multicore)
- [C lang based uCore kernel](https://github.com/NKU-EmbeddedSystem/riscv64-ucore)
- [RT-Thread/K210 with SMP](https://github.com/RT-Thread/rt-thread/tree/master/bsp/k210)
- [rCore-Tutorial-v3](https://github.com/rcore-os/rCore-Tutorial-v3)
  - [一步一步写rCore-Tutorial v3 OS Kernel的实验指导书](https://github.com/rcore-os/rCore-Tutorial-Book-v3) 

### Tutorial of developing OS for RV/x86 in C
- [xv6 riscv book MIT](https://github.com/mit-pdos/xv6-riscv-book)
- [基于代理内核PKE rv64 的实验指导书 华中](https://gitee.com/syivester/pke-doc)
- [ucore rv64 实验指导书 南开](https://nankai.gitbook.io/ucore-os-on-risc-v64/)
- [计算机系统基础实验指导(包含x86/arm/rv) 南大](https://nju-projectn.github.io/ics-pa-gitbook/ics2020/)
- [ucore rv32 实验指导书 较老](https://ring00.github.io/bbl-ucore/#/)
- [肖政杭同学完成 uCore x86 实验的详细笔记](https://kiprey.github.io/2020/08/uCore-1/)
 
### Tutorial of developing OS for RV/x86/ARM in Rust
- [Writing an OS in Rust (x86)](https://os.phil-opp.com/)
- [The Adventures of OS: Making a RISC-V Operating System using Rust](https://osblog.stephenmarz.com/)
- [rCore-Tutorial-Book 第三版 中文](https://rcore-os.github.io/rCore-Tutorial-Book-v3/)
- [Operating System development tutorials in Rust on the Raspberry Pi](https://github.com/rust-embedded/rust-raspberrypi-OS-tutorials)
- [Book of Drone RTOS in Rust](https://book.drone-os.com/)
  - [Drone OS: An Embedded Operating System written in Rust](https://github.com/drone-os)
- [BookOS (x86)](https://www.book-os.org/)
  - [BookOS repo](https://github.com/hzcx998/xbook2)
- [信息收集：用RUST进行系统编程的自学资源](https://github.com/rcore-os/rCore/wiki/study-resource-of-system-programming-in-RUST)

### 下面是一些教学用的开源OS：
- [C lang based xv6 on x86](https://github.com/mit-pdos/xv6-public)
- [C lang based xv6 on risc-v](https://github.com/mit-pdos/xv6-riscv)
- [Rust based blogos on x86](https://github.com/phil-opp/blog_os)
- [Rust based osblog on x86](https://github.com/sgmarz/osblog)
- [C/Rust based os kernel lab](https://github.com/chyyuu/os_kernel_lab)
- [rCore-Tutorial-v3](https://github.com/rcore-os/rCore-Tutorial-v3)
- [BookOS on x86](https://github.com/hzcx998/xbook2)

### 开发OS相关的信息
- [OSDEV 讨论如何开发OS的WIKI社区](https://wiki.osdev.org/Main_Page)

### 固件（Firmware）：Bootloader/BIOS/UEFI/OpenSBI等相关
- 符合OpenSBI接口的开源固件
  - [Rust based SBI](https://github.com/rustsbi/rustsbi)


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
