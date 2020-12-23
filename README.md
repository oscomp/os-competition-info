# "全国大学生操作系统比赛2021"相关信息
## 事件
- 2020.12.26 [关于2021全国大学生操作系统比赛的研讨会](https://www.bagevent.com/event/7056666)


## [比赛章程](https://shimo.im/docs/N2A1M8vV47cJP5AD/)

## [比赛技术方案](https://shimo.im/docs/Wr3DVevExDc8wDkJ)

## 相关网站
- [全国高等院校计算机系统能力培养官方网站](http://www.csc-he.com)
- ["龙芯杯"CPU比赛](http://www.nscscc.org)
- ["华为毕昇杯"编译比赛](https://course.educg.net/acm/)

## 与比赛相关的一些OS实例/教程的参考信息

这里列出了一些可以在基于[K210 CPU](https://github.com/kendryte/kendryte-doc-datasheet)的[Sipeed MAIX Dock开发板](https://item.taobao.com/item.htm?spm=a1z10.1-c-s.w4004-21410578015.7.5a6752b1xJE3v2&id=591616120470)或QEMU(rv64)上运行的开源OS：
- [nommu linux 0.11](https://github.com/lizhirui/K210-Linux0.11)
- [C lang based xv6 kernel](https://github.com/SKTT1Ryze/xv6-k210)
- [Rust lang based xv6 kernel(uncompleted)](https://github.com/Jaic1/xv6-riscv-rust)
- [Rust based rcore tutorial kernel](https://github.com/wyfcyx/rCore-Tutorial/tree/multicore)
- [C lang based uCore kernel](https://github.com/NKU-EmbeddedSystem/riscv64-ucore)

### Tutorial of developing OS 
- [Writing an OS in Rust (x86)](https://os.phil-opp.com/)
- [The Adventures of OS: Making a RISC-V Operating System using Rust](https://osblog.stephenmarz.com/)
- [rCore-Tutorial-Book 第三版 中文](https://rcore-os.github.io/rCore-Tutorial-Book-v3/)

### 下面是一些教学用的开源OS：
- [C lang based xv6 on x86](https://github.com/mit-pdos/xv6-public)
- [C lang based xv6 on risc-v](https://github.com/mit-pdos/xv6-riscv)
- [Rust based blogos on x86](https://github.com/phil-opp/blog_os)
- [Rust based osblog on x86](https://github.com/sgmarz/osblog)
- [C/Rust based os kernel lab](https://github.com/chyyuu/os_kernel_lab)
- [rCore-Tutorial-v3](https://github.com/rcore-os/rCore-Tutorial-v3)

这里列出符合SBI接口的开源固件
- [Rust based SBI](https://github.com/luojia65/rustsbi)


### RISC-V 系统功能级模拟器（支持运行OS kernel）
- [qemu](https://www.qemu.org/)
- [Spike RISC-V ISA Simulator](https://github.com/riscv/riscv-isa-sim)
- [rvemu](https://github.com/d0iasm/rvemu): simple, on web
- [riscv-rust](https://github.com/takahirox/riscv-rust): on web, with debug
- [TinyEMU](https://bellard.org/tinyemu/): simple
  - [MARSS-RISCV: Cycle-level Micro-Architectural System Simulator for RISC-V on top of TinyEMU](https://github.com/bucaps/marss-riscv)
- [rv8](https://github.com/rv8-io/rv8): fast
- [terminus](https://github.com/shady831213/terminus)：multicore,virtio-net/disk/mouse/console...
- [Rips](https://github.com/mortbopet/Ripes) ： with nice gui interface...

### 其他RISC-V模拟器
- [Web界面时钟周期级的RISC-V CPU](http://x.dii.unisi.it:8098/~giorgi/WebRISC-V/index.php)
