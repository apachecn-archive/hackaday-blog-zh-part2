# 不太像是在建拉斯皮·阿杜伊诺桥

> 原文：<https://hackaday.com/2012/08/05/not-quite-building-a-raspi-arduino-bridge/>

[![](img/634c105e43a5a3059e0f2c2065a7a188.png "ponte")](http://hackaday.com/wp-content/uploads/2012/08/ponte.jpeg)

几个月前，[Omer]送了一个树莓 Pi 到他一直在做的 Arduino bridgePonte。现在他已经组装了一些，他实际上可以[测试他的想法](http://omer.me/2012/07/ponte-revision-0/)将强大的 Raspi 与无处不在的 Arduino 结合起来。

Ponte revision 0 使用了一对 [12 位模数转换器](http://www.ti.com/product/ads1014)，但是在开发的焊接和调试阶段【Omer】发现他的原始设计有一些问题。制造板上的 fet 漏极和源极引脚混在一起，但这个问题很容易通过一点电路板手术解决。

最糟糕的问题是 Ponte rev. 0 的机械设计——Ponte 上的电源插孔直接位于 Raspi 的 USB 端口上方，这意味着不可能将 Ponte 插入 pi。

[Omer]正在解决这些问题，应该会很快完成修订版。一些人问他们在哪里可以买到 Ponte，但是现在还没有组装和运输电路板的计划。这可能会改变，但现在，如果可能值得窃听[欧默]把他的新的和改进的庞特(与 8 端口 I2C 港口扩展器！)上[见工作室](http://www.seeedstudio.com/depot/)