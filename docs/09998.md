# 从… Excel 发送串行数据？

> 原文：<https://hackaday.com/2015/09/03/sending-serial-data-from-excel/>

当您考虑串行通信时，Microsoft Excel 通常不是第一个出现在脑海中的程序。但是这个电子表格中隐藏着一种相当强大的脚本语言，只需编写一点代码，就可以用来通过你的串口发送和接收数据。该脚本语言被称为[Visual Basic for Applications(VBA)](https://msdn.microsoft.com/en-us/library/office/gg264383.aspx)，自 1993 年以来，它一直是微软 Office 套件的一部分。从那以后，它已经发展成为一种强大的(尽管有时令人沮丧)语言，提供了 Visual Basic 的一部分功能。

它可以是一个有用的工具。例如，假设您正在记录一台具有串行端口(甚至是 USB 上的仿真端口)的仪器的数据。使用一点 VBA，您可以创建一个直接与仪器对话的电子表格，获取数据并根据需要直接处理到电子表格中。这是一个方便的技巧，我自己也用过几次，Maurizio 很好地解释了代码如何工作，以及如何将代码集成到 Excel 中。

如果你正在寻找利用这个 Excel 功能的其他方式，可以考虑[在工作中看电影](http://hackaday.com/2014/10/24/using-excel-to-watch-movies-at-work/)或者在你的工作表中构建[一个虚拟机](http://hackaday.com/2014/12/25/writing-a-virtual-machine-in-excel/)。