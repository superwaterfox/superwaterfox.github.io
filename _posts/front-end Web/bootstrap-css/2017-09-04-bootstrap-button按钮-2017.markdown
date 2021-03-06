---
layout:     post
title:      "bootstrap的Button"
subtitle:   " \"bootstrap的Button\""
date:       2017-09-06 15:20:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端bootstrap
---

> “一站式，就缺前端 ”

## button按钮样式
```
.btn	为按钮添加基本样式	
.btn-default	默认/标准按钮	
.btn-primary	原始按钮样式（未被操作）	
.btn-success	表示成功的动作	
.btn-info	该样式可用于要弹出信息的按钮	
.btn-warning	表示需要谨慎操作的按钮	
.btn-danger	表示一个危险动作的按钮操作	
.btn-link	让按钮看起来像个链接 (仍然保留按钮行为)	
.btn-lg	制作一个大按钮	
.btn-sm	制作一个小按钮	
.btn-xs	制作一个超小按钮	
.btn-block	块级按钮(拉伸至父元素100%的宽度)	
.active	按钮被点击	
.disabled	禁用按钮
```
```
<!-- 标准的按钮 -->
<button type="button" class="btn btn-default">默认按钮</button>
<!-- 提供额外的视觉效果，标识一组按钮中的原始动作 -->
<button type="button" class="btn btn-primary">原始按钮</button>
<!-- 表示一个成功的或积极的动作 -->
<button type="button" class="btn btn-success">成功按钮</button>
<!-- 信息警告消息的上下文按钮 -->
<button type="button" class="btn btn-info">信息按钮</button>
<!-- 表示应谨慎采取的动作 -->
<button type="button" class="btn btn-warning">警告按钮</button>
<!-- 表示一个危险的或潜在的负面动作 -->
<button type="button" class="btn btn-danger">危险按钮</button>
<!-- 并不强调是一个按钮，看起来像一个链接，但同时保持按钮的行为 -->
<button type="button" class="btn btn-link">链接按钮</button>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/buttonoptions_demo.jpg)


## 按钮大小
```
.btn-lg	这会让按钮看起来比较大。
.btn-sm	这会让按钮看起来比较小。
.btn-xs	这会让按钮看起来特别小。
.btn-block	这会创建块级的按钮，会横跨父元素的全部宽度。
```
```
<p>
  <button type="button" class="btn btn-primary btn-lg">大的原始按钮</button>
  <button type="button" class="btn btn-default btn-lg">大的按钮</button>
</p>
<p>
  <button type="button" class="btn btn-primary">默认大小的原始按钮</button>
  <button type="button" class="btn btn-default">默认大小的按钮</button>
</p>
<p>
  <button type="button" class="btn btn-primary btn-sm">小的原始按钮</button>
  <button type="button" class="btn btn-default btn-sm">小的按钮</button>
</p>
<p>
  <button type="button" class="btn btn-primary btn-xs">特别小的原始按钮</button>
  <button type="button" class="btn btn-default btn-xs">特别小的按钮</button>
</p>
<p>
  <button type="button" class="btn btn-primary btn-lg btn-block">块级的原始按钮</button>
  <button type="button" class="btn btn-default btn-lg btn-block">块级的按钮</button>
</p>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/buttonsize_demo.jpg)

## 按钮状态
```
 .active   激活，选中
```