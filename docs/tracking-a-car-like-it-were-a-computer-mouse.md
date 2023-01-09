# 像追踪电脑鼠标一样追踪一辆车

> 原文：<https://hackaday.com/2013/03/10/tracking-a-car-like-it-were-a-computer-mouse/>

![optical-mouse-sensor-tracks-vehicle-motion](img/bbac15cfe52fd4d2a9f9d978a3436437.png)

这是【保罗·曼德尔的】[地面真实速度传感器](http://www.mand3l.com/work/velocimeter/)。这是一种设备的别出心裁的名字，这种设备通过实际监控车辆行驶的地面来跟踪车辆的运动。这不同于简单地测量车轮旋转(这是传统里程表的工作方式)，因为这些系统是对运动的间接测量。对我们来说，有趣的部分是在左边使用了 ADNS-3080 单芯片光学鼠标传感器。它便宜、精确，只需要在绑在汽车底部之前进行加固。

[Paul]设计了一个保护电子设备的外壳，并允许传感器安装在车辆不平坦的下腹部。光学芯片需要与镜头配对，他选择了一个价格约为传感器十倍的镜头。使用 PIC 18F2221 将数据从传感器传送到主系统控制器。我们从这个项目中学到的一个小窍门是轮询一个总是返回默认值的寄存器作为健全性检查。如果你得不到预期的值，这表明存在通信问题，这是对进入振动地狱的硬件的一个重要测试，这就是汽车技术。