---
layout:     post
title:      "bootstrap-listGroup"
subtitle:   " \"bootstrap-listGroup\""
date:       2017-09-11 17:40:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端bootstrap
---

	.list-group   标记区域
	.list-group-item   标记列表样式
	这两个样式支持ul和li，div和a
	
	list-group-item-heading 标题
	list-group-item-text   文字
	
	
## ul和li添加下拉并且支持微章
```
	<ul class="list-group">
    <li class="list-group-item">免费域名注册</li>
    <li class="list-group-item">免费 Window 空间托管</li>
    <li class="list-group-item">
        <span class="badge">新</span>
        折扣优惠
    </li>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/badgeslistgroup_demo.jpg)

## div 和a
```
	<div class="list-group">
<a href="#" class="list-group-item active">
	免费域名注册
</a>
<a href="#" class="list-group-item">24*7 支持</a>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/linkslistgroup_demo.jpg)


## div 和 a 同时添加标题和文本
```
<div class="list-group">
    <a href="#" class="list-group-item active">
        <h4 class="list-group-item-heading">
            入门网站包
        </h4>
    </a>
    <a href="#" class="list-group-item">
        <h4 class="list-group-item-heading">
            免费域名注册
        </h4>
        <p class="list-group-item-text">
            您将通过网页进行免费域名注册。
        </p>
    </a>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/customcontentlistgroup_demo.jpg)