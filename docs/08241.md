# 打造自己的 Gear VR

> 原文：<https://hackaday.com/2015/02/05/build-your-own-gear-vr/>

随着三星新 Gear VR 的公布，开发者和 VR 爱好者正在等待智能手机连接的 VR 耳机的发布。有几个人迫不及待地想染指这个平台，于是他们创造了一款 Gear VR 兼容耳机， [OpenGear](http://open-gear.com/) 。

OpenGear 从三星 Galaxy Note 4 开始，这是 Gear VR 头戴设备的目标平台。一个纸板外壳，类似于[谷歌纸板](http://hackaday.com/2014/07/12/google-cardboard-vr-kit-for-under-15/)耳机，容纳镜头并将手机绑在你的脸上。

唯一缺少的部分是运动跟踪电子设备。幸运的是，ST 的 [STM32F3 Discovery](http://www.st.com/web/catalog/tools/FM116/SC959/SS1532/PF254044) 开发板拥有所需的一切:一个支持 USB 设备的微控制器、一个 [L3GD20](http://www.st.com/web/catalog/sense_power/FM89/SC1288/PF252443?sc=internet/analog/product/252443.jsp) 3 轴陀螺仪和一个 [LSM303DLHC](http://www.st.com/web/catalog/sense_power/FM89/SC1449/PF251940) 加速度计/磁力计。这些组件共同提供了一个 USB 惯性测量单元，用于跟踪您的头部。

发现板绑在纸板耳机上，一个[开源固件](https://github.com/yetifrisstlama/Foculus_Rift_Tracker_STM32F3DISCOVERY)被刷新。这模拟了由合法的 Oculus Rift 运动跟踪器发送的消息。Galaxy Note 4 将该设备视为 VR 耳机，并允许您运行 VR 应用程序。

如果您感兴趣，OpenGear 团队将提供一个开发工具包。对于开发者来说，这是在 Gear VR 实际发布之前抢先开发应用程序的好方法。主要的缺点是你把这个东西贴在脸上会是什么样子。休息之后有一场与真实 Gear VR 的正面交锋。

[通过[路到 VR](http://www.roadtovr.com/can-now-clone-gear-vr-test-virtual-reality-apps/)

[https://www.youtube.com/embed/vgajSfh0W_I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=280&wmode=transparent](https://www.youtube.com/embed/vgajSfh0W_I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=280&wmode=transparent)