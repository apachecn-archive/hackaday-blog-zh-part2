# 用 GPIB 磁盘模拟器保存旧示波器的数据

> 原文：<https://hackaday.com/2015/01/22/save-data-from-old-scopes-with-a-gpib-disk-emulator/>

如果您仍然定期使用旧的测试设备，那么您可能会因为缺少从这些老化设备中提取数据的选项而感到沮丧。许多高端设备都配备了 GPIB 端口，这是一种通用总线，用于与各种过时的外设进行通信。由于 GPIB 磁盘驱动器目前并不太常见(或实用)，因此[Anders]制作了一个模拟磁盘驱动器并将数据存储到 SD 卡的[GPIB 适配器。](http://www.dalton.ax/hpdisk/)

[Anders]设计了一个带有 PIC 微控制器的 PCB，可插入 GPIB 端口。PIC 使用 AMIGO 协议或 SS/80 协议模拟磁盘驱动器，可以在 SD 卡上的配置文件中进行选择。大多数测试设备都支持这两种协议中的一种，所以他的适配器应该可以与几乎所有配备 GPIB 的套件一起工作。

数据保存在 SD 卡上的单个图像文件中，该文件以原生 HP 磁盘格式编码。图像文件可以在 Windows 和 Linux 上用[Anders]在他的项目页面上提到的一些工具打开。如果你有任何带 GPIB 的旧测试设备，并想建造自己的设备，原理图和源代码就在他的网站上，或者[Anders]正在出售裸板。

现在，如果你需要一个协议转换器[，我们已经在几个](http://hackaday.com/2014/05/09/gpib-to-usb-with-a-python-api/)[不同品种](http://hackaday.com/2012/05/01/gpib-connectivity-twofer/)中看到了这些。