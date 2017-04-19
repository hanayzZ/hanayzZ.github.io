---
layout: post
title:  "JavaScript基于原型链的继承的js工具库的实现方法"
date:   2016-09-13
desc: "JavaScript基于原型链的继承的js工具库的实现方法"
keywords: "JavaScript,Prototype,继承"
categories: [JavaScript]
tags: [JavaScript]
icon: icon-javascript
---

### 一、__proto__属性（原型指针）和prototype属性（原型对象）

代码如下：

``` javascript
window.prototype === window.__proto__
false
Window.prototype === window.__proto__
true
window.constructor === Window
true
Window.__proto__.__proto__.__proto__.__proto__
null
```


个构造函数都有一个原型对象(prototype)，原型对象都包含一个指向构造函数的指针(constructor)，而实例都包含一个指向原型对象的内部指针(__proto__)。
除了使用__proto__方式访问对象的原型，还可以通过Object.getPrototypeOf方法来获取对象的原型，以及通过Object.setPrototypeOf方法来重写对象的原型。__proto__属性只有浏览器才需要部署，其他环境可以没有这个属性，而且前后的两根下划线，表示它本质是一个内部属性，不应该对使用者暴露。
instanceof和Object.isPrototypeOf()可以判断两个对象是否是继承关系。

文章：
JavaScript面向对象简介
JavaScript 原型中的哲学思想
Javascript继承机制的设计思想

### 二、打造一个自己的类jQuery的js工具库
 闭包
代码如下：

``` javascript
if (foo) bar(); ==> foo && bar();
if (!foo) bar(); ==> foo || bar();
```

### 三、省略大括号{}

代码如下：

``` javascript
if (foo) return bar(); else other(); ==> {if (foo) return bar();other()}
```

