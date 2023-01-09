# 用太阳能电池平衡一个球

> 原文：<https://hackaday.com/2015/02/19/balancing-a-ball-with-a-solar-cell/>

去上任何一堂控制系统课，你会看到一个期末专题，展示了循环，积分，以及其他所有可以在一两个学期的控制理论中学到的东西。[这个项目不属于这些类中的一类](http://hackaday.io/project/4267-balance-wheel)。然而，它非常酷:它只使用太阳能电池作为传感器，在激光切割木轮的轮缘上平衡一个 40 毫米的钢珠。

大约六年前，在 CCC 看到一个类似的项目后，[Manuel]受到启发，建造了这个球平衡装置。他不记得是谁做的，也避开了最初的 PC/Matlab 架构，但这个版本保留了其灵感的一个有趣特征。控制系统的输入只是一个高强度灯泡和一个太阳能电池。40 毫米的钢球在大部分时间里阻挡了到达太阳能电池的光线。电压的微小变化通过控制系统来保持这个球在轮子上的平衡。

这个构建的唯一硬件是一个电机、一个电机驱动器和一个 ATMega644P。硬件的第一个版本只是几个分线板塞到构建基础的鼠窝布线中，但这已经在版本二[中用新的 PCB](http://hackaday.io/project/4267-balance-wheel/log/14097-pcb-layout-for-rev-2) 修复了。下面视频。

[https://www.youtube.com/embed/zIvI4XlTdEk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zIvI4XlTdEk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)