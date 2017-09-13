---
layout:     post
title:      "bootstrap-Scrollspy滚动插件"
subtitle:   " \"bootstrap-Scrollspy滚动插件\""
date:       2017-09-11 17:40:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端bootstrap
---

## 用法
	通过 data 属性：向您想要监听的元素（通常是 body）添加 data-spy="scroll"。然后添加带有 Bootstrap .nav 组件的父元素的 ID 或 class 的属性 data-target。为了它能正常工作，您必须确保页面主体中有匹配您所要监听链接的 ID 的元素存在。
```
<body data-spy="scroll" data-target=".navbar-example">
...
<div class="navbar-example">
	<ul class="nav nav-tabs">
		...
	</ul>
</div>
...
</body>
```
或者
```
$('body').scrollspy({ target: '.navbar-example' })
```