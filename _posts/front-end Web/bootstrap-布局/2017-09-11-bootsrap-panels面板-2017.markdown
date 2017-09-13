---
layout:     post
title:      "bootstrap-panels面板"
subtitle:   " \"bootstrap-panels面板\""
date:       2017-09-11 17:40:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端bootstrap
---


div .panel   面板标记
div .panel-default 默认面板样式
div .panel-heading  面板标题样式
h3 .panel-title    面板标题文字样式

```
<div class="panel panel-default">
		<div class="panel-heading">
		   <h3 class="panel-title">
        带 title 的面板标题
           </h3>
    </div>
    <div class="panel-body">
        这是一个基本的面板
    </div>
</div>
```

  
## 面板样式
```
.panel-primary
.panel-success
.panel-info
.panel-warning
.panel-danger
```
![](http://www.runoob.com/wp-content/uploads/2014/06/panelstyles_demo.jpg)

## 带列表组的面板
```
<div class="panel panel-default">
    <div class="panel-heading">面板标题</div>
    <div class="panel-body">
        <p>这是一个基本的面板内容。这是一个基本的面板内容。
            这是一个基本的面板内容。这是一个基本的面板内容。
            这是一个基本的面板内容。这是一个基本的面板内容。
            这是一个基本的面板内容。这是一个基本的面板内容。
        </p>
    </div>
    <ul class="list-group">
        <li class="list-group-item">免费域名注册</li>
        <li class="list-group-item">免费 Window 空间托管</li>
        <li class="list-group-item">图像的数量</li>
        <li class="list-group-item">24*7 支持</li>
        <li class="list-group-item">每年更新成本</li>
    </ul>
</div>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/panellistgroups_demo.jpg)