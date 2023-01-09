# 破解激光标签和制造定制枪支

> 原文：<https://hackaday.com/2012/08/08/hacking-laser-tag-and-building-custom-guns/>

![](img/7c9e51a7257904b4e4acfc8bd16d4508.png "tag")

LVL1 hackerspace 的[Brad]看到他的朋友为 2012 年底特律车展制作了一个激光标签/tazer 混搭，他注意到这些新的激光标签枪非常酷。对于一个 30 美元的玩具来说，这些轻型打击枪拥有令人印象深刻的电子设备阵列，但仍有许多需要改进的地方。[Brad]决定对这些枪进行逆向工程，并为游戏的电子设备开发一种替代产品，这样像他朋友这样的人就可以更容易地伤害自己。

[Wowwee Light Strike](http://www.lightstrike.com/)gun 使用红外发光二极管操作，因此解码激光标签协议的显而易见的解决方案是 [Arduino 红外远程库](http://www.arcfn.com/2009/08/multi-protocol-infrared-remote-library.html)。[Brad]在让他的孩子正确读取红外数据时遇到了一点麻烦，但在将所有东西都连接到逻辑分析仪后，他已经弄清楚了数据格式。

现在[布拉德]已经搞清楚了光击数据格式，理论上能够制造自己的枪，与现成的激光标签系统兼容。[Brad]还可以通过使用“健康”功能来扩展这种激光标签系统的功能，以创建一种中型枪，或者为激光标签迷你枪建立一种具有更大弹匣的枪。

如果你想建立自己的激光标签版本，与 Wowwee Light Strike 兼容，你可以在[Brad]的 git 上获取所有代码。