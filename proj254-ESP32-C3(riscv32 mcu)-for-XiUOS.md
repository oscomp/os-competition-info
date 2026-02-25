# proj254-ESP32-C3(riscv32 mcu)-for-XiUOS
### 项目名称
将XiUOS中的XiZi内核移植到[ESP32-C3开发板](https://docs.espressif.com/projects/esp-idf/zh_CN/latest/esp32c3/hw-reference/esp32c3/user-guide-devkitm-1.html)

### 支持单位  
浙江省北大信息技术高等研究院

### 项目描述
ESP32-C3-DevKitM-1 是一款入门级开发板，使用以尺寸小而得名的 ESP32-C3-MINI-1 模组。该款开发板具备完整的 Wi-Fi 和低功耗蓝牙功能。本项目目标是将XiUOS中的XiZi内核移植到所述开发板


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
* 需了解XiUOS源码架构，新建目录xiuos/Ubiquitous/XiZi_IIoT/board/esp-32-devkitm-1，包括相关测试用例和测试结果文档展示
* 在XiUOS上提供新的开发板支持请[参考](https://www.gitlink.org.cn/xuos/xiuos/tree/prepare_for_master/Ubiquitous%2FXiZi_IIoT%2Fboard%2Fedu-arm32)
* 该开发板详细[使用方法](https://docs.espressif.com/projects/esp-idf/zh_CN/latest/esp32c3/hw-reference/esp32c3/user-guide-devkitm-1.html)



### 文档

* 矽璓网站介绍：http://xuos.io/



### License

* 本项目遵循MulanPSL-2.0协议，同时兼容Apache-2.0/BSD/MIT协议，**不兼容GPL协议**，其他协议如果与木兰协议不冲突也可兼容。



## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

* 一、：将XiUOS中的xizi内核运行在ESP32-C3开发板,支持串口打印,支持ShowTask和ShowMemory两个shell命令。
* 二、开源协议检查：
XiUOS遵循MulanPSL-2.0开源协议，所有新增代码遵循MulanPSL-2.0，源码和参考代码需遵循其原有的开源协议，避免协议污染。

## 备注（可选内容）