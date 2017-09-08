---
layout:     post
title:      "bootstrap-navbar导航栏"
subtitle:   " \"bootstrap-navbar导航栏\""
date:       2017-09-08 17:10:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端
---

## Bootstrap 导航栏<nav class="navbar navbar-default" role="navigation">
使用<nav可以自适应到视图，缩进和扩展。没有这个标签的时候就可以查看这篇文章  
[bootsrap-nav导航元素](./2017-09-06-bootsrap-nav导航元素-2017.markdown)


### nav包裹
```
<nav class="navbar navbar-default" role="navigation">
```

### 标题内容navbar-header
```
<div class="navbar-header">
        <a class="navbar-brand" href="#">菜鸟教程</a>
    </div>
```
## 普通标签页举例
```
<nav class="navbar navbar-default" role="navigation">
    <div class="container-fluid">
    <div class="navbar-header">
        <a class="navbar-brand" href="#">菜鸟教程</a>
    </div>
    <div>
        <ul class="nav navbar-nav">
            <li class="active"><a href="#">iOS</a></li>
            <li><a href="#">SVN</a></li>
            <li class="dropdown">
                <a href="#" class="dropdown-toggle" data-toggle="dropdown">
                    Java
                    <b class="caret"></b>
                </a>
                <ul class="dropdown-menu">
                    <li><a href="#">jmeter</a></li>
                    <li><a href="#">EJB</a></li>
                    <li><a href="#">Jasper Report</a></li>
                    <li class="divider"></li>
                    <li><a href="#">分离的链接</a></li>
                    <li class="divider"></li>
                    <li><a href="#">另一个分离的链接</a></li>
                </ul>
            </li>
        </ul>
    </div>
    </div>
</nav>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/C927D25C-CA7D-4FD1-8651-5680874BBE3E.jpg)


---

## 折叠导航栏
	简单解释：nav包裹，同时使用navbar-header作为标题，标题的位置作为按钮，同时添加事件和样式class="navbar-toggle" data-toggle="collapse"，接下来就是样式填充
	
	
	<div class="navbar-header">
		 <button type="button" class="navbar-toggle" data-toggle="collapse"
                data-target="#example-navbar-collapse">


```
<nav class="navbar navbar-default" role="navigation">
    <div class="container-fluid">
    <div class="navbar-header">
        <button type="button" class="navbar-toggle" data-toggle="collapse"
                data-target="#example-navbar-collapse">
            <span class="sr-only">切换导航</span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
        </button>
        <a class="navbar-brand" href="#">菜鸟教程</a>
    </div>
    <div class="collapse navbar-collapse" id="example-navbar-collapse">
        <ul class="nav navbar-nav">
            <li class="active"><a href="#">iOS</a></li>
            <li><a href="#">SVN</a></li>
            <li class="dropdown">
                <a href="#" class="dropdown-toggle" data-toggle="dropdown">
                    Java <b class="caret"></b>
                </a>
                <ul class="dropdown-menu">
                    <li><a href="#">jmeter</a></li>
                    <li><a href="#">EJB</a></li>
                    <li><a href="#">Jasper Report</a></li>
                    <li class="divider"></li>
                    <li><a href="#">分离的链接</a></li>
                    <li class="divider"></li>
                    <li><a href="#">另一个分离的链接</a></li>
                </ul>
            </li>
        </ul>
    </div>
    </div>
</nav>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/98B4B325-7C69-4C93-8419-8B77D12395D5.jpg)


## 结合图标的导航栏
```
<nav class="navbar navbar-default" role="navigation"> 
    <div class="container-fluid"> 
        <div class="navbar-header"> 
            <a class="navbar-brand" href="#">菜鸟教程</a> 
        </div> 
        <ul class="nav navbar-nav navbar-right"> 
            <li><a href="#"><span class="glyphicon glyphicon-user"></span> 注册</a></li> 
            <li><a href="#"><span class="glyphicon glyphicon-log-in"></span> 登录</a></li> 
        </ul> 
    </div> 
</nav>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/64E5993E-ED1A-4B72-AE90-50076B78224D.jpg)



## 其他
```
导航栏中的表单 <form class="navbar-form  
纯文本.   <p class="navbar-text
纯button没有form标签  可以使用 <button class="navbar-btn
```

## 导航栏的对齐方式
	使用上边的所有navbar的标签，都可以配套使用以下的标签
	.navbar-right
	.navbar-left
```
<nav class="navbar navbar-default" role="navigation">
    <div class="container-fluid">
    <div class="navbar-header">
        <a class="navbar-brand" href="#">菜鸟教程</a>
    </div>
    <div>
        <!--向左对齐-->
        <ul class="nav navbar-nav navbar-left">
            <li class="dropdown">
                <a href="#" class="dropdown-toggle" data-toggle="dropdown">
                    Java
                    <b class="caret"></b>
                </a>
                <ul class="dropdown-menu">
                    <li><a href="#">jmeter</a></li>
                    <li><a href="#">EJB</a></li>
                    <li><a href="#">Jasper Report</a></li>
                    <li class="divider"></li>
                    <li><a href="#">分离的链接</a></li>
                    <li class="divider"></li>
                    <li><a href="#">另一个分离的链接</a></li>
                </ul>
            </li>
        </ul>
        <form class="navbar-form navbar-left" role="search">
            <button type="submit" class="btn btn-default">
                向左对齐-提交按钮
            </button>
        </form>
        <p class="navbar-text navbar-left">向左对齐-文本</p>
        <!--向右对齐-->
        <ul class="nav navbar-nav navbar-right">
            <li class="dropdown">
                <a href="#" class="dropdown-toggle" data-toggle="dropdown">
                    Java <b class="caret"></b>
                </a>
                <ul class="dropdown-menu">
                    <li><a href="#">jmeter</a></li>
                    <li><a href="#">EJB</a></li>
                    <li><a href="#">Jasper Report</a></li>
                    <li class="divider"></li>
                    <li><a href="#">分离的链接</a></li>
                    <li class="divider"></li>
                    <li><a href="#">另一个分离的链接</a></li>
                </ul>
            </li>
        </ul>
        <form class="navbar-form navbar-right" role="search">
            <button type="submit" class="btn btn-default">
                向右对齐-提交按钮
            </button>
        </form>
        <p class="navbar-text navbar-right">向右对齐-文本</p>
    </div>
    </div>
</nav>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/B4F6F15B-EFAC-44D7-A577-2F36ED59252C.jpg)

## 不受影响的顶部.navbar-fixed-top
	<nav class="navbar navbar-default navbar-fixed-top" role="navigation">
由于会受其他模块样式影响，有可能会顶走nav标签的样式，可以添加navbar-fixed-top 进行永远漂浮置顶

## 底部.navbar-fixed-bottom
## 黑色主题.navbar-inverse