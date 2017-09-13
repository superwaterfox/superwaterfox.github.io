---
layout:     post
title:      "bootstrap-pagination分页"
subtitle:   " \"bootstrap-pagination分页\""
date:       2017-09-08 17:10:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端bootstrap
---

## <ul class="pagination"
```
<ul class="pagination 
.pagination-lg  大些
.pagination-sm  小些


<Li .disabled    禁用
<Li .active      选中

<li .previous.  摆放到屏幕左侧
<li .next       摆放到屏幕右侧
```


## 默认三种大小的分页

```
<ul class="pagination pagination-lg">
<li><a href="#">&laquo;</a></li>
    <li><a href="#">1</a></li>
    <li><a href="#">2</a></li>
    <li><a href="#">3</a></li>
    <li><a href="#">4</a></li>
    <li><a href="#">5</a></li>
    <li><a href="#">&raquo;</a></li>
</ul><br>
<ul class="pagination">
    <li><a href="#">&laquo;</a></li>
    <li><a href="#">1</a></li>
    <li><a href="#">2</a></li>
    <li><a href="#">3</a></li>
    <li><a href="#">4</a></li>
    <li><a href="#">5</a></li>
    <li><a href="#">&raquo;</a></li>
</ul><br>
<ul class="pagination pagination-sm">
    <li><a href="#">&laquo;</a></li>
    <li><a href="#">1</a></li>
    <li><a href="#">2</a></li>
    <li><a href="#">3</a></li>
    <li><a href="#">4</a></li>
    <li><a href="#">5</a></li>
    <li><a href="#">&raquo;</a></li>
</ul>
```

![](http://www.runoob.com/wp-content/uploads/2014/06/paginationstate_demo.jpg)