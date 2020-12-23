# projX-name
### 项目名称
简易调度器

### 项目描述

云原生场景下，虚拟机的规格会变的越来越小，传统的CFS调度器在CPU数量很少的Guest内显的非常臃肿，开销大并且大部分功能也是不需要的。
简易调度器项目的目标，是基于小规格虚拟机场景，从零出发构建一个新的调度器，需要考虑的目标有：
• 兼容所有对通用调度器的需求和接口
• 可以通过系统接口动态接管CFS任务
• 不需要非必要特性的支持，例如quota、share、nice等，数据结构以及队列维护开销最低
• 重新定义调度策略/负载平衡，尽量简单且低开销
       例如：
• 目前的内核调度器还是分散在每个cpu上，由于单个cpu缺乏系统任务运行的整体概念， 对于任务唤醒和平衡上有着天然缺陷，造成load balance做出错误的调度决策，context switch增多等问题。 
• 如果调度器可以了解系统全局负载和计算资源，做集中统一的调度，调度决策会更加准确，也会减少不必要的contentx swith和错误的load_balance。
• 提醒
• 考虑任务负载的特点（batch or interactive), 和虚拟化和容器化场景
• 考虑系统CPU结构、算力、多层cache
• 考虑以上全局数据的一致性和调度时的cpu局部性问题
即通过极简设计提升稳定性和性能表现，在确保多任务正常流转的前提下，把调度延迟或吞吐做到极致（或能用开关在两者之间切换）。

### 所属赛道

2021全国大学生操作系统比赛的“OS功能设计”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2021年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2021全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

......

* github https://github.com/......

* email ......@......



### 难度

中等



### 特征

替代CFS调度器
在少量CPU和任务的场景下性能表现优于CFS
可以动态的使能和关闭



### 文档

........

### License

........



## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

第一题：简易调度器的设计和实现， 一键动态切换调度器
• 设计调度策略，基于CFS调度器，实现相应的回调函数
• 实现一键动态在CFS和简易调度器之间的来回切换
第二题：新负载平衡策略的实现
• 完成load balance基本算法，比较与CFS算法的优缺点
• 实现性能趋向性和功耗趋向性的算法