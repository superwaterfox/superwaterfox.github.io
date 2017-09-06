---
layout:     post
title:      "bootstrap表单"
subtitle:   " \"bootstrap表单\""
date:       2017-09-05 18:06:00
author:     "Waterfox"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 前端
---

> “一站式，就缺前端 ”

## 垂直表单form

```
向父 <form> 元素添加 role="form"。
把标签和控件放在一个带有 class .form-group 的 <div> 中。这是获取最佳间距所必需的。
向所有的文本元素 <input>、<textarea> 和 <select> 添加 class ="form-control" 。 

<form role="form"           表单标记
	<div class="form-group"       表单渲染
    <p class="form-control-static"    静态文字渲染
		<input class="form-control"       动态输入渲染
```

	bs3-form  使用intellij的bootstrap插件就可以生成
	
	
	
```
<form class="form-horizontal" role="form">
  <div class="form-group">
    <label for="firstname" class="col-sm-2 control-label">名字</label>
    <div class="col-sm-10">
      <input type="text" class="form-control" id="firstname" placeholder="请输入名字">
    </div>
  </div>
  <div class="form-group">
    <label for="lastname" class="col-sm-2 control-label">姓</label>
    <div class="col-sm-10">
      <input type="text" class="form-control" id="lastname" placeholder="请输入姓">
    </div>
  </div>
  <div class="form-group">
    <div class="col-sm-offset-2 col-sm-10">
      <div class="checkbox">
        <label>
          <input type="checkbox">请记住我
        </label>
      </div>
    </div>
  </div>
  <div class="form-group">
    <div class="col-sm-offset-2 col-sm-10">
      <button type="submit" class="btn btn-default">登录</button>
    </div>
  </div>
</form>

```
## Input
	type支持text、password、datetime、datetime-local、date、month、time、week、number、email、url、search、tel 和 color


## Textarea文本框支持row显示的行数
```
<textarea class="form-control" rows="5"></textarea>
```
## Checkbox和Radio
	对一系列复选框和单选框使用 .checkbox-inline 或 .radio-inline class，控制它们显示在同一行上

## Select支持多选
```
<select multiple class="form-control">
```
	
## form使用 p标签form-control-static 展示文字
```
<form class="form-horizontal" role="form">
  <div class="form-group">
    <label class="col-sm-2 control-label">Email</label>
    <div class="col-sm-10">
      <p class="form-control-static">email@example.com</p>
    </div>
  </div>
  <div class="form-group">
    <label for="inputPassword" class="col-sm-2 control-label">密码</label>
    <div class="col-sm-10">
      <input type="password" class="form-control" id="inputPassword" placeholder="请输入密码">
    </div>
  </div>
</form>
```

## 使用<fieldset disabled 进行批量禁用所有的表单控件,单个用disbaled属性
```
<form class="form-horizontal" role="form">
  <div class="form-group">
    <label class="col-sm-2 control-label">聚焦</label>
    <div class="col-sm-10">
      <input class="form-control" id="focusedInput" type="text" value="该输入框获得焦点...">
    </div>
  </div>
  <div class="form-group">
    <label for="inputPassword" class="col-sm-2 control-label">禁用</label>
    <div class="col-sm-10">
      <input class="form-control" id="disabledInput" type="text" placeholder="该输入框禁止输入..." disabled>
    </div>
  </div>
  <fieldset disabled>
    <div class="form-group">
      <label for="disabledTextInput" class="col-sm-2 control-label">禁用输入（Fieldset disabled）</label>
      <div class="col-sm-10">
        <input type="text" id="disabledTextInput" class="form-control" placeholder="禁止输入">
      </div>
    </div>
    <div class="form-group">
      <label for="disabledSelect" class="col-sm-2 control-label">禁用选择菜单（Fieldset disabled）</label>
      <div class="col-sm-10">
        <select id="disabledSelect" class="form-control">
          <option>禁止选择</option>
        </select>
      </div>
    </div>
  </fieldset>
  <div class="form-group has-success">
    <label class="col-sm-2 control-label" for="inputSuccess">输入成功</label>
    <div class="col-sm-10">
      <input type="text" class="form-control" id="inputSuccess">
    </div>
  </div>
  <div class="form-group has-warning">
    <label class="col-sm-2 control-label" for="inputWarning">输入警告</label>
    <div class="col-sm-10">
      <input type="text" class="form-control" id="inputWarning">
    </div>
  </div>
  <div class="form-group has-error">
    <label class="col-sm-2 control-label" for="inputError">输入错误</label>
    <div class="col-sm-10">
      <input type="text" class="form-control" id="inputError">
    </div>
  </div>
</form>
```