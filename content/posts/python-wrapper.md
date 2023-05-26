---
title: "Python从入门到放弃：装饰器"
date: 2023-05-26T17:26:01+08:00
description: ""
draft: true
author: "LotuSrc"
cover: ""
tags: ["python"]
theme: "light"
---
Python装饰器的官方定义，本质上是一个Python函数，它可以让其他函数在不需要做任何代码改动的前提下增加额外的功能，在打印日志、测试性能等场景下经常被使用。
装饰器就好比是给礼物包装的盒子，它有三个特点：
- 不能改变礼物本身（不能改变函数的内部代码）
- 送礼物时，礼物和包装盒是一起的（调用函数时装饰器一并调用）
- 送礼物时，只会说礼物的名字，而不是包装盒的名字（使用函数名调用函数）
我们定义一个函数
```python
def func():
    print('run func')

func()

```

