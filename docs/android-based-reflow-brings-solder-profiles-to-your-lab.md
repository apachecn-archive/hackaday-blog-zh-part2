# 基于 Android 的回流焊将焊料特性带入您的实验室

> 原文：<https://hackaday.com/2015/07/15/android-based-reflow-brings-solder-profiles-to-your-lab/>

[安迪·布朗]是一个多产的黑客，并最终建立了许多硬件。大约一年前，他做了一个回流炉控制器。他设计的电路板使用了大量的表面贴装器件。这看起来像是先有鸡还是先有蛋的问题。因此，他设计了一个新的，易于构建的，基于 Android 的回流控制器。新版本仅使用一个易于焊接的表面贴装器件。通过在控制器上安装一个廉价的蓝牙模块，他能够编写一个应用程序，使用任何支持蓝牙的 Android 手机或平板电脑来控制烤箱。

单个 PCB 分为高压、市电供电部分，与低功率控制电子设备分开，并带有断流槽以解决爬电问题。一个 [BTA312-600B](http://www.nxp.com/documents/data_sheet/BTA312-600B.pdf) 三端双向可控硅开关用于打开和关闭烤箱(负载)。三端双向可控硅开关由 [MOC3020M](https://www.fairchildsemi.com/datasheets/MO/MOC3023M.pdf) 光隔离三端双向可控硅开关驱动器控制，该驱动器又由微控制器通过晶体管驱动。结实的 12Amp T0220 封装 triac 在切换 1300W 负载时预计会变热，[Andy]通过数学计算展示了他是如何选择散热器的。为了确保安全，他使用一个隔离的、完全封闭的降压变压器为低压控制部分供电。他的要求之一是检测电源波形的过零点。利用该信号，他可以将三端双向可控硅开关元件打开特定的角度，该角度可以由微控制器根据负载所需的电流大小来改变。经过整流但未经滤波的交流信号馈入晶体管的基极，每当达到基极-发射极电压阈值时，晶体管就会切换。

为了进行温度测量，[Andy]使用了 k 型热电偶和 Maxim MAX31855 热电偶数字转换器。由于生产批次不良，这部分给他带来了相当大的痛苦，他通过 [eevblog 论坛](http://www.eevblog.com/forum/projects/max31855-temperature-error/)发现了这一点——最终通过订购替代品解决了这一问题。蓝牙功能由流行且廉价的 HC-06 模块处理，该模块允许简单的自动配对。他在 ATmega328P 上制作了代码原型，然后在使用 gcc 优化器优化并将其缩减到 7.5kb 以下后，将其转移到 ATmega8 上。为了使电路板独立，他还添加了一个廉价的诺基亚 5110 显示器和一个带开关的旋转编码器选择器。这允许本地控制，而不需要 Android 设备。

开发板的 Gerbers(zip 文件)可从他的博客中获得，ATmega 代码和 Android 应用程序可从他的 [Github repo](https://github.com/andysworkshop/awreflow2) 中获得。他博客上的 BoM 表让订购所有零件变得很容易。在休息后长达一小时的视频中，[Andy]将带您了解焊嘴的选择、焊接 SMD 器件的技巧、电路板的整个组装过程以及演示。然后，他将电路板连接到他的烤箱，并展示它的运行。他仍然需要完善他的 PID 调节和算法，所以请在下面的评论中加入你的建议。

[https://www.youtube.com/embed/1ExZUTiHOVY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1ExZUTiHOVY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)