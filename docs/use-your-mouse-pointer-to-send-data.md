# 使用鼠标指针发送数据

> 原文：<https://hackaday.com/2015/08/30/use-your-mouse-pointer-to-send-data/>

[Ido Gendel]正在思考在设备之间发送数据的新的有趣方法，这时他意识到答案就在他手中。字面意思:他决定尝试用鼠标指针发送数据。他想出了一个有趣的方法，利用鼠标指针的微小移动以高达 1200bps，或每秒 150 字节的速度发送数据。

他做这件事的方式非常非常聪明。他使用了一个 Arduino Leonardo 来模拟鼠标，与他现有的鼠标一起工作。这种设置意味着他可以使用他现有的鼠标:系统只是将 Arduino 视为第二个鼠标，当你放大时，指针看起来有点不稳定。这是因为 Arduino 只是发送微小的动作，每个动作都是一个代码，代表一个任意字节(4 个二进制位)的数据。通过使用三种左右或上下运动的组合，他能够创造 16 种运动，每种运动可以编码 4 位数据。这些编码动作中的每一个也将鼠标返回到它的原点，这样鼠标就不会在发送数据时神秘地滚出屏幕。

[![The encoding scheme used by [Ido].](img/033fe34d74eeb81d225699d94d84c920.png)](https://hackaday.com/wp-content/uploads/2015/08/encoding2.jpg)

【I do】所使用的编码方案。

在电脑上，一个定制的程序检测并解码这个动作，重新创建数据流。在他的例子中，这是来自光敏电阻的数据，但也可能是从随机数据到秘密文件内容的任何东西。

当然，这不是发送秘密数据的实用方法:它只在自定义程序处于活动状态时有效，每秒 150 字节相当慢，在 Windows 中启用鼠标加速会停止它的工作，因为它掩盖了微小的移动。但这是一个很棒的黑客技术，它展示了如何以你可能不会首先想到的方式发送数据。当你试图使设备尽可能简单时，这是一个重要的教训。

[https://www.youtube.com/embed/FCapWbz_va0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FCapWbz_va0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)