---
layout:     post
title:      "bootstrap表格"
subtitle:   " \"bootstrap表格\""
date:       2017-09-05 16:52:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端
---

> “一站式，就缺前端 ”


## 表格标签
```
<table>	为表格添加基础样式。
<thead>	表格标题行的容器元素（<tr>），用来标识表格列。
<tbody>	表格主体中的表格行的容器元素（<tr>）。
<tr>	一组出现在单行上的表格单元格的容器元素（<td> 或 <th>）。
<td>	默认的表格单元格。
<th>	特殊的表格单元格，用来标识列或行（取决于范围和位置）。必须在 <thead> 内使用。
<caption>	关于表格存储内容的描述或总结。
```

## 表格样式
```
.table	为任意 <table> 添加基本样式 (只有横向分隔线)	
.table-striped	在 <tbody> 内添加斑马线形式的条纹 ( IE8 不支持)	尝试一下
.table-bordered	为所有表格的单元格添加边框	
.table-hover	在 <tbody> 内的任一行启用鼠标悬停状态	
.table-condensed	  让表格更加紧凑,通过将行内间距进行调少
```

## tr ,th,td标签样式
```
.active	将悬停的颜色应用在行或者单元格上	尝试一下
.success	表示成功的操作	尝试一下
.info	表示信息变化的操作	尝试一下
.warning	表示一个警告的操作	尝试一下
.danger	表示一个危险的操作
```
![image](http://www.runoob.com/wp-content/uploads/2014/06/contextualtable_demo.jpg)

## 响应式表格边框表格

```
<div class="table-responsive">
  <table class="table">
```