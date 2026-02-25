# proj252-CoAP-for-XiUOS
### 项目名称
基于XiUOS矽璓工业物联操作系统XiZi内核，开发支持CoAP协议

### 支持单位  
浙江省北大信息技术高等研究院

### 项目描述
CoAP 是一种在物联网领域应用较广泛的类 HTTP 的协议，通常部署在资源受限的物联网设备上，具体详细标准参考 RFC 7252，其特性在于：

- 基于消息模型

- 传输层基于 UDP 协议

- 使用类似 HTTP 请求的请求/响应模型，CoAP 采用二进制格式，比 HTTP 更加紧凑

- 支持双向通信

- 轻量、低功耗

- 支持可靠传输，数据重传，块传输，确保数据可靠到达

- 支持 IP 多播

- 支持观察模式

- 支持异步通信

- 本项目基于XiUOS实现CoAP协议栈，运行在MCU环境。


### 所属赛道

2024全国大学生操作系统比赛的“OS功能挑战”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2024年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2024全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

* 刘伟超

* github https://gitlink.org.cn/xuos/xiuos.git
* email iacu2016@163.com
* wechat liuweichao292070



### 难度

* 中



### 特征

* 需要了解XiUOS 内核的XiZi的使用
* XiUOS提交PR分支为[prepare_for_master分支](https://www.gitlink.org.cn/xuos/xiuos/tree/prepare_for_master)
* 需了解XiUOS源码架构，新建目录xiuos/APP_Framework/lib/CoAP，包括相关测试用例和测试结果文档展示
* 项目提供基于ARM架构的矽璓硬件终端，在其上编译、烧写、运行的详细步骤[请参考](https://www.gitlink.org.cn/xuos/xiuos/tree/prepare_for_master/Ubiquitous%2FXiZi_IIoT%2Fboard%2Fedu-arm32)




### 文档

* 矽璓网站介绍：http://xuos.io/
* CoAP介绍网站：https://blog.51cto.com/sddai/3018073



### License

* 本项目遵循MulanPSL-2.0协议，同时兼容Apache-2.0/BSD/MIT协议，**不兼容GPL协议**，其他协议如果与木兰协议不冲突也可兼容。



## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标


* 一、移植CoAP或根据协议自己实现CoAP：
存放目录为xiuos/APP_Framework/lib/CoAP，修改对应的Kconfig、Makefile文件，确保编译成功，提供测试程序，验证CoAP测试通过；

* 二、开源协议检查：
XiUOS遵循MulanPSL-2.0开源协议，所有新增代码遵循MulanPSL-2.0，源码和参考代码需遵循其原有的开源协议，避免协议污染。

## 备注（可选内容）