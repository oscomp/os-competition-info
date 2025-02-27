# 与比赛相关的一些硬件，OS相关的实例/教程的参考信息
## 内核实现赛道涉及的QEMU模拟器、编译器工具信息
- [2025年OS比赛内核实现赛道题目仓库中的赛题评测指南](https://github.com/oscomp/testsuits-for-oskernel/tree/pre-2025/?tab=readme-ov-file#%E8%B5%9B%E9%A2%98%E8%AF%84%E6%B5%8B%E6%8C%87%E5%8D%97)给出了详细信息
  - QEMU-9.2.1
## 与操作系统相对无关的内核核心组件
### 硬件抽象层相关组件
- [rtthread内核为参考例子的C-based 多种HAL](https://github.com/RT-Thread/rt-thread/tree/master)
  - [RISC-V64/32](https://github.com/RT-Thread/rt-thread/tree/master/libcpu/risc-v)
  - [LoongArch64](https://freeflyingsheep.github.io/posts/rt-thread/loongarch64/)
  - [LoongArch32](https://freeflyingsheep.github.io/posts/rt-thread/loongarch32/)
  - [ARM aarch64](https://github.com/RT-Thread/rt-thread/tree/master/libcpu/aarch64)
  - [arm32](https://github.com/RT-Thread/rt-thread/tree/master/libcpu/arm)
- [Rust-based HAL: 支持RISC-V64, LoongArch64, x86-64, ARM aarch64](https://github.com/oscomp/arceos/tree/main/modules/axhal)

  - [starry-next宏内核参考例子](https://github.com/oscomp/starry-next) ：对 2025 年 OS 比赛已经初步完成了环境适配，能够运行 riscv64 和 loongarch64 的大部分 basic 测例，并可以支持在OS内核赛道比赛平台上进行评测。
  - [可在OS比赛平台上运行的改造代码仓库](https://gitlab.eduxiji.net/Azure_stars/starry-next/-/tree/pre2025test)（相比于 github 仓库进行了一些环境配置的改变）
  - [starry-next 内核使用说明](https://azure-stars.github.io/Starry-Tutorial-Book/ch01-00.html)
  - [如何在 OS 比赛平台上测试 Starry 的说明](https://azure-stars.github.io/Starry-Tutorial-Book/ch01-00.html)
  - [starry-next所基于的arceos unikernel参考内核](https://github.com/oscomp/arceos)

### 文件系统相关组件
#### ext4文件系统参考实现
- [C-based lwext4库](https://github.com/gkostka/lwext4)
  - [这个C库的起源来自 helenOS](http://helenos.org/)
  - [修改并使用此C库的RT-Thread OS](https://packages.rt-thread.org/en/detail.html?package=lwext4)
- [封装了C-based lwext4的Rust-based ext4 Crate](https://github.com/rcore-os/lwext4_rust/tree/main)
  - [使用此库的StarryOS](https://github.com/Starry-OS/Starry)
  - [使用此库的ByteOS](https://github.com/Byte-OS/ByteOS)
- [Rust-based ext4 Crate](https://github.com/yuoo655/ext4_rs)
  - [使用此库的StarryOS](https://github.com/Starry-OS/Starry)

### TCP/IP协议栈相关组件
- C based
  - [lwip](https://github.com/lwip-tcpip/lwip)
  - [CycloneTCP](https://github.com/Oryx-Embedded/CycloneTCP)
- Rust based
  - [Rust-based tcpip stack: smoltcp](https://github.com/rcore-os/smoltcp)
  - [Rust封装C-based tcpip stack:lwip](https://github.com/Centaurus99/arceos-lwip)

### 可用于QEMU的设备驱动相关组件
- [virtio drivers](https://github.com/rcore-os/virtio-drivers): Block, NIC, GPU, Input, Console ... Drivers

**注1：2025决赛阶段的内核实现赛道比赛，测试用例所在文件系统格式为Ext4， 上面提供的C和Rust的Ext4库与具体OS无关，经过适配后，可集成到各种OS中。**

**注2：2025决赛阶段的内核实现赛道比赛，操作系统内核要求能支持RISC-V 64和 LoongArch64，在必须遵循2025OS比赛技术方案的比赛要求（请仔细阅读）下，上面的或相关的符合开源协议的源代码可参考、引用、复制。**

## RISC-V相关参考信息
### RISC-V 相关文档

- [RISC-V 硬件中文手册](https://github.com/oscomp/books/blob/main/RISC-V-Reader-Chinese-v2p12017.pdf)

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
- [二等奖：西北工大-npucore+](https://gitlab.eduxiji.net/202310699101073/oskernel2023-npucore-plus)
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

### 与OS无关的kernel components
这是部分与OS无关的kernel components，有一些不一定特别完善，供参考、引用或改进

- [与OS无关且支持x64/aarch64/riscv64/loongarch64，以及星光二代开发板和龙芯2k1000的处理器抽象层Crates: PolyHAL](https://github.com/Byte-OS/polyhal)
- [基于C的ext4 crate](https://github.com/rcore-os/lwext4_rust)
- [基于Rust的ext4 crate](https://github.com/yuoo655/ext4_rs)
- [Rust-based tcpip stack: smoltcp](https://github.com/rcore-os/smoltcp)
- [C-based tcpip stack:lwip](https://github.com/Centaurus99/arceos-lwip)
- [virtio drivers](https://github.com/rcore-os/virtio-drivers): Block, NIC, GPU, Input, Console ... Drivers
- [e1000 NIC driver](https://github.com/rcore-os/e1000-driver)
- [Cadence Macb ethernet driver on Sifive fu740 board](https://github.com/rcore-os/cadence-macb-driver)
- [RISC-V星光二代开发板的网卡驱动](https://github.com/yuoo655/visionfive2_net_driver)
- [RISC-V星光二代开发板的SD卡驱动](https://github.com/os-module/visionfive2-sd) 
- [nvme driver](https://github.com/rcore-os/nvme_driver)
- [isomorphic_drivers](https://github.com/rcore-os/isomorphic_drivers)
- [os scheduler](https://github.com/131131yhx/arceos)
- [os memory malloc subsystem](https://github.com/rcore-os/mem_malloc_subsystem)

### 开发OS过程中形成的kernel components
- [开发unikernel Arceos形成的crates](https://github.com/Arceos-crates/.github/blob/main/README.md)
- [开发宏内核 ByteOS形成的crates](https://github.com/Byte-OS/.github/blob/main/README.md)
 
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

## LoongArch相关参考信息

### 内核赛道选用的2K1000开发板参考资料

- [开发板资料包 *提取码：1111* ](https://pan.baidu.com/s/1yWOJT8TD1tLlNtY6UW_QFQ?pwd=1111)。其中包括但不限于开发板和2k1000处理器用户手册，主板设计资料，uboot、内核和文件系统二进制以及源代码等信息。
- [在线论坛](https://bbs.elecfans.com/group_1650)
- [开发者社区](gitee.com/loongarch_community)
- [2k1000LA 开发板套件](https://m.tb.cn/h.5sYX3Ja?tk=m0U1WjTPIUW)
- [龙芯2K1000LA处理器用户手册_V1.0](https://github.com/LoongsonLab/oscomp-documents/blob/main/pdf/%E9%BE%99%E8%8A%AF2K1000LA%E5%A4%84%E7%90%86%E5%99%A8%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C_V1.0.pdf)
- [龙芯2K1000星云板用户手册V1.1](https://github.com/LoongsonLab/oscomp-documents/blob/main/pdf/%E5%B9%BF%E4%B8%9C%E9%BE%99%E8%8A%AF2K1000%E6%98%9F%E4%BA%91%E6%9D%BF%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8CV1.1.pdf)

### LoongArch架构通用文档

- [龙芯架构参考手册](https://github.com/LoongsonLab/oscomp-documents/blob/main/pdf/%E9%BE%99%E8%8A%AF%E6%9E%B6%E6%9E%84%E5%8F%82%E8%80%83%E6%89%8B%E5%86%8C%E5%8D%B7%E4%B8%80.pdf)
- [《计算机体系结构基础(第三版)》](https://github.com/LoongsonLab/oscomp-documents/blob/main/pdf/%E8%AE%A1%E7%AE%97%E6%9C%BA%E4%BD%93%E7%B3%BB%E7%BB%93%E6%9E%84%E5%9F%BA%E7%A1%80(LoongArch)-3rd.pdf)
- [LoongArch 系统调用(syscall)ABI](https://github.com/LoongsonLab/oscomp-documents/blob/main/pdf/LoongArch%20%E7%B3%BB%E7%BB%9F%E8%B0%83%E7%94%A8(syscall)ABI.pdf)
- [LoongArch-工具链约定](https://github.com/LoongsonLab/oscomp-documents/blob/main/pdf/LoongArch-%E5%B7%A5%E5%85%B7%E9%93%BE%E7%BA%A6%E5%AE%9A.pdf)
- [LoongArch ELF ABI(中文版)](https://github.com/LoongsonLab/oscomp-documents/blob/main/pdf/LoongArch-ELF-ABI-CN.pdf)
- 更多龙架构相关文档，可以参考[龙芯开源社区](http://loongnix.cn)，[龙芯中科公司官网](https://loongson.cn/)，[龙芯在github的官方账号](https://github.com/loongson)以及[龙芯实验室为大赛设置的文档仓库](https://github.com/LoongsonLab/oscomp-documents)

### 模拟器

- [QEMU模拟器](https://qemu.org)已经对LoongArch提供了较好的支持。我们正在致力于完善高度仿真大赛主板的2k1000版本QEMU，目前[这个版本](https://github.com/LoongsonLab/2k1000-materials/releases/tag/qemu-static-20240126)可以运行原生的uboot和内核。该版本基于较老的qemu开发，我们正在将其移植到上游最新版本，后续会开源发布。

### LoongArch上可以运行的参考OS
- [Starry OS](https://github.com/LoongsonLab/StarryOS-LoongArch.git)。StarryOS LoongArch版会持续更新。
- [mit xv6-loongarch](https://github.com/skt-cpuos/xv6-loongarch-exp)。 xv6 是MIT开发的一个类Unix教学操作系统，与Linux或BSD不同，xv6非常简单，足以在一个学期内讲完，但仍包含Unix的重要概念和组织结构。xv6被全世界很多高校用于操作系统教学。 开发者： 深圳大学罗老师。 含OS代码、实验代码、实验指导书和PPT演示资料，可以直接用于操作系统教学。
- [mit xv6-labs](https://github.com/Fan33oo/xv6-labs-loongarch). 本项目是xv6-labs-2021相关实验在LoongArch平台的参考实现。具体的实验设计参见xv6主页 的labs标签页。
- [uCore] (https://github.com/cyyself/ucore-loongarch32).  [实验指导书](https://cyyself.github.io/ucore_la32_docs)
- [rCore](https://github.com/Godones/rCoreloongArch). 2022年全国大学生操作系统大赛-功能挑战赛二等奖。
- [MaQueOS](https://gitee.com/dslab-lzu/maqueos). 本项目是用于兰州大学的教学操作系统，兰州大学相关团队为其编写了教材《MaQueOS：基于龙芯LoongArch架构的教学版操作系统》。
- [Yocto](https://www.yoctoproject.org/). Yocto是用于定制嵌入式Linux系统的主流工具之一，它已经支持LoongArch.
- [seL4](https://github.com/tyyteam/la-seL4). 2022年全国大学生操作系统大赛-功能挑战赛一等奖。
- [NuttX](https://github.com/LA-NuttX). NuttX是完全兼容Posix和ANSI标准的嵌入式实时系统，有着轻量级、定制化的特点，已被广泛应用在成熟的商业系统或软件中，如小米Vela系统、三星Tizen RT系统、px4飞行控制软件。

###  LoongArch上可以运行的内核模块
- [与OS无关且支持x64/aarch64/riscv64/loongarch64，以及星光二代开发板和龙芯2k1000的处理器抽象层Crates: PolyHAL](https://github.com/Byte-OS/polyhal)

## 其它参考信息
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

### [2024年以前的各种参考实现的相关信息](https://github.com/oscomp/os-competition-info/blob/main/ref-info-before-2024.md)
### [2024年的各种参考实现的相关信息](https://github.com/oscomp/os-competition-info/blob/main/ref-info-2024.md)
