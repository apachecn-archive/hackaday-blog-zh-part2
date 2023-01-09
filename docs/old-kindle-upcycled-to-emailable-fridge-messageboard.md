# 旧 Kindle 升级为电子邮件冰箱留言板

> 原文：<https://hackaday.com/2015/07/29/old-kindle-upcycled-to-emailable-fridge-messageboard/>

我们都有一堆旧设备躺在某个地方，等着被拆成零件，或者变成有用的东西。[Peter Voljek]决定用一个旧的 Kindle 电子书阅读器做后一件事，[把它变成一个整洁的留言板，可以贴在冰箱上](https://petervojtek.github.io/diy/2015/07/28/share-messages-with-kindle-on-fridge.html)。通过添加一些服务器端 Ruby 代码，您可以通过电子邮件向此发送消息，它会自动显示收到的最后一条消息。贴上一些磁性胶带，你就有了一个整洁的冰箱门布告栏。

[Peter]在 Raspberry Pi 上运行他的 Ruby web 服务器，但它应该在任何支持 Ruby 的平台上运行，所以你可以在 NAS 设备上运行它，或者在任何内置 web 服务器的设备上运行它。黑客的 Kindle 端利用一些秘密命令来禁用屏保，然后使用 AJAX 和 JavaScript 来自动刷新 RPi 提供的网页。

嘿，为什么不把这个和 Kindle weather station hack 结合起来，创建一个布告栏，告诉你需要从商店买什么，同时提醒你为什么不应该离开家？