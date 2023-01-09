# 用无线鼠标加密狗控制四轴飞行器

> 原文：<https://hackaday.com/2015/07/15/controlling-quadcopters-with-wireless-mouse-dongles/>

上周，我们赠送了一些 Crazyflie 2.0 四轴飞行器给一些很酷的 Hackaday 奖参赛作品。这款四轴飞行器旨在通过智能手机进行控制。但它也可以由带有 USB 加密狗和 nRF24LU1+ SOC 的 PC 控制。[ajlitt]没有想到他想要一个 USB 加密狗(Crazyradio)来控制这个 quad，直到他使用他的礼物代码来认领他的 Crazyflie quad。不管；罗技无线键盘和鼠标的加密狗使用与 Crazyflie [相同的无线电，可以改装成这种四轴飞行器](https://hackaday.io/project/6741-crazyradio-for-cheapskates)。

罗技统一接收器内的电路板很简单，有一些 USB 连接器的焊盘，一个晶体，nRF24LU1+无线电模块和一些无源器件。为了让这个无线电芯片与他的计算机一起工作，[ajlitt]只需要打开 SPI 引脚，将所有东西连接到一个总线盗版者。

事实证明，将 Crazyradio 固件安装到这上面比将一些磁线焊接到几个引脚上要困难一些。该芯片首先在没有引导加载程序的情况下进行闪存，在将一个字节放入适当位置后，发现了带有引导加载程序的完整映像，[ajlitt]拥有了一个由无线鼠标加密狗制成的工作正常的 Crazyflie 无线电。范围不是很大——只有 30 英尺左右，或者是你期望无线鼠标工作的最远距离。出色的工作，即使[ajlitt]暂时没有鼠标。

Crazyflie 2.0 可以从 Hackaday 商店买到，如果你不想黑自己的，还可以带附件。