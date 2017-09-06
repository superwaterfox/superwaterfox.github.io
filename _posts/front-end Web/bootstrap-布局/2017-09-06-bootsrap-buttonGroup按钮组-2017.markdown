---
layout:     post
title:      "bootstrap-buttonGroup"
subtitle:   " \"bootstrap-buttonGroup\""
date:       2017-09-06 17:40:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端
---


## bs3-button-toolbar分组btn-group
```
<div class="btn-toolbar" role="toolbar">
        <div class="btn-group">
            <button type="button" class="btn btn-default">1</button>
            <button type="button" class="btn btn-default">2</button>
            <button type="button" class="btn btn-default">3</button>
            <button type="button" class="btn btn-default">4</button>
        </div>
        <div class="btn-group">
            <button type="button" class="btn btn-default">5</button>
            <button type="button" class="btn btn-default">6</button>
            <button type="button" class="btn btn-default">7</button>
        </div>
        <div class="btn-group">
            <button type="button" class="btn btn-default">8</button>
        </div>
    </div>
```


## bs3-button-group 分组btn
```
 <div class="btn-group">
        <button type="button" class="btn btn-default">Left</button>
        <button type="button" class="btn btn-default">Middle</button>
        <button type="button" class="btn btn-default">Right</button>
    </div>
```

![](http://www.runoob.com/wp-content/uploads/2014/06/basicbuttongroup_demo.jpg)  
	btn-group分组是为了，里边的btn按钮，将原有的间隔去掉，那么每个按钮会进行重新排列，靠得比较近，从而达到分组的效果,如上图，如果不进行btn-group，那么三个按钮会有间距而分开
	
	
## bs3-button-group    归元button-dropdown
```
<div class="btn-group">
    <button type="button" class="btn btn-default">按钮 1</button>
    <button type="button" class="btn btn-default">按钮 2</button>
    <div class="btn-group">
    <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown">
        下列
        <span class="caret"></span>
    </button>
    <ul class="dropdown-menu">
        <li><a href="#">下拉链接 1</a></li>
        <li><a href="#">下拉链接 2</a></li>
    </ul>
    </div>
</div>
```
	由于.dropdown-menu样式渲染后，下拉的菜单是固定的。下拉按钮在btn-group重整后会移动位置，但是下拉菜单没有移动，需要在dropdown外围在加上 <div class="btn-group">进行菜单项归位

![](http://www.runoob.com/wp-content/uploads/2014/06/nestedbuttongrp_demo.jpg)
	如上，菜单项回归到下拉按钮上，如果不再包裹btn-group，菜单项会错位
	
## 调整group和toolbar的整体大小
```
按钮的大小是固定的三种：
.btn-group-lg, .btn-group-sm, .btn-group-xs
```

## 垂直按钮组.btn-group-vertical 