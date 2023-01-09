# ESP8266 的更多 GPIOs

> 原文：<https://hackaday.com/2015/05/31/more-gpios-for-the-esp8266/>

ESP8266 是一款不可思议的硬件；这是一个可以通过串口控制的 WiFi 模块，价格是 5 美元，如果这还不够，还有一个微控制器。在有新的无线电标准之前，这是物联网模块。

ESP 最常见的版本-01 版本只有一排 2×4 引脚，用于串行、电源、配置和两行 GPIO。令人遗憾的是，该模块只有两个 GPIOs，[但如果你有足够好的烙铁，你可以得到几个更多的](https://www.youtube.com/watch?v=9RVyWZCSMtA&feature=youtu.be)。这需要很多仔细的焊接，但[Hugatry]设法在这个小小的模块上突破了两个以上的 GPIOs。

根据[Hugatry]的说法，将这些电线焊接到那些微小的焊盘上需要很大的耐心，但在完成这个小小的概念证明后，他发现一名俄罗斯黑客[成功接入了 ESP8266-01 模块](http://esp8266.ru/esp8266-esp-01-hacked/) ( [Google Translatrix](https://translate.google.com/translate?sl=ru&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fesp8266.ru%2Fesp8266-esp-01-hacked%2F&edit-text=&act=url) )上的四个额外 GPIOs。

作为概念验证，这很好，但是 ESP 模块不止一个。如果你正在寻找一个便宜的 WiFi 模块，看看 ESP-03，-04，或-07；他们有很好的齿形引脚，非常容易焊接。

下面视频。

[https://www.youtube.com/embed/9RVyWZCSMtA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/9RVyWZCSMtA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)