# 表单

    表单
      基本表单
      内联表单
      水平排列表单
    控件
      控件列表
        输入框
        文本域
        复选框和单选框
        下拉框
        帮助文本
      属性控制
      校验状态
      控件图标


## 表单

单独的表单控件会被设置了全局样式。

.form-control 类的 `<input>、<textarea> 和 <select>` 元素都将被默认设置宽度属性为 width: 100%;。

.form-group 类将label元素和表单控件包裹在一起可以获得最好的排列。

### 基本表单
```html
<form class="form">
  <div class="form-group">
    <label for="name">Name</label>
    <input type="text" class="form-control" id="name" placeholder="asushiye">
  </div>
  <div class="form-group">
    <label for="email">Email</label>
    <input type="email" class="form-control" id="email" placeholder="zhenyun.su@example.com">
  </div>
  <button type="submit" class="btn btn-default">Send invitation</button>
</form>
```

### 内联表单

```html
<form class="form-inline">
  <div class="form-group">
    <label for="name">Name</label>
    <input type="text" class="form-control" id="name" placeholder="asushiye">
  </div>
  <div class="form-group">
    <label for="email">Email</label>
    <input type="email" class="form-control" id="email" placeholder="zhenyun.su@example.com">
  </div>
  <button type="submit" class="btn btn-default">Send invitation</button>
</form>
```

### 水平排列表单

```html
<form class="form-horizontal">
  <div class="form-group">
    <label for="name">Name</label>
    <input type="text" class="form-control" id="name" placeholder="asushiye">
  </div>
  <div class="form-group">
    <label for="email">Email</label>
    <input type="email" class="form-control" id="email" placeholder="zhenyun.su@example.com">
  </div>
  <button type="submit" class="btn btn-default">Send invitation</button>
</form>
```

## 控件

### 控件列表

#### 输入框控件

text、password、datetime、datetime-local、date、month、time、week、number、email、url、search、tel 和 color

只有正确设置了 type 属性的输入控件才能被赋予正确的样式。

实例：`<input type="text" class="form-control" placeholder="Text input">`


#### 文本域

Textarea

支持多行文本的表单控件。可根据需要改变 rows 属性。

`<textarea class="form-control" rows="3"></textarea>`

#### 复选框和单选框

复选框（checkbox）用于选择列表中的一个或多个选项，而单选框（radio）用于从多个选项中只选择一个。

实例：
```html
<div class="checkbox">
  <label>
    <input type="checkbox" value="">
    Option one is this and that&mdash;be sure to include why it's great
  </label>
</div>
<div class="checkbox disabled">
  <label>
    <input type="checkbox" value="" disabled>
    Option two is disabled
  </label>
</div>

<div class="radio">
  <label>
    <input type="radio" name="optionsRadios" id="optionsRadios1" value="option1" checked>
    Option one is this and that&mdash;be sure to include why it's great
  </label>
</div>
<div class="radio">
  <label>
    <input type="radio" name="optionsRadios" id="optionsRadios2" value="option2">
    Option two can be something else and selecting it will deselect option one
  </label>
</div>
<div class="radio disabled">
  <label>
    <input type="radio" name="optionsRadios" id="optionsRadios3" value="option3" disabled>
    Option three is disabled
  </label>
</div>
```

内联演示
```html
<label class="checkbox-inline">
  <input type="checkbox" id="inlineCheckbox1" value="option1"> 1
</label>
<label class="checkbox-inline">
  <input type="checkbox" id="inlineCheckbox2" value="option2"> 2
</label>
<label class="checkbox-inline">
  <input type="checkbox" id="inlineCheckbox3" value="option3"> 3
</label>

<label class="radio-inline">
  <input type="radio" name="inlineRadioOptions" id="inlineRadio1" value="option1"> 1
</label>
<label class="radio-inline">
  <input type="radio" name="inlineRadioOptions" id="inlineRadio2" value="option2"> 2
</label>
<label class="radio-inline">
  <input type="radio" name="inlineRadioOptions" id="inlineRadio3" value="option3"> 3
</label>
```

#### 下拉列表
```html
<select class="form-control">
  <option>1</option>
  <option>2</option>
  <option>3</option>
</select>
```

#### 帮助文本

bootstrap为表单控件提供帮助文本样式

```html
<label class="sr-only" for="inputHelpBlock">Input with help text</label>
<input type="text" id="inputHelpBlock" class="form-control" aria-describedby="helpBlock">

<span id="helpBlock" class="help-block">A block of help textnew line and may extend beyond one line.</span>
```

### 控件特有属性

1. disabled 表示控件禁用
2. readonly 表示控件只读
3. checked 用户表示复选框或单选框已选择
4. multiple 用于下拉框显示多个选项

### 校验状态

Bootstrap 对表单控件的校验状态，如 error、warning 和 success 状态，都定义了样式。

使用时添加 .has-warning、.has-error 或 .has-success 类到这些控件的父元素即可

```html
<div class="form-group has-success">
  <label class="control-label" for="inputSuccess1">Input with success</label>
  <input type="text" class="form-control" id="inputSuccess1" aria-describedby="helpBlock2">
  <span id="helpBlock2" class="help-block">A block of help text that breaks onto a new line and may extend beyond one line.</span>
</div>
<div class="form-group has-warning">
  <label class="control-label" for="inputWarning1">Input with warning</label>
  <input type="text" class="form-control" id="inputWarning1">
</div>
<div class="form-group has-error">
  <label class="control-label" for="inputError1">Input with error</label>
  <input type="text" class="form-control" id="inputError1">
</div>
```

### 添加控件图标
