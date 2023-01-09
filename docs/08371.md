# ESP8266 ESP07 模块 DoA 修复

> 原文：<https://hackaday.com/2015/02/21/esp8266-esp07-module-doa-fix/>

看起来远东工厂不能足够快地生产出基于 ESP8266 的模块来满足世界上所有黑客的需求。好吧，取放机也是人，所以用不了多久你就会从工厂得到一批混乱的产品。[追踪者约翰尼]发现了一堆 ESP07 模块，它们的[谐振器围绕](http://esp8266-projects.blogspot.in/2015/02/esp-07-module-problem-and-fix.html)安装错误，实际上使它们成为 DoA。谐振器安装也不总是错误的-大多数人报告它们有 90 度偏移，而其他人有 180 度偏移。关了。

不幸的是，您需要一些工具和技能来修复错误。ESP07 模块有一个金属屏蔽，需要拆除才能接触到谐振器。这最好用热风枪来完成。取下盖子后，你需要将谐振器去焊料，并将其放回正确的方向，如[追踪者约翰尼]博客上的图片所示。你可以在这个[论坛的帖子](http://www.esp8266.com/viewtopic.php?f=6&t=811&sid=da7df1aaf04aed5fa36a9dc41b22aa66&start=50)中找到其他人报告同样的故障。在我们之前报道的基于 ESP8266 的 ESP01 模块产生的[魔法烟雾问题之后，质量显然是有代价的。](http://hackaday.com/2015/01/08/faulty-esp8266s-release-smoke-then-keep-working/)