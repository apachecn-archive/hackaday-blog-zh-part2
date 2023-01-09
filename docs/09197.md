# 在 3D 打印中嵌入 PCB

> 原文：<https://hackaday.com/2015/06/04/embedding-pcbs-in-3d-prints/>

午餐盒电子公司的人正在研究一个非常酷的原型:在标准的 1×1 乐高积木里嵌入发光二极管。作为一个原型，他们需要一种廉价的方法来生产填充电子产品的乐高积木。事实证明，一台普通的 3D 打印机有足够的分辨率，但是如何把电子设备放进砖块里呢？[当然是 Gcode 巫师](http://www.lunchboxelectronics.com/how-to-embed-electronics-into-a-3d-print)。

被塞进砖块里的电子设备并不多——只是一个带 LED 的小印刷电路板。然而，它确实需要进入砖块内部。这需要在正确的层停止 3D 打印机，将打印头移开，插入 PCB，然后将打印头移回停止的位置。

救援代码。通过在打印的 Gcode 中插入几行，打印可以暂停，打印头上升和返回，打印继续进行。

如果你想看看这些发光的乐高是什么样子，[现在有一个 Kickstarter 正在进行](https://www.kickstarter.com/projects/1828089281/build-upons-worlds-tiniest-light-up-bricks)。这正是 80 年代太空布景所需要的，只是晚了三十年。