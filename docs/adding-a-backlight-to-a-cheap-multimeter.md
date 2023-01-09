# 给便宜的万用表加背光

> 原文：<https://hackaday.com/2015/06/11/adding-a-backlight-to-a-cheap-multimeter/>

我们并不都需要超高质量的电子测试设备。有时，二手或便宜的设备足以完成工作。虽然错过了一些“奢侈”的功能会有点烦人。[Ekriirke]他的廉价万用表有这个问题。他希望 LCD 屏幕有背光，以便更容易看到，所以他没有升级到更昂贵的设备，而是自己加了一个。

打开万用表后[Ekriirke]发现它靠一节 12V 的电池运行。他意识到最简单的方法就是将四个白光 led 串联起来。四个发光二极管排列在液晶显示器两侧的外壳内，每个角一个。引线弯曲成 90 度角，以“死虫”方式焊接在一起。薄铜箔带贴在 PCB 上，这样当外壳合上时，led 的阳极和阴极就会接触。

胶带缠绕在 PCB 的另一侧，那里有更多的空间放置下一片电路。电容器、电阻器和晶体管与瞬时开关一起使用。这个电路允许[Ekriirke]按下按钮一次打开灯大约十秒钟。该电路还通过仪表的拨号开关运行，防止 led 在仪表关闭时打开。

[via [Reddit](https://www.reddit.com/r/electronics/comments/399suv/i_hacked_my_dollar_meter_to_have_backlighting/)