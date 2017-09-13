---
layout:     post
title:      "badges提醒微章"
subtitle:   " \"badges提醒微章\""
date:       2017-09-29 9:30:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端bootstrap
---

## <span class="badge"
```
<a href="#">Mailbox <span class="badge">50</span></a>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/badges_demo.jpg)


## 为导航添加 微章事件.
其实就是<span标签添加a标签
```
<h4>胶囊式导航中的激活状态</h4>
<ul class="nav nav-pills">
    <li class="active">
        <a href="#">首页
            <span class="badge">42</span>
        </a>
    </li>
    <li>
        <a href="#">简介</a>
    </li>
    <li>
        <a href="#">消息
            <span class="badge">3</span>
        </a>
    </li>
</ul>
<br>FC
<h4>列表导航中的激活状态</h4>
<ul class="nav nav-pills nav-stacked" style="max-width: 260px;">
    <li class="active">
        <a href="#">
            <span class="badge pull-right">42</span>首页</a>
        </li>
    <li>
        <a href="#">简介</a>
    </li>
    <li>
        <a href="#">
            <span class="badge pull-right">3</span>消息
        </a>
    </li>
</ul>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/badgesactivestate_demo.jpg)