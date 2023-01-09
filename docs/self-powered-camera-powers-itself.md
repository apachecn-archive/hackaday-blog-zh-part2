# 自供能相机自己供电

> 原文：<https://hackaday.com/2015/04/18/self-powered-camera-powers-itself/>

相机感应光线来创建图像，太阳能电池将光线转化为能量。为什么不把两者融合在一起，创造一个[自供电相机](http://www.cs.columbia.edu/CAVE/projects/self_powered_camera/)？

哥伦比亚大学的计算机视觉实验室制造了这种独特的相机，它从光电二极管传感器中获取能量。这些光电二极管还充当可以恢复图像的像素阵列。结果是黑白摄像机不需要外部电源。

能量采集器电路为超级电容充电，为系统供电。相机的帧速率受到可以收获的能量的限制:更高的帧速率需要更多的能量。出于这个原因，该团队开发了一种基于可用能量改变帧速率的算法。

用于该构建的 [MC13226V](http://www.freescale.com/webapp/sps/site/prod_summary.jsp?code=MC13226V) 微控制器具有内部 2.4 GHz 无线电。该小组提到，无线功能是未来的一个可能特征，这将使一个完全不受束缚的，无电池的相机。