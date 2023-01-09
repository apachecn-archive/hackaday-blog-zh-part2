# Extreme Vectrex Multicart 播放坏苹果

> 原文：<https://hackaday.com/2015/04/24/extreme-vectrex-multicart-plays-bad-apple/>

[Sprite_TM]有一台他想玩的 Vectrex 游戏机。唉，他的临时多卡已经年久失修了。卷起他的袖子，他开始做一个新的，更好的。他的 PCB 设计包括他选择的微控制器:ST STM32F411，32 位 100Mhz ARM Cortex M4，以及 16MB SPI 闪存芯片。[Sprite_TM]想让在多卡上编程游戏变得简单。将 STM 的 libopencm3 固件库与 Elm-Chans FatFS 结合使用，multicart 可以插入计算机的 USB 端口，并像 u 盘一样将任何游戏数据拖放到其上。然后，PCB 直接连接到 Vectrex 的盒式端口。第一个卡片盒文件是一个基本菜单，它列出了存储在闪存中的所有游戏 rom。当用户选择游戏时，STM 加载 ROM 文件，然后菜单软件启动。

在将他的整个 Vectrex ROM 库加载到 multicart 上之后，[Sprite_TM]意识到他还有太多的剩余空间，所以他决定添加一些额外的东西。他的第一选择是[坏苹果](https://www.youtube.com/watch?v=VzEUeWnV73U) (YouTube 链接)，这是一个由[头后计划](http://en.wikipedia.org/wiki/Touhou_Project)游戏系列粉丝制作的音乐视频。该视频以阴影艺术风格展示了许多游戏角色的黑白轮廓。自首次亮相以来，坏苹果已经被移植到从[世嘉创世纪](https://www.youtube.com/watch?v=2vPe452cegU) (YouTube 链接)到[激光扫描仪](https://www.youtube.com/watch?v=5A9Eh6D-K_g) (YouTube 链接)的所有东西。是时候让[威格斯](http://hackaday.com/2013/09/05/making-asteroids-miniature/)加入这个名单了。

从 YouTube 上抓取视频后，[Sprite_TM]使用 MPlayer 将每一帧保存为 PNG 格式，同时保存音乐的波形文件。接下来，他对 PNG 文件运行 [Potrace](http://potrace.sourceforge.net/) 来获得矢量版本。使用定制的 PHP 脚本，生成的 JSON 文件被后处理成 Vectrex 使用的相对向量。通过让 Vectrex 的 8 位 DA 转换器执行视频电路和音频的双重任务，数字音频成为可能。然而，为了听音乐，音量必须调到最大。顺便说一句，在这种情况下，DAC 只能在未绘制矢量时输出音频，因此需要调整事件时序。在将坏苹果传送到多卡之前，视频和音频数据在修改版本的 [VecX](http://www.bannister.org/software/vecx.htm) 用于同步定时事件后被重新解析。

休息之后，你可以看到坏苹果的 Vectrex 版本，以及基于厄运等级的 3D 引擎。该引擎是用 C 语言编写的，利用了 Z 缓冲区，创建了立体 3D 对象的效果。这里没有武器或敌人可以派遣，但效果仍然令人印象深刻。

[https://www.youtube.com/embed/_aFXvoTnsBU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/_aFXvoTnsBU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

感谢伟大的提示，[莫里斯]！