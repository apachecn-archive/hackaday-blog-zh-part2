# 没有汉堡的进出板

> 原文：<https://hackaday.com/2014/07/15/in-n-out-boards-sans-hamburgers/>

在这个项目之前，[David]的办公室有一个相当糟糕的系统，告诉每个人谁在办公室，谁出去了，谁今天不来了。Velcro 和白板将完成这项工作，但街机按钮和 led 召唤[大卫]，引导他创建这个[输入/输出状态板](http://hackaday.io/project/1809)。

旧的系统是在每块隔板的边上有一块白板，白板上的标签标明某个人今天是在办公室、外出、生病还是在度假。不方便更换，而且没有一个单一的地方，每个人都可以查看某个特定的人是否在。新系统包括一个四人舱，带有四个街机按钮和 WS2811 LEDs，一个 Arduino Nano 和一个 433 MHz 无线电。主面板只是一个四人舱的更大版本，可以跟踪办公室的每个人。

一个按钮开关将改变一个人从在家到不在家，长时间的按压是“生病”和“休假”所必需的。有趣的是，我们注意到这个版本中没有包括什么:指纹扫描仪是不可能的，因为这将有效地消除任何被标记为“生病”的人。出于同样的原因，RFID 标签阅读器被淘汰了。也不包括显示器。这很好，真的——[ David]不会经常改变标签，无论如何，这只会增加项目的成本和复杂性。