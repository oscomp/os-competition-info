# proj123-Lwext4-for-XiUOS
### 项目名称

基于XiUOS矽璓工业物联操作系统XiZi内核，移植Lwext4文件系统

### 支持单位

浙江省北大信息技术高等研究院

### 项目描述

Lwext4（Lightweight ext4 filesystem）文件系统是针对微处理器、嵌入式设备进行适配的文件系统，由ext4文件系统优化而来。目前XiUOS已支持FatFs文件系统，为补充XiUOS生态支持，需要新增支持Lwext4文件系统。
项目要求基于XiUOS工程XiZi内核，在挂载存储设备上，如SD卡、USB存储设备，支持Lwext4文件系统挂载和通用的文件系统命令，包括但不限于：
* ls;
* cd;
* rm;
* mv;
* mkdir;
* find。

### 所属赛道

2022全国大学生操作系统比赛的“OS功能挑战”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2021年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2022全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

薛栋梁

* XiUOS gitlink : https://www.gitlink.org.cn/xuos/xiuos

* Lwext4 for XiUOS gitlink : https://www.gitlink.org.cn/xuos/Lwext4_support_XiUOS

* email xuedongliang010@163.com



### 难度

中等

### 特征

* 需了解Lwext4源码架构，整理Lwext4移植接口
* 需了解XiUOS源码架构，尤其是fs文件系统注册流程，以及MountSD、MountUSB等挂载函数调用依赖
* 代码提交分支为https://www.gitlink.org.cn/xuos/Lwext4_support_XiUOS

### 文档

* Lwext4下载：https://sourceforge.net/projects/Lwext4/
* Lwext4源码：https://github.com/gkostka/Lwext4
* XiUOS技术博客：https://blog.csdn.net/AIIT_Ubiquitous

### License

本项目遵循MulanPSL-2.0协议，同时兼容Apache-2.0/BSD/MIT协议，其他协议如果与木兰协议不冲突也可兼容



## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

一、正确运行XiUOS：
选定合适开发板，可参考XiUOS已支持BSP，正确编译、烧写、运行，提供运行成功terminal终端显示即可；

二、适配存储设备：
基于一的工作，支持SD卡、USB等存储设备，提供测试程序，验证存储设备读写功能是否正常；

三、移植Lwext4文件系统：
* 获取Lwext4源码，移植至XiUOS/Ubiquitous/XiZi/fs/Lwext4目录，修改对应的Kconfig、Makefile文件，确保编译成功，提供测试程序，验证Lwext4文件系统读写正常；
* 验证通过后，移植Lwext4代码、测试文档提交PR至https://www.gitlink.org.cn/xuos/Lwext4_support_XiUOS。

四、开源协议检查：
XiUOS遵循MulanPSL-2.0开源协议，Lwext4遵循GPL-2.0开源协议，所有新增代码遵循MulanPSL-2.0，Lwext4源码和参考代码需遵循其GPL-2.0开源协议，避免协议污染。

