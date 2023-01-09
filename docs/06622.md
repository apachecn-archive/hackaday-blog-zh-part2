# USB 旋转电话:回到过去的 Lync

> 原文：<https://hackaday.com/2014/07/22/usb-rotary-phone-a-lync-to-the-past/>

[Ivan]受够了这种猖獗的虚拟化。当他的公司拿走了他的实体台式电话，转而使用 Lync 女士时，他被迫制作了一部 USB 旋转式电话。他的同事们很喜欢它，其中一个人要求[伊万]再建一个。构建日志专注于转换他的同事的老式黄铜和铜的数量，必须重达一吨。

他不得不在这一个上多下点功夫，因为它里面已经生锈了，有几个触点弯曲了。好消息是，扬声器和麦克风工作正常，他可以使用它们。在恢复了股票功能后，他添加了一个 USB 声卡，并使用一个 [PIC32MX440F256H](http://www.microchip.com/wwwproducts/Devices.aspx?product=PIC32MX440F256H) 创建了一个 USB 键盘。

旋转式电话的拨号使用两个开关，一个是打开的，一个是在无人拨号时关闭的。一旦检测到拨号，打开的开关闭合，闭合的开关根据拨号数字发出滴答声(十次滴答声表示 0)。[Ivan]还读取开关挂钩状态，并增加了去抖功能。这给他带来了一些麻烦，因为 PC 总线预期的快速响应，但他利用了中断并被允许保留他的座位。

请不要挂断。[Ivan]的视频将很快提供给您。

[https://www.youtube.com/embed/OcKlAbpA09g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/OcKlAbpA09g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/EtUKXqRbHPQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EtUKXqRbHPQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)