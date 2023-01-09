# 重新设计的自行车灯控制器

> 原文：<https://hackaday.com/2014/11/06/redesigned-bike-light-controller/>

[JP]正在寻找一款自行车灯，以便在他家附近进行夜间骑行。他找到了一个价格合理的灯，适合他的需要，但当他开始使用它时，他发现控制器有点暗淡。为了解决其中的一些问题，他最终从零开始建造了自己的照明控制器。

最初的控制器的主要问题是它不能消除单个按钮输入的抖动。这意味着按一下按钮可能会导致它在两种或三种不同的模式之间循环，这很不方便，也很烦人。新的控制器解决了这个问题，同时实现了几个新的亮度模式和一个“频闪”模式，用于通勤上班，以帮助提醒其他司机注意[JP]的自行车。

虽然[JP]指出 Arduino 在这种情况下非常容易使用，但它不适合原始外壳。他带了一个 8 针的 ATtiny45，大小正好满足他的需要。一切都完美地结合在一起，比原来的有用得多。也许下一步他可以给它配一个比他现在使用的更亮的[灯。](http://hackaday.com/2011/11/28/building-a-1300-lumen-bike-light/)