# 墨西哥卷饼炸弹客

> 原文：<https://hackaday.com/2012/12/09/the-burrito-bomber/>

[![Burrito Bomber](img/4a7611d9a44075854ecb4acdadfefb62.png)](http://hackaday.com/?attachment_id=91364)

由 [Darwin Aerospace](http://www.darwinaerospace.com/ "Darwin Aerospace") 的人创造的[墨西哥卷饼轰炸机](http://www.darwinaerospace.com/burritobomber "Burrito Bomber")，声称是“世界上第一个墨西哥食品递送系统”交付流程始于顾客通过基于[烧瓶](http://flask.pocoo.org/ "Flask")的玉米煎饼炸弹 webapp 下订单。使用 [HTML5 地理定位 API](http://www.w3schools.com/html/html5_geolocation.asp "HTML5 Geolocation API") 从智能手机中获取客户的位置，并用于为无人机生成航路点文件。接下来，订单被放入递送管，装载到无人机上，航点文件被上传到无人机上。最后，无人机飞到你所在的位置，投下投送管。降落伞打开，安全地运送美味的有效载荷。

该无人机基于天行者 X-8 机身和量子 RTR 炸弹系统。炸弹系统提供了保持和投放有效载荷的基本机制，但达尔文空域为输送管设计了自己的 3D 打印部件。这些零件在 [Thingiverse](http://www.thingiverse.com/thing:36746 "Burrito Bomber on Thingiverse") 上有售。无人机由 [ArduPilot](http://code.google.com/p/ardupilot-mega/ "ArduPilot") 自主控制，它使用 webapp 的航路点输出来引导无人机到达目标并释放有效载荷。

不幸的是，由于联邦航空局的规定，这还不能成为商业产品，但联邦航空局被要求在 2015 年前制定出商业无人机法规。希望在 2015 年，我们都能用飞机订墨西哥卷饼。

对于所有的来源和模型，请查看该集团的 [Github](https://github.com/darwinaerospace/burritobomber "Burrito Bomber Github") 。休息之后还有一段投弹手的视频。

[https://www.youtube.com/embed/3lqMRHwGsRA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/3lqMRHwGsRA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)