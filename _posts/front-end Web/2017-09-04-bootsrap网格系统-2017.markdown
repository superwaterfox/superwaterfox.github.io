---
layout:     post
title:      "bootstrap学习"
subtitle:   " \"bootstrap学习\""
date:       2017-09-04 16:30:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端
---

> “一站式，就缺前端 ”





## bootstrap的.container网格系统

1  | 2| 3| 4| 5| 6| 7 | 8 | 9 | 10 | 11 | 12
---|---|---|---|---|---|---|---|---|---|---|---
1 | 1|1| 1| 1| 1| 1| 1| 1| 1| 1| 1

	>将屏幕进行12等分，那么切换设备就进行拆分比例。例如12个1，
	444，48，66，12只有四个。这里的网格不是长度，而是位置
	
	
	### 查看几个常见的位置
```

    <table class="grid" cellspacing="0">
        <tbody>
        <tr>
            <td width="8.33%">1</td>
            <td width="8.33%">1</td>
            <td width="8.33%">1</td>
            <td width="8.33%">1</td>
            <td width="8.33%">1</td>
            <td width="8.33%">1</td>
            <td width="8.33%">1</td>
            <td width="8.33%">1</td>
            <td width="8.33%">1</td>
            <td width="8.33%">1</td>
            <td width="8.33%">1</td>
            <td width="8.33%">1</td>
        </tr>
        <tr>
            <td colspan="4">4</td>
            <td colspan="4">4</td>
            <td colspan="4">4</td>
        </tr>
        <tr>
            <td colspan="4">4</td>
            <td colspan="8">8</td>
        </tr>
        <tr>
            <td colspan="6">6</td>
            <td colspan="6">6</td>
        </tr>
        <tr>
            <td colspan="12">12</td>
        </tr>
        </tbody>
    </table>
```


	Container使用方式： .container下使用.row 创建列，然后重点来了：使用.col-x-x创建行，一个标签上可以使用多个设备类型的.col-x-x，那么这个标签可以同时支持多个设备的展示方式
	
### 测试窗口使用哪种网格
[测试页面使用哪种样式](http://www.runoob.com/bootstrap/bootstrap-responsive-utilities.html)


### 媒体查询，定义窗口大小
```
/* 超小设备（手机，小于 768px） */
@media (max-width: @screen-xs-max) { ... }
/* 小型设备（平板电脑，768px 起） */
@media (min-width: @screen-sm-min) and (max-width: @screen-sm-max) { ... }
/* 中型设备（台式电脑，992px 起） */
@media (min-width: @screen-md-min) and (max-width: @screen-md-max) { ... }
/* 大型设备（大台式电脑，1200px 起） */
@media (min-width: @screen-lg-min) { ... }
```

## 标准书写格式
```
<div class="container">
   <div class="row">
      <div class="col-*-*"></div>
      <div class="col-*-*"></div>      
   </div>
   <div class="row">...</div>
</div>
<div class="container">....
```


## 偏移列

```
 <!--定义两种设备展示方式：一种是中型设备占6，一种是小型设备占2，还有一个向右偏移3个单位-->
        <div class="row">
            <div class="col-md-6 col-xs-2">6</div>
            <div class="col-md-6 col-xs-offset-3">6</div>
        </div>
```
```
 .col-x-offset-*.   X指的是设备类型。offset是偏移，原理是创建指定数量的空白的网格，达到偏移位置的效果。  
 例如： .col-md-offset-3通过左边网格的列上，向右增加三个空白的空格，那么这个样式的位置就是最后的位置
```

## 嵌套列
```
    <div class="container">
        <div class="row">
            <div class="col-md-3" style="background-color: #B18904;box-shadow: inset 1px -1px 1px #444, inset -1px 1px 1px #444;"><h1>第一列</h1></div>
            <div class="col-md-9" style="background-color: #B18904;box-shadow: inset 1px -1px 1px #444, inset -1px 1px 1px #444;">
                <h1>第一行第二列分为两个盒子</h1>
                <div class="row" style="background-color: #B18904;box-shadow: inset 1px -1px 1px #444, inset -1px 1px 1px #444;">
                    <div class="col-md-6" style="background-color: #B18904;box-shadow: inset 1px -1px 1px #444, inset -1px 1px 1px #444;">
                        <h1>第二行的第一行第一列</h1>
                    </div>
                    <div class="col-md-6" style="background-color: #B18904;box-shadow: inset 1px -1px 1px #444, inset -1px 1px 1px #444;">
                        <h1>第二行的第一行第二列</h1>
                    </div>
                </div>
            </div>
        </div>
    </div>
```
	先定义行row然后定义列col，col里边可以重新定义行row并进行重新分割当前的col里边的大小进行12等分进行分配
	
	
	## 偏移位置
	```
	<div class="container">
        <div class="row"
             style="background-color: #B18904;box-shadow: inset 1px -1px 1px #444, inset -1px 1px 1px #444;">
            <div class="col-md-3"
                 style="background-color: #B18904;box-shadow: inset 1px -1px 1px #444, inset -1px 1px 1px #444;">
                <h1>第一列</h1>
            </div>
            <div class="col-md-9"
                 style="background-color: #B18904;box-shadow: inset 1px -1px 1px #444, inset -1px 1px 1px #444;">
                <h1>第二列</h1>
            </div>
        </div>
        <br>
        <div class="row"
             style="background-color: #B18904;box-shadow: inset 1px -1px 1px #444, inset -1px 1px 1px #444;">
            <div class="col-md-3 col-md-push-9"
                 style="background-color: #B18904;box-shadow: inset 1px -1px 1px #444, inset -1px 1px 1px #444;">
                <h1>第一列</h1>
            </div>
            <div class="col-md-9 col-md-pull-3"
                 style="background-color: #B18904;box-shadow: inset 1px -1px 1px #444, inset -1px 1px 1px #444;">
                <h1>第二列</h1>
            </div>
        </div>

    </div>
	```

如上，col-xx-push-xx   向右推
col-xx-pull-xx   向左边拉

col-md-push-9  向右推9个方向
一般使用是逆序推，例如是39，那么push9，pull3，那么就会变成93了。适用于已经写好的页面，重新改变左右布局