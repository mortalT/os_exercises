# 操作系统概述思考题

## 个人思考题

---

分析你所认识的操作系统（Windows、Linux、FreeBSD、Android、iOS）所具有的独特和共性的功能？
- [x]  

>  共性：支持多种文件系统、支持多种网络协议、支持多种物理设备接口、支持多用户和组策略。
   Windows特性：GUI高度集成，使用文件名扩展
   Linux特性：更加偏重于网络OS，代码执行效率高，且系统更为稳定

请总结你认为操作系统应该具有的特征有什么？并对其特征进行简要阐述。
- [x]  

>   1.Concurrence : Multiple tasks are performed in same intervals.
    2.Sharing : System resources can be shared by several processes(or threads).
    3.Virtual : Reflect a physical item to a logical(virtual) item such as VM/Virtual Memory/Virtual Channels.
    4.Asynchronism : Processes run and halt(wait for resources) while multitasking.

请给出你觉得的更准确的操作系统的定义？
- [x]  

>   OS是管理电脑硬件设备与软件资源的程序。

你希望从操作系统课学到什么知识？
- [x]  

>   OS的结构与原理 & OS是如何运作的。

---

## 小组讨论题

---

目前的台式PC机标准配置和价格？
- [x]  

>      CPU: Intel Core i5 4690.
       Motherboard: MSI Z97.
       Graphics: Nvidia 970GTX.
       RAM : 16G DDR3 1600MHz.
       
       PRICE: Around 8000 CNY.
       
你理解的命令行接口和GUI接口具有哪些共性和不同的特征？
- [x]  

>     共性：人机交互
      CLI：高效性
      GUI：易用性

为什么现在的操作系统基本上用C语言来实现？
- [x]  

>  C语言可以直接操作底层硬件同时也可以作为高级语言提供用户接口。


为什么没有人用python，java来实现操作系统？
- [x]  

> 无法直接操作底层硬件。 

请评价用C++来实现操作系统的利弊？
- [x]  

>  OS的内核部分并不需要C++的特性，反而C++会使得内核实现更麻烦..
   好处是外层部分(驱动,etc.)运用C++的OO、泛型等技术能简化程序。

---

## 开放思考题

---

请评价微内核、单体内核、外核（exo-kernel）架构的操作系统的利弊？
- [x]  

>  微内核：模块化的方式设计操作系统，模块的设计者只需要关注自己的功能模块
           操作系统的更新时，除了微内核本身，可以动态的更新其他的功能模块
           在系统运行的时候，可以根据需要动态的使能 / 禁止对应的模块，以释放计算机的资源
           在性能上有不可避免的弱点，因为一个进程需要使用某个功能模块的时候，需要通过消息机制来传输。这里涉及到消息传递进程切            换的时间，这比函数调用的消耗大的多
     外核：减少软件的抽象化，简化传统内核的消息机制。
     
请评价用LISP,OCcaml, GO, D，RUST等实现操作系统的利弊？
- [x]  

>   利：这些语言在某些具体实现上比较优越..
    弊：都需要编译器将其编译成为机器可识别的语言..

进程切换的可能实现思路？
- [x]  

>  Step1.决定是否作上下文切换以及是否允许作上下文切换
   Step2.保存当前执行进程的上下文
   Step3.使用进程调度算法，选择一处于就绪状态的进程
   Step4.恢复或装配所选进程的上下文，将CPU控制权交到所选进程手中
   
计算机与终端间通过串口通信的可能实现思路？
- [x]  

>  9pin串口数据线，23交叉互联。

为什么微软的Windows没有在手机终端领域取得领先地位？
- [x]  

>  进入市场较晚，移动市场已被iOS和Android占领，导致iOS和Android平台的app数量远超WP，手机厂商也不是很关注WP。
   

你认为未来（10年内）的操作系统应该具有什么样的特征和功能？
- [x]  

>  1.Better Mobility
   2.Rely on networks(Internet) more.

---
