---
layout:     post
title:      "bootstrap-Alerts"
subtitle:   " \"bootstrap-Alerts\""
date:       2017-09-11 17:40:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端bootstrap
---

.media和.media-list都是可以通过media定义不规则的展示内容
```
<div class="media".           //定义多媒体范围
  <a class="media-left"       //定义多媒体定位是左边还是右边
    <img class="media-object"   //多媒体承载体
 </a>
  <div class="media-body       //多媒体主要文字区
     <h4 class="media-heading"     //多媒体标题
 ```
## .media 多媒体
```

<div class="media">
	<a class="media-left" href="#">
		<img class="media-object" src="/wp-content/uploads/2014/06/64.jpg" alt="媒体对象">
	</a>
	<div class="media-body">
		<h4 class="media-heading">媒体标题</h4>
		这是一些示例文本。这是一些示例文本。
		这是一些示例文本。这是一些示例文本。
		这是一些示例文本。这是一些示例文本。
		这是一些示例文本。这是一些示例文本。
		这是一些示例文本。这是一些示例文本。
		<div class="media">
			<a class="media-left" href="#">
				<img class="media-object" src="/wp-content/uploads/2014/06/64.jpg" alt="媒体对象">
			</a>
			<div class="media-body">
				<h4 class="media-heading">媒体标题</h4>
				这是一些示例文本。这是一些示例文本。
				这是一些示例文本。这是一些示例文本。
				这是一些示例文本。这是一些示例文本。
				这是一些示例文本。这是一些示例文本。
				这是一些示例文本。这是一些示例文本。
			</div>
		</div>
	</div>
</div>
<div class="media">
	<a class="media-left" href="#">
		<img class="media-object" src="/wp-content/uploads/2014/06/64.jpg" alt="媒体对象">
	</a>
	<div class="media-body">
		<h4 class="media-heading">媒体标题</h4>
		这是一些示例文本。这是一些示例文本。
		这是一些示例文本。这是一些示例文本。
		这是一些示例文本。这是一些示例文本。
		这是一些示例文本。这是一些示例文本。
		这是一些示例文本。这是一些示例文本。
	</div>
</div>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/mediaobject_demo.jpg)

## .media-list  列表多媒体
```
<ul class="media-list">
	<li class="media">
		<a class="media-left" href="#">
			<img class="media-object" src="/wp-content/uploads/2014/06/64.jpg"
				 alt="通用的占位符图像">
		</a>
		<div class="media-body">
			<h4 class="media-heading">媒体标题</h4>
			<p>这是一些示例文本。这是一些示例文本。
				这是一些示例文本。这是一些示例文本。
				这是一些示例文本。这是一些示例文本。
				这是一些示例文本。这是一些示例文本。
				这是一些示例文本。这是一些示例文本。</p>
			<!-- 嵌套的媒体对象 -->
			<div class="media">
				<a class="media-left" href="#">
					<img class="media-object" src="/wp-content/uploads/2014/06/64.jpg"
						 alt="通用的占位符图像">
				</a>
				<div class="media-body">
					<h4 class="media-heading">嵌套的媒体标题</h4>
					这是一些示例文本。这是一些示例文本。
					这是一些示例文本。这是一些示例文本。
					这是一些示例文本。这是一些示例文本。
					这是一些示例文本。这是一些示例文本。
					这是一些示例文本。这是一些示例文本。
					<!-- 嵌套的媒体对象 -->
					<div class="media">
						<a class="media-left" href="#">
							<img class="media-object" src="/wp-content/uploads/2014/06/64.jpg"
								 alt="通用的占位符图像">
						</a>
						<div class="media-body">
							<h4 class="media-heading">嵌套的媒体标题</h4>
							这是一些示例文本。这是一些示例文本。
							这是一些示例文本。这是一些示例文本。
							这是一些示例文本。这是一些示例文本。
							这是一些示例文本。这是一些示例文本。
							这是一些示例文本。这是一些示例文本。
						</div>
					</div>
				</div>
			</div>
			<!-- 嵌套的媒体对象 -->
			<div class="media">
				<a class="media-left" href="#">
					<img class="media-object" src="/wp-content/uploads/2014/06/64.jpg"
						 alt="通用的占位符图像">
				</a>
				<div class="media-body">
					<h4 class="media-heading">嵌套的媒体标题</h4>
					这是一些示例文本。这是一些示例文本。
					这是一些示例文本。这是一些示例文本。
					这是一些示例文本。这是一些示例文本。
					这是一些示例文本。这是一些示例文本。
					这是一些示例文本。这是一些示例文本。
				</div>
			</div>
		</div>
	</li>
	<li class="media">
		<a class="pull-right" href="#">
			<img class="media-object" src="/wp-content/uploads/2014/06/64.jpg"
				 alt="通用的占位符图像">
		</a>
		<div class="media-body">
			<h4 class="media-heading">媒体标题</h4>
			这是一些示例文本。这是一些示例文本。
			这是一些示例文本。这是一些示例文本。
			这是一些示例文本。这是一些示例文本。
			这是一些示例文本。这是一些示例文本。
			这是一些示例文本。这是一些示例文本。
		</div>
	</li>
</ul>
```