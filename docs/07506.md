# 用树莓皮猎狐

> 原文：<https://hackaday.com/2014/11/06/fox-hunting-with-a-raspberry-pi/>

不，不是真的狐狸！[KM4EFP]是一名业余无线电爱好者，热衷于猎狐活动，在这项活动中，几名无线电操作员试图使用无线电测向技术找到一个广播信标(一只“狐狸”)。[KM4EFP]刚刚用树莓皮在一个建造得非常好的外壳里建造了他自己的[便携式狐狸。](http://hackaday.io/project/3325-pifox)

由于狐狸可能会在外面呆上一段时间，这个项目被安置在一个防风雨的弹药箱里。侧面安装了一个天线支架，它与 Raspberry Pi 上的 GPIO 引脚相连。整个设备由 6000 毫安的电池组供电，这使得狐狸能够广播足够长的时间以被发现。

运行在 Raspberry Pi 上的软件与 [Pi FM 发射机程序](http://hackaday.com/2014/06/15/easily-turn-your-raspberry-pi-into-an-fm-transmitter/)非常相似，但它是专门为业余无线电广播制作的。获得 Pi 广播电台几乎不需要额外的硬件，因为这些软件包可以直接从 GPIO 引脚驱动天线。这是一个标准调频发射机的伟大转折，各地的业余无线电爱好者可以用它来开始寻找那些狡猾的狐狸！