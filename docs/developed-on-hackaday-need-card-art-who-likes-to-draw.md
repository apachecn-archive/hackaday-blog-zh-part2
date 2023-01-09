# 在 Hackaday 上开发:需要卡片艺术——谁喜欢画画？

> 原文：<https://hackaday.com/2014/03/27/developed-on-hackaday-need-card-art-who-likes-to-draw/>

[![](img/7219dcd7a64c32c329571c18c2ea0299.png)](http://hackaday.com/wp-content/uploads/2014/03/p10505931.jpg)

我们的离线密码管理员项目(又名 [Mooltipass](https://github.com/limpkin/mooltipass) )非常幸运地拥有非常活跃(并且非常有能力)的贡献者。[Harlequin-tech]最近完成了我们的有机发光二极管屏幕低级[图形库](https://github.com/limpkin/mooltipass/tree/master/source_code/src/OLEDMP)，它(以及其他)支持[RLE](http://en.wikipedia.org/wiki/Run-length_encoding)解压缩，可变宽度字体和字体多位深度 T10 位图。为了让事情变得简单，他还发布了一个[漂亮的 python 脚本](https://github.com/limpkin/mooltipass/tree/master/bitmaps)来从位图图片自动生成 c 头文件[和另一个](https://github.com/limpkin/mooltipass/tree/master/fonts)来导出字体。

[Miguel]完成了 AES 加密/解密方案(在 CTR 模式下使用[AES](http://en.wikipedia.org/wiki/Block_cipher_mode_of_operation#Counter_.28CTR.29))并写了一篇[精彩自述](https://github.com/limpkin/mooltipass/tree/master/source_code/src/AES)，其中解释了一切是如何工作的，以及有人如何使用几个标准化测试来检查他的代码。我们强烈建议读者确保我们没有犯任何错误，因为是你们中的一个人建议我们迁移到 CTR 模式(谢谢[mate]！).

在硬件方面，我们开始生产 Olivier 设计的顶部和底部 PCB。我们目前也在寻找拥有多个 Arduino 盾牌的人，以确保他们可以连接到 Mooltipass。几天前，我们成功地将 Arduino bootloader 放入了我们的微控制器中，并使官方的 Arduino Ethernet shield 与它一起工作。

最后，正如你可能已经从上面的图片中猜到的，我们亲爱的智能卡经销商几乎可以在上面打印任何东西(这些是样本)。如果你们中的一个人想画点什么，请通过 mathieu[at]hackaday.com 联系我！

更幼稚的说法是，不要犹豫给 HaD 项目的[mu ltipass 一个头骨，这样它就可以重新获得“](http://hackaday.io/project/86-Mooltipass)[最狡猾的](http://hackaday.io/projects)”的合法地位。