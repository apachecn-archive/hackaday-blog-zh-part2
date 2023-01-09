# 基于 Arduino 的 Enigma 副本功能齐全

> 原文：<https://hackaday.com/2013/10/07/arduino-based-enigma-replica-is-fully-functional/>

[ST-Geotronics]的人制作的这个[开源的 Enigma 复制品](http://www.instructables.com/id/Make-your-own-Enigma-Replica/)简直令人震惊。他们从几年前我们看到的一个[滑稽建筑](http://hackaday.com/2011/02/15/wwiis-top-cryptography-comes-to-a-childs-toy/)中汲取灵感，将一个儿童玩具破解成一个谜机。相反，他们的项目是模仿最初的[英格玛·M4 密码机](http://www.cryptomuseum.com/crypto/enigma/m4/index.htm)，除了一点艺术许可，我们认为他们抓住了视觉风格。至于功能，指南声称一切正常，包括插板。

[ST-Geotronics]团队没有试图立即将所有东西都塞进最后一个外壳，而是煞费苦心地设计了一个原型，以确保四个 16 段 LED 显示屏接线正确，功能正常。下一步是在一个 6”x8”的性能板上布置一组按钮和电阻。他们使用 [charlieplexing](http://hackaday.com/2013/04/08/another-way-to-look-at-charlieplexing/) 来处理 16 段显示器(实际上每段有 17 个 led ),并通过将它们垂直安装并封装在透明圆顶中，将每个显示器伪装成数码管。该案件遵循 M4 的原始尺寸，包括一个胶合板箱与废钢铁的顶板。

请浏览他们的指导页面，了解更多详情。在那里，你可以找到几个 Arduino 草图来测试五种不同 M4 操作模式的功能和代码。