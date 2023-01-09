# 自制活动监视器

> 原文：<https://hackaday.com/2014/09/01/homemade-activity-monitor/>

一群开发者上传了一份 Instructables 教程，展示了开发一款自制 DIY 健身追踪器所需的步骤。该设计是他们基于 Arduino 的[可穿戴智能手表项目](http://www.instructables.com/id/Make-your-own-smart-watch/?ALLSTEPS)的第二次迭代。这一次，他们选择更多地关注监控系统，而不是视觉显示。它被称为“RetroBand ”,记录用户采取的步骤和消耗的卡路里。

使用的微控制器是 Arduino Pro mini 3.3v。集成了加速度计和陀螺仪传感器，以捕捉“RetroBand”的运动。一个无线蓝牙模块连接到一个 Android 手机，该手机通过一个包含图表的 [Play Store 应用程序](https://play.google.com/store/apps/details?id=com.hardcopy.retroband)显示数据。一个外壳是 3D 打印的。一切都由一节锂聚合物电池供电。该项目的代码可以在 [Github](https://github.com/godstale/retroband) 上找到，带有操作手册的附加信息可以在[他们的网站](http://www.hardcopyworld.com/ngine/aduino/index.php/archives/871)上找到(该网站是韩语的，但可以很容易地通过浏览器翻译)。