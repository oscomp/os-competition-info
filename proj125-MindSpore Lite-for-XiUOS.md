# proj125-MindSpore Lite-for-XiUOS
### 项目名称
基于XiUOS矽璓工业物联操作系统rt-thread内核，移植开发MindSpore Lite 到XiUOS knowing 框架

### 支持单位  （可选内容）
浙江省北大信息技术高等研究院

### 项目描述
MindSpore Lite是一个极速、极智、极简的AI引擎，使能全场景智能应用，为用户提供端到端的解决方案，帮助用户使能AI能力。


### 所属赛道

2022全国大学生操作系统比赛的“OS功能挑战”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2021年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2022全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

* 薛栋梁

* github https://gitlink.org.cn/xuos/xiuos.git

* email xuedongliang010@163.com



### 难度

* 高



### 特征


* 需要了解XiUOS knowing框架以及其对应的Rt-thread 使用。
* XiUOS提交PR分支为prepare_for_master分支
* 需了解XiUOS源码架构，新建目录xiuos/APP_Framework/Framework/knowing/MindSpore_Lite,包括相关测试用例和测试结果文档展示
* 需要了解MindSpore_Lite在MCU部署推理所需的代码



### 文档

* 矽璓网站介绍：http://xuos.io/
* MindSpore 网站：https://www.mindspore.cn/lite?version=/r1.6/
* Rt-thread网站：https://www.rt-thread.org/

### License

* 本项目遵循MulanPSL-2.0协议,同时兼容Apache-2.0/BSD/MIT协议,其他协议如果与木兰协议不冲突也可兼容。



## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

* 一、正确运行XiUOS：
选定合适开发板（rt-thread内核aiit_board目录下的stm32f407_core），可参考XiUOS已支持BSP，正确编译、烧写、运行，提供运行成功terminal终端显示即可；

* 二、移植MindSpore Lite：
获取MindSpore Lite源码，移植至目录xiuos/APP_Framework/Framework/knowing/MindSpore_Lite目录，修改对应的Kconfig、SConscript文件，确保编译成功，提供测试程序，验证MindSpore Lite测试通过；

* 三、开源协议检查：
XiUOS遵循MulanPSL-2.0开源协议，所有新增代码遵循MulanPSL-2.0，MindSpore Lite源码和参考代码需遵循其原有的开源协议，避免协议污染。

## 备注（可选内容）

