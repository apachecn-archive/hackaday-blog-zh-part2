# 带高度控制的路由器桌

> 原文：<https://hackaday.com/2015/02/10/a-router-table-with-height-control/>

木刳刨机是一种多功能电动工具，价格低廉。更好的刳刨机安装在桌子下面，切割头穿过桌子。这使得使用该工具更加容易和安全。

[保罗]结合了他对电子和木工的兴趣，制作了一个带自动控制的[刳刨桌](http://hiramhouse.blogspot.be/p/v-behaviorurldefaultvmlo.html)[翻译](https://translate.google.ca/translate?sl=auto&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fhiramhouse.blogspot.be%2Fp%2Fv-behaviorurldefaultvmlo.html&edit-text=&act=url)。这种构造的巧妙之处在于自动高度控制，确保精确的切割深度。

刳刨机安装在螺纹杆上，这使得它可以通过马达上下移动。低成本 L298 电机驱动器为电机提供电源，电机由 Arduino Uno 控制。基于[传感器板](https://www.tindie.com/products/BBTech/vcnl4020-proximity-and-ambient-light-module/)的 [VCNL4020](http://www.vishay.com/optical-sensors/list/product-83476/) 用于测量距离和精确设置路由器高度。这个微小的接近传感器看起来像一个漂亮的芯片，在一个封装中提供高达 200 毫米的距离测量和环境光传感器。

路由表有一个 LCD 显示屏和按钮，允许用户拨入他们想要的高度。整个东西是用回收的碎片建造的，新零件不到 100 美元。