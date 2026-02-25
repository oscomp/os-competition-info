# proj-JerryScript-for-XiUOS
### 项目名称
基于XiUOS矽璓工业物联操作系统XiZi内核，移植开发JerryScript

### 支持单位  
浙江省北大信息技术高等研究院

### 项目描述
JerryScript 是一个轻量级的 JavaScript 引擎，它可以运行在受限制的设备上，例如微控制器，它能在 RAM < 64 KB， ROM < 200 KB 的设备上运行。


### 所属赛道

2023全国大学生操作系统比赛的“OS功能挑战”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2022年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2023全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

* 刘伟超

* github https://gitlink.org.cn/xuos/xiuos.git

* email iacu2016@163.com



### 难度

* 低



### 特征


* 需要了解XiUOS 内核的XiZi的使用
* XiUOS提交PR分支为prepare_for_master分支
* 需了解XiUOS源码架构，新建目录xiuos/APP_Framework/lib/JerryScript，包括相关测试用例和测试结果文档展示
* 项目提供基于ARM架构的矽璓硬件终端，片上ROM 512KB，Flash 2MB



### 文档

* 矽璓网站介绍：http://xuos.io/
* JerryScript网站：https://jerryscript.net/



### License

* 本项目遵循MulanPSL-2.0协议，同时兼容Apache-2.0/BSD/MIT协议，其他协议如果与木兰协议不冲突也可兼容。



## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

* 一、正确运行XiUOS：
XiUOS中XiZi BSP板级支持包为hc32f4a0，正确编译、烧写、运行，提供运行成功terminal终端显示即可；

* 二、移植JerryScript：
获取JerryScript源码，移植至目录xiuos/APP_Framework/lib/JerryScript目录，修改对应的Kconfig、Makefile文件，确保编译成功，提供测试程序，验证JerryScript测试通过；

* 三、开源协议检查：
XiUOS遵循MulanPSL-2.0开源协议，所有新增代码遵循MulanPSL-2.0，MindSpore Lite源码和参考代码需遵循其原有的开源协议，避免协议污染。

## 备注（可选内容）