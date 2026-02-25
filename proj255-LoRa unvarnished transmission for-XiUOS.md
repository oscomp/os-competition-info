# pro255--LoRa unvarnished transmission for-XiUOS

### 项目名称
基于XiUOS矽璓工业物联操作系统XiZi内核，开发支持LoRa到RS485接口的数据透传功能。

### 支持单位  
浙江省北大信息技术高等研究院

### 项目描述
本项目实现 lora 与 RS485 接口的数据透传，接收 RS485 数据，并通过 Lora 传送出去，接收 lora 的数据，通过 RS485 发出去。在数据跨介质的传输过程中,不发生改变.


### 所属赛道

2024全国大学生操作系统比赛的“OS功能挑战”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2024年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2024全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

* 田春雨

* github https://gitlink.org.cn/xuos/xiuos.git

* email chunyexixiaoyu@163.com

* wechat  fortunerains



### 难度

* 中



### 特征

* 需要了解XiUOS 内核的XiZi的使用
* XiUOS提交PR分支为[prepare_for_master分支](https://www.gitlink.org.cn/xuos/xiuos/tree/prepare_for_master)
* 需了解XiUOS源码架构，新建目录xiuos/APP_Framework/Applications/LoRa_RS485，包括相关测试用例和测试结果文档展示
* 项目提供基于ARM架构的矽璓硬件终端，在其上编译、烧写、运行的详细步骤[请参考](https://www.gitlink.org.cn/xuos/xiuos/tree/prepare_for_master/Ubiquitous%2FXiZi_IIoT%2Fboard%2Fedu-arm32)



### 文档

* 矽璓网站介绍：http://xuos.io/



### License

* 本项目遵循MulanPSL-2.0协议，同时兼容Apache-2.0/BSD/MIT协议，其他协议如果与木兰协议不冲突也可兼容。



## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

* 一、LoRa到RS485数据透传：
  利用另外的相关LoRa模块或者设备，向ARM架构的矽璓硬件终端发送数据，该终端RS485外接usb转串口模块到个人PC，验证是否可以实现透传功能，提供功能源码和测试程序，验证通过；
* 二、RS485到LoRa数据透传：
ARM架构的矽璓硬件终端的RS485外接usb转串口至个人PC，个人PC串口软件向对于的RS485接口写入数据，通过LoRa模块向外转发，利用另外的LoRa模块或者设备查看是否为RS485写入的数据，从而验证透传功能，提供功能源码和测试程序，验证通过；
* 三、开源协议检查：
XiUOS遵循MulanPSL-2.0开源协议，所有新增代码遵循MulanPSL-2.0，源码和参考代码需遵循其原有的开源协议，避免协议污染。

## 备注（可选内容）
