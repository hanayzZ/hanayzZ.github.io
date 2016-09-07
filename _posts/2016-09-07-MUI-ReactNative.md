---
layout: post
title:  "比较MUI和ReactNative"
date:   2016-09-07
desc: "MUI和ReactNative的比较"
keywords: "MUI,ReactNative"
categories: [HTML]
tags: [MUI,ReactNative]
icon: icon-phone-gap
---

> 

MUI:
MUI的核心还是webview,和phonegap或者自己编写的webview核心原理差不多。只是MUI通过CSS动画、预加载、多个webview的显示隐藏等技术，比常规的纯webview还是好很多。同时，html5+提供很多与手机原生交互的接口，实质就是通过JS调取原生系统接口。当然，MUI也支持通过JS完全调用原生UI。虽然框架支持调用原生的，但是和原生开发工作量和技术难度差不多，所以调用原生框架只能在极少情况下使用。

缺点：项目越大，页面越多，流程性越差，有天花板，优化的效果并不明显。稍微具有一定规模的项目，或者对流畅性要求较高的项目，建议不要用MUI。

ReactNative：
ReactNative与MUI最大的区别就是，ReactNative不是Webview的方式进行开发，语法虽然是JS，但是和MUI是完全不同的两个东西，产生的UI、动画基本都是原生的UI、动画，流畅度媲美原生。

缺点：学习成本和学习曲线还是比较高的，真的需要一段时间去学习。JSX看起来像JS，但是部分语法很奇葩。界面布局和CSS完全不一样，state和props相对还是比较好理解的，团队的学习成本更高。性能上可以说是完胜MUI。

结论：对流畅性要求不太高的，可以考虑MUI。开发速度快，成本低。对流程性要求高的，还是用ReactNative吧。



转载知乎


