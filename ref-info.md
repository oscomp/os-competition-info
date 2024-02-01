# 与比赛相关的一些硬件，OS相关的实例/教程的参考信息

### RISC-V 相关文档

- [RISC-V 硬件中文手册](http://crva.ict.ac.cn/documents/RISC-V-Reader-Chinese-v2p1.pdf)

### 赛昉星光二代开发板（RV64）信息
- [社区 Rvspace](https://rvspace.org/)
- [VisionFive 2  SBC](https://rvspace.org/zh/homepage/product_center_sbc)
- [SDK](https://github.com/starfive-tech/VisionFive2)
- [Quick Start Guide](https://doc-en.rvspace.org/VisionFive2/PDF/VisionFive2_QSG.pdf)
- [SDK Quick Start Guide](https://doc-en.rvspace.org/VisionFive2/PDF/VisionFive2_SDK_QSG.pdf)
- [Software Technical Reference Manual](https://doc-en.rvspace.org/VisionFive2/PDF/VisionFive2_SW_TRM.pdf)
- [Debian OS  User Guide](https://wiki.rvspace.org/en/project/VisionFive2_Debian_User_Guide)
- [Debian OS  Release](https://debian.starfivetech.com/)
- [40-Pin GPIO Header User  Guide](https://doc-en.rvspace.org/VisionFive2/PDF/VisionFive2_40-Pin_GPIO_Header_UG.pdf)
- [Datasheet](https://doc-en.rvspace.org/VisionFive2/PDF/VisionFive2_Datasheet.pdf)
- [Accessories](https://rvspace.org/zh/application/Accessories)
- [FAQ](https://doc-en.rvspace.org/VisionFive2/PDF/VisionFive2_FAQ.pdf)
- [RVspace 论坛资料发布，技术答疑](https://forum.rvspace.org/)
- [开源PDF文档:英文版](https://wiki.rvspace.org/en/project/Document_Publish_Status)
- [开源PDF文档:中文版](https://wiki.rvspace.org/zh/project/Document_Publish_Status)
- [Sipeed MAIX Dock开发板硬件说明文档](https://cn.maixpy.sipeed.com/zh/develop_kit_board/maix_dock.html)

### 采用赛昉星光二代开发板（RV64）的部分2023年参赛获奖作品
- [一等奖：北京理工大学-Alien](https://gitlab.eduxiji.net/202310007101563/Alien)
- [二等奖：华中科技大学-AVX](https://gitlab.eduxiji.net/202310487101114/oskernel2023-avx)
- [二等奖：哈尔滨工业大学（深圳）-MankorOS](https://gitlab.eduxiji.net/MankorOS/OSKernel2023-MankorOS)
- [三等奖：武汉大学-AA5555AA](https://gitlab.eduxiji.net/202310486101581/luoos)

### 可以在基于QEMU(RV64)上运行的开源OS：
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


## [2024年以前的相关信息](https://github.com/oscomp/os-competition-info/blob/main/ref-info-before-2024.md)