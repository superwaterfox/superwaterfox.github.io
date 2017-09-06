---
layout:     post
title:      "bootstrap-dropdown"
subtitle:   " \"bootstrap-dropdown\""
date:       2017-09-06 17:40:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端
---


## Dropdown
```
<div class="dropdown">
        <button class="btn btn-default dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown">
            Dropdown
            <span class="caret"></span>
        </button>
        <ul class="dropdown-menu" role="menu" aria-labelledby="dropdownMenu1">
            <li role="presentation" class="dropdown-header">Dropdown header</li>
            <li role="presentation"><a role="menuitem" tabindex="-1" href="#">Action</a></li>
            <li role="presentation"><a role="menuitem" tabindex="-1" href="#">Another action</a></li>
            <li role="presentation" class="disabled"><a role="menuitem" tabindex="-1" href="#">Something else here</a>
            </li>
            <li role="presentation" class="divider"></li>
            <li role="presentation" class="dropdown-header">Dropdown header</li>
            <li role="presentation"><a role="menuitem" tabindex="-1" href="#">Separated link</a></li>
        </ul>
    </div>
```


```
.dropdown	指定下拉菜单，下拉菜单都包裹在 .dropdown 里	
.dropdown-menu	创建下拉菜单	
.dropdown-menu-right	下拉菜单右对齐	
.dropdown-header	下拉菜单中添加标题	
.dropup	指定向上弹出的下拉菜单	
.disabled	下拉菜单中的禁用项	 
.divider	下拉菜单中的分割线  <li class="divider"></li>
```


## Dropdown的按钮大小
```
按钮大小总共有三种，菜单大小是没办法改变的
.btn-large、.btn-sm 或 .btn-xs
```

```
<div class="btn-group">
    <button type="button" class="btn btn-default dropdown-toggle btn-lg" data-toggle="dropdown">默认
        <span class="caret"></span>
    </button>
```