# 焦耳小偷为时钟偷电

> 原文：<https://hackaday.com/2014/10/03/joule-thief-steals-power-for-a-clock/>

电子修补程序中的一个常见项目是[焦耳窃贼](http://en.wikipedia.org/wiki/Joule_thief)，这是一种自振荡电路，可以在电压下降到大多数设备停止工作后“窃取”电池中的剩余能量。通常情况下，该电路为 LED 供电，直到几乎所有的能量都从电池中提取出来，但[Lionel Sears]已经创造了一种[专用焦耳 theif，使用“额外”的能量为时钟](http://rimstar.org/science_electronics_projects/joule_thief_powering_clock_ls.htm)供电。

该电路使用四个线圈而不是通常的两个线圈来从电池中提取能量。该电路为一个大电容器充电，该电容器提供驱动时钟机构所需的更高电流脉冲。它可以用一节 AA 电池为时钟供电，并将一直运行到电池上的电压仅为 0.5 伏。

正常情况下，时钟会在电压下降到这么低之前停止运行，尽管事实上电池中仍有少量化学能。该电路可以使用新电池驱动时钟更长时间，或者可以使用旧的“死”电池来运行时钟一小段时间，同时从它们中提取最后一点能量。如果你愿意的话，你甚至可以用[热水和冷水以及一个焦耳窃贼](http://hackaday.com/2013/11/12/peltier-joule-thief-power-supply/)来运行你的时钟！感谢[史蒂文]的提示。