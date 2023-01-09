# 通过蓝牙适配器连接智能手机的红外遥控器

> 原文：<https://hackaday.com/2015/06/19/ir-remote-for-smartphone-via-bluetooth-adapter/>

通常，构建项目的存在理由是为了学习和磨练自己的技能。在这种情况下，如果最终用途看起来有点轻浮也没关系。[indiantinker]制造了 [BlueIR，这是一种使用 BT-Aux 适配器控制蓝牙 A2DP 设备的设备](http://rohitg.in/2015/05/29/TruPlay/)。

听起来很复杂？让我们再试一次。他使用一个旧的红外遥控器向 MSP430 系列微控制器发送数据，该微控制器通过串行连接到 USB 蓝牙接收器适配器，该适配器又连接到一组有线扬声器。蓝牙适配器与他的手机配对。与蓝牙适配器相比，红外遥控器允许他从更远的距离控制手机上的音频播放器命令。

他首先打开 BT 适配器，发现芯片上的标记已经被擦除。相反，他确实找到了两个标有 TX 和 RX 的 pad，但他仍然不知道波特率或命令集。他在互联网上搜索，发现使用的芯片是 OVC3860 蓝牙 2.0 + EDR 立体声音频处理器，并找到了其 at 命令的[列表。在使用串行控制台进行了一些测试后，他发现它可以在 115600 波特下工作。很快，他将它连接到 MSP430 Launchpad，并能够进行通信。接下来，他用墨粉转移法制作了一个小 PCB。该板由 MSP430G2553 微控制器、IR 接收器、LED、一些去耦电容和几个上拉电阻组成。他从主机 BT 适配器上的 3.3V 调节器中提取电能。组装好的 PCB 暂时背在 BT 适配器的顶部，3d 打印的外壳在他的待办事项中。他的代码可以在](http://www.electrodragon.comimg/4/4b/BLK-MD-SPK-B_AT_Commands_OVC3860_List.pdf) [BlueIR Github repo](https://github.com/IndianTinker/BlueIR) 获得，下面的视频展示了它的运行。

[https://www.youtube.com/embed/mrToz8M_BPQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=171&wmode=transparent](https://www.youtube.com/embed/mrToz8M_BPQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=171&wmode=transparent)