---
layout:     post
title:      "bootstrap-Alerts"
subtitle:   " \"bootstrap-Alerts\""
date:       2017-09-11 17:10:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端bootstrap
---

```
.alert-success、
.alert-info、
.alert-warning、
.alert-danger
.alert-dismissable 关闭的按钮
```


```

<div class="alert alert-success alert-dismissable">
	<button type="button" class="close" data-dismiss="alert"
			aria-hidden="true">
		&times;
	</button>
	<a class="alert-link" >
	成功！很好地完成了提交。
	</a>
</div>
<div class="alert alert-info alert-dismissable">
	<button type="button" class="close" data-dismiss="alert"
			aria-hidden="true">
		&times;
	</button>
	信息！请注意这个信息。
</div>
<div class="alert alert-warning alert-dismissable">
	<button type="button" class="close" data-dismiss="alert"
			aria-hidden="true">
		&times;
	</button>
	警告！请不要提交。
</div>
<div class="alert alert-danger alert-dismissable">
	<button type="button" class="close" data-dismiss="alert"
			aria-hidden="true">
		&times;
	</button>
	错误！请进行一些更改。
</div>
```
![](http://www.runoob.com/wp-content/uploads/2014/06/dismissalalert_demo.jpg)