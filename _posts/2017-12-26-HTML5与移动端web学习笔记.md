---
title:        "HTML5与移动端web学习笔记"
description:  "web"
image:        "http://placehold.it/400x200"
author:       "Amadues"
---
# HTML5 提供了很多新的功能，主要有：
新的 HTML 元素，例如 section, nav, header, footer, article 等
用于绘画的 Canvas 元素
用于多媒体播放的 video 和 audio 元素
用于定位的 Geolocation API
本地存储以及离线应用
Web Workers、Web WebSocket API
# 移动前端开发可分为：

手机网页开发。这部分跟web前端开发差别不大，使用的技术都是html+css+js。区别为手机浏览器是webkit的天下，pc端是IE的天下。
App前端开发。使用的技术也是html+css+js，但它需要基于PhoneGap，React Native等开发平台调用手机核心功能接口（包括地理定位，加速器，联系人，声音和振动等）模拟native app，这部分跟web前端开发完全不同。最终代码发布要分别编译成各系统平台的app。

# drag and drop(拖拽)

拖拽元素事件: 事件对象为被拖拽元素

dragstart:  拖拽前触发 
drag:拖拽前、拖拽结束之间，连续触发
dragend: 拖拽结束触发
# 目标元素事件: 事件对象为目标元素

dragenter:  进入目标元素触发，相当于mouseover
dragover: 进入目标、离开目标之间，连续触发
dragleave:  离开目标元素触发，相当于mouseout
drop: 在目标元素上释放鼠标触发
# 事件的执行顺序 ：drop不触发的时候

dragstart  >  drag >  dragenter >  dragover >  dragleave > dragend 
# 事件的执行顺序 ：drop触发的时候(dragover的时候阻止默认事件)

dragstart  >  drag >  dragenter >  dragover >  drop > dragend
# 解决火狐下的问题

火狐浏览器下必须设置dataTransfer对象的setData方法才可以拖拽除图片外的其他标签。

# dataTransfer属性和方法
![Mou icon](https://i.loli.net/2018/01/03/5a4ca7cf255c8.png)
# 只有加阻止默认事件才可以触发drop
![Mou icon]()
#drag and drop的浏览器支持情况：
![Mou icon](https://i.loli.net/2018/01/03/5a4ca7cf26cba.jpg)
***
# FileReader(读取文件信息)
![Mou icon](https://i.loli.net/2018/01/03/5a4ca7cf294e1.jpg
)




  










