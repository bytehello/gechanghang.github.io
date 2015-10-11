---
layout: post
title: "Effective Object-C 2.0 tips_1"
date: 2015-10-11 10:30:35 +0800
comments: true
categories: Objective-C

---

#Effective Objective-C 2.0 tips_1
Objective-C 是C语言的超集，C语言可用的语法在OC中也是适用的。
##C和OC的区别
1. C语言是函数调用，OC是消息发送
2. 由第一点而来的不同就是：C语言这种采用函数调用的语言，是在运行时采用“虚方法表”的方式来确定该执行哪个函数；而OC是采用动态时绑定的方式来实现，也就是说只有在运行时才去查找要执行的方法，**而且**消息的接受对象也是运行时才能确定e

## OC的动态绑定

OC所能实现的运行时动态绑定是有**运行时组件**来完成的。**运行时组件**包含了OC中所有动态绑定需要的数据结构等等

##更好的理解OC

如下面

```
NSString *string = @"Hello World"

```
申明了一个**string**，**string**指向NSString的对象。它表示的是分配在堆中的一块内存，该内存里面保存了NSString对象
