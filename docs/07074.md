# THP 半决赛:NoteOn 智能笔

> 原文：<https://hackaday.com/2014/09/22/thp-semifinalist-noteon-smartpen/>

有大量的应用程序可以用来做笔记和记录想法，但有时简陋的笔是最好的。然而，如果你有丢失、弄皱或把含咖啡因的饮料洒在笔和纸笔记上的倾向，拥有一份电子副本是非常好的。

[ [尼克](http://hackaday.io/hacker/11592)的 [NoteOn 智能笔](http://hackaday.io/project/2678-NoteOn-Smartpen)旨在动态数字化你的书写，同时像普通笔一样工作。这是通过使用 [ST LSM9DS0TR](http://www.st.com/web/catalog/sense_power/FM89/SC1448/PF258556) 实现的:一个 9 轴惯性测量单元(IMU)。这些惯性测量值由一个 [STM32 Cortex M4F](http://www.st.com/web/en/catalog/mmc/FM141/SC1169/SS1576/LN1824?icmp=ln1824_pron_pr_apr2014&sc=stm32f302-pr) 处理器处理，并存储在内部闪存中。

为了检索您的笔记， [Nordic nRF8001](https://www.nordicsemi.com/eng/Products/Bluetooth-Smart-Bluetooth-low-energy/nRF8001) 蓝牙低能耗无线电将 MCU 与电话或计算机配对。USB 口只用来给设备充电，用户界面是单个按键和 LED。

这种设备的主要硬件挑战是将其封装在像一支笔一样小的东西中。令人印象深刻的是，该板是来自 OSHPark 的廉价 2 层 PCB。组装好的设备直径为 10 毫米，与“哑”笔的直径相似。

笔记不需要特殊的纸张，仅依靠惯性测量来重建书写。随着硬件的工作，[Nick]现在正在处理使设备可用的固件。

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png) **本帖介绍的项目是[黑客日奖的四分之一决赛。](http://hackaday.io/list/2864-The-Hackaday-Prize%3A-Semifinalists)**