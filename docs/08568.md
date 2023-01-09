# 向 3D 打印添加回收代码

> 原文：<https://hackaday.com/2015/03/18/adding-recycling-codes-to-3d-prints/>

你接触的每个小塑料玩具都有某种回收代码。既然我们在家里生产塑料 3D 打印零件，就如何回收所有这些零件达成一致将是一个好主意，密歇根理工大学的[【约书亚·皮尔斯】实验室有了答案](http://www.mtu.edu/news/stories/2015/march/call-change-recycling-standards-3-d-printing-expands.html)；因为我们正在打印这些对象，我们可以直接在对象中打印回收代码。

美国的塑料回收码系统特别不适合识别有问题的物体是由哪种塑料制成的；只有 7 个编码，而中国的塑料识别系统使用 140 个识别码。这种用于标记 3D 打印零件的系统大量借鉴了中国的系统，将 ABS 指定为“9”，PLA 指定为“92”，HIPS 指定为“108”。

就回收代码达成一致后，剩下唯一要做的就是在每张照片上贴上正确的回收代码。这是一个简单的任务，只需要几个 OpenSCAD 脚本–[论文](https://www.academia.edu/11229348/Polymer_recycling_codes_for_distributed_manufacturing_with_3-D_printers)展示了一个由贴有正确代码的 HIPS 制成的扳手，以及一个标有数字 9 的 ABS 钻头手柄。3D 打印开辟了一些有趣的制造技术，研究小组用一个 PLA 花瓶展示了这一点，该花瓶的前几层嵌入了回收代码 lithophane。