# 如何运行这个项目

下载项目，然后用浏览器打开```index.html```。

# 项目目标

1、```index.html``` 在移动设备和桌面上的 ```PageSpeed``` 分数至少为90分；
2、对 ```views/js/main.js``` 进行的优化可使 ```views/pizza.html``` 在滚动时保持 ```60fps``` 的帧速；
3、利用 ```views/pizza.html``` 页面上的 pizza 尺寸滑块调整 pizza 大小的时间小于5毫秒，大小的调整时间在浏览器开发工具中显示。

# 项目优化概述

## 一、对于```index.html```的优化

1、利用```media:none```不阻塞渲染地加载Google font；
2、为```print.css```添加媒体属性;
3、内嵌```style.css```到```index.html```;
4、异步加载js文件。

## 二、在```views/js/main.js```中对于```pizza.html```的优化

1、使用```getElementById```替代```querySelector```;
2、删除```determineDx()```函数，优化```changePizzaSizes()```函数；
3、使用```tramsform```替代```left```去移动背景pizza;
4、减少pizza个数。

