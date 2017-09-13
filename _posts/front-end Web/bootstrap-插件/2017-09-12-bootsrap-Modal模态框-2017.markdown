---
layout:     post
title:      "bootstrap-well插图效果"
subtitle:   " \"bootstrap-well插图效果\""
date:       2017-09-11 17:40:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端bootstrap
---
使用a标签data-toggle和同级div[class="modal和id进行动作绑定
	<a data-toggle="modal" href="#modal-id"></a>  //添加事件绑定data-toggle和执行对象者的href
	
	<div class="modal fade" id="modal-id" tabindex="-1">  //.fade淡入淡出效果. tabindex=-1没有意义，但是可以给model添加默认的esc事件绑定 
			 <div class="modal-dialog"> //dialog类型绑定

```
 <a class="btn btn-primary" data-toggle="modal" href="#modal-id">Trigger modal</a>
    <div class="modal fade" id="modal-id" tabindex="-1">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <button type="button" class="close" data-dismiss="modal" aria-hidden="true">&times;</button>
                    <h4 class="modal-title">Modal title</h4>
                </div>
                <div class="modal-body">
                    Modal body ...
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
                    <button type="button" class="btn btn-primary">Save changes</button>
                </div>
            </div><!-- /.modal-content -->
        </div><!-- /.modal-dialog -->
    </div><!-- /.modal -->
```
    
```
.modal 用来把 <div> 的内容识别为模态框。
.fade  当模态框被切换时，它会引起内容淡入淡出。
aria-labelledby="myModalLabel"  标记属性引用模态框的标题。
aria-hidden="true" 默认true，默认隐藏，事件触发显示
<div class="modal-header">，modal-header 是为模态窗口的头部定义样式的类。
class="close"，close 是一个 CSS class，用于为模态窗口的关闭按钮设置样式。
data-dismiss="modal" 是一个自定义的 HTML5 data 属性。在这里它被用于关闭模态窗口。
class="modal-body"，是 Bootstrap CSS 的一个 CSS class，用于为模态窗口的主体设置样式。
class="modal-footer"，是 Bootstrap CSS 的一个 CSS class，用于为模态窗口的底部设置样式。
data-toggle="modal"，HTML5 自定义的 data 属性 data-toggle 用于打开模态窗口。
```


## 使用options参数 和 标签上绑定初始化事件（不推荐）
```
options参数    标签参数
backdrop   data-backdrop 默认值：true		遮罩层显示模态框，并且点击模态框外部就关闭
keyboard   data-keyboard 默认值：true		当按下 escape 键时关闭模态框，设置为 false 时则按键无效。
show       data-show     默认值：true		当初始化时显示模态框。
remote     data-remote	  默认值：false	使用 jQuery .load 方法，为模态框的主体注入内容。如果添加了一个带有有效 URL 的 href，则会加载其中的内容。如下面的实例所示：
<a data-toggle="modal" href="remote.html" data-target="#modal">请点击我</a>
```

## js与modal()原生事件，操作modal
```
Options: .modal(options)	 使用上述options参数作为初始化
$('#identifier').modal({
keyboard: false
})
Toggle: .modal('toggle')	手动切换模态框。	$('#identifier').modal('toggle')

Show: .modal('show')	手动打开模态框 $('#identifier').modal('show')
Hide: .modal('hide')	手动隐藏模态框 $('#identifier').modal('hide')
```

## bs.modal定制事件
```
show.bs.modal	在调用 show 方法后触发。	
$('#identifier').on('show.bs.modal', function () {
  // 执行一些动作...
})
shown.bs.modal	当模态框对用户可见时触发（将等待 CSS 过渡效果完成）。	
$('#identifier').on('shown.bs.modal', function () {
  // 执行一些动作...
})
hide.bs.modal	当调用 hide 实例方法时触发。	
$('#identifier').on('hide.bs.modal', function () {
  // 执行一些动作...
})
hidden.bs.modal	当模态框完全对用户隐藏时触发。	
$('#identifier').on('hidden.bs.modal', function () {
  // 执行一些动作...
})
```

