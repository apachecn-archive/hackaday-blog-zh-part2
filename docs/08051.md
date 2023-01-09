# 自动台锯切割光伏太阳能电池

> 原文：<https://hackaday.com/2015/01/12/automated-table-saw-cuts-photovoltaic-solar-cells/>

[sudarshan]是一名太阳能爱好者，他需要一种方法来为他的项目切割太阳能电池。他以前创造了一个旋转工具锯，但手动通过他们是粗略的。只要他的手有一点错误的移动或者在工作面上弯曲都会导致电池破裂。这些细胞非常脆弱，很容易破碎。他需要一种切割这些细胞的方法，这种方法不会产生抖动，并且可以直线切割。他环顾他的垃圾箱，发现了一个奇怪的解决方案…一个扫描仪。是的，你可以用它来扫描你电脑里的照片。该扫描仪有两个至关重要的特征，一个平坦的表面和一个与平坦表面完全平行移动的托架机构。

[sudarshan]用扫描仪制作了一个太阳能电池切割迷你台锯,并使切割自动进行。他把一个装有金刚石锯盘的马达安装到马车上，负责切割。刀片的位置刚好够高，可以穿透取代原来玻璃床的有机玻璃。电源开关打开切割盘电机，Arduino 用于来回移动托架，包括切割刀片。两个库存扫描仪按钮被重复使用并连接到 Arduino，以保持锯的外观良好。

锯的最初几遍是为了在有机玻璃上切一个槽。为了切割太阳能电池，将电池绑在床上，所需的切割位置与有机玻璃床上的槽对齐。一旦一切都设置好了，点击“开始”按钮，锯片被慢慢地推过电池，留下一个直的，干净的切口。

[https://www.youtube.com/embed/PmdaVf0kplE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/PmdaVf0kplE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

如果你的手足够稳定，可以切割太阳能电池而不会将其打碎，你可能会对这个由 Dremel 供电的太阳能电池锯感兴趣。