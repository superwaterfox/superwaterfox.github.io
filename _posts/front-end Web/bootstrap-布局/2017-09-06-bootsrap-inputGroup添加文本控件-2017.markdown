---
layout:     post
title:      "bootstrap-inputTextGroup"
subtitle:   " \"bootstrap-inputTextGroup\""
date:       2017-09-06 17:40:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端bootstrap
---


## inputTextGroup 为input<Text>的前缀和后缀添加任意元素
```
<div class="input-group">
            <span class="input-group-addon">@</span>
            <input type="text" class="form-control" placeholder="twitterhandle">
        </div>
```

	Input标签添加文本说明或者图标的时候，不需要考虑样式和间距，直接使用<div class="input-group">包裹就可以成为一行了。同时这个元素使用 <span class="input-group-addon">进行包裹，如果是button那么需要用.input-group-btn来包裹
	
	
## inputTextGroup 调整一整行的大小
```
 .input-group-lg
 .input-group-sm
```

## 为inputText添加复选框和单选框 。
	使用<span class="input-group-addon"进行渲染
```
<div style="padding: 100px 100px 10px;">
    <form class="bs-example bs-example-form" role="form">
        <div class="row">
            <div class="col-lg-6">
                <div class="input-group">
                    <span class="input-group-addon">
                        <input type="checkbox"></span>
                    <input type="text" class="form-control">
                </div><!-- /input-group -->
            </div><!-- /.col-lg-6 -->
            <br>
            <div class="col-lg-6">
                <div class="input-group">
                    <span class="input-group-addon">
                        <input type="radio"></span>
                    <input type="text" class="form-control">
                </div><!-- /input-group -->
            </div><!-- /.col-lg-6 -->
        </div><!-- /.row -->
    </form>
</div>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/inputgrpradiochkbox_demo.jpg)

## 为inputText添加button
	使用.input-group-btn进行渲染
```
<div style="padding: 100px 100px 10px;">
    <form class="bs-example bs-example-form" role="form">
        <div class="row">
            <div class="col-lg-6">
                <div class="input-group">
                    <span class="input-group-btn">
                        <button class="btn btn-default" type="button">Go!</button>
                    </span>
                    <input type="text" class="form-control">
                </div><!-- /input-group -->
            </div><!-- /.col-lg-6 -->
            <br>
            <div class="col-lg-6">
                <div class="input-group">
                    <input type="text" class="form-control">
                    <span class="input-group-btn">
                        <button class="btn btn-default" type="button">Go!</button>
                    </span>
                </div><!-- /input-group -->
            </div><!-- /.col-lg-6 -->
        </div><!-- /.row -->
    </form>
</div>
```

![](http://www.runoob.com/wp-content/uploads/2014/06/Inputgrpbuttonaddons_demo.jpg)

## 为inputText添加dropdown下拉菜单
	 .input-group-btn进行渲染
```
<div style="padding: 100px 100px 10px;">
    <form class="bs-example bs-example-form" role="form">
        <div class="row">
            <div class="col-lg-6">
                <div class="input-group">
                    <div class="input-group-btn">
                        <button type="button" class="btn btn-default 
                        dropdown-toggle" data-toggle="dropdown">下拉菜单
                            <span class="caret"></span>
                        </button>
                        <ul class="dropdown-menu">
                            <li>
                                <a href="#">功能</a>
                            </li>
                            <li>
                                <a href="#">另一个功能</a>
                            </li>
                            <li>
                                <a href="#">其他</a>
                            </li>
                            <li class="divider"></li>
                            <li>
                                <a href="#">分离的链接</a>
                            </li>
                        </ul>
                    </div><!-- /btn-group -->
                    <input type="text" class="form-control">
                </div><!-- /input-group -->
            </div><!-- /.col-lg-6 -->
            <br>
            <div class="col-lg-6">
                <div class="input-group">
                    <input type="text" class="form-control">
                    <div class="input-group-btn">
                        <button type="button" class="btn btn-default 
                        dropdown-toggle" data-toggle="dropdown">下拉菜单
                            <span class="caret"></span>
                        </button>
                        <ul class="dropdown-menu pull-right">
                            <li>
                                <a href="#">功能</a>
                            </li>
                            <li>
                                <a href="#">另一个功能</a>
                            </li>
                            <li>
                                <a href="#">其他</a>
                            </li>
                            <li class="divider"></li>
                            <li>
                                <a href="#">分离的链接</a>
                            </li>
                        </ul>
                    </div><!-- /btn-group -->
                </div><!-- /input-group -->
            </div><!-- /.col-lg-6 -->
        </div><!-- /.row -->
    </form>
</div>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/inputgrpbtndropdown_demo.jpg)