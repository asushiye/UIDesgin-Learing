# 文本

## 全局设置

Bootstrap中variables.less 文件中定义的两个 Less 变量决定了排版尺寸：@font-size-base 和 @line-height-base。

第一个变量定义了全局 font-size 基准，第二个变量是 line-height 基准。

我们使用这些变量和一些简单的公式计算出其它所有页面元素的 margin、 padding 和 line-height


### 标题
HTML 中的所有标题标签，<h1> 到 <h6> 均可使用。

```HTML
<h1>h1. Bootstrap heading</h1>
<h2>h2. Bootstrap heading</h2>
```

### body

Bootstrap 将<body> 元素和所有段落<p>元素全局 字体大小font-size= 14px，行高line-height=1.428
段落间高度被设置了等于 1/2 行高（即 10px）的底部外边距（margin）。

 `.lead` 类可以让段落突出显示


## 内联文本

|名称|关键字|实例|
|-|-|-|
|标记|mark|tag to <mark>highlight</mark> text|
|插入|ins|tag to <ins>highlight</ins> text|
|删除|del|tag to <del>highlight</del> text|
|下划线|u|tag to <u>highlight</u> text|
|小号文本|samll|tag to <samll>highlight</samll> text|
|重点文本|strong|tag to <strong>highlight</strong> text|
|斜体文本|em|tag to <em>highlight</em> text|

## 对齐

通过文本对齐类，可以简单方便的将文字重新对齐。

```HTML
<p class="text-left">Left aligned text.</p>
<p class="text-center">Center aligned text.</p>
<p class="text-right">Right aligned text.</p>
<p class="text-justify">Justified text.</p>
<p class="text-nowrap">No wrap text.</p>
```

## 大小写

```HTML
<p class="text-lowercase">Lowercased text.</p>
<p class="text-uppercase">Uppercased text.</p>
<p class="text-capitalize">Capitalized text.</p>
```

## 缩略语
当鼠标悬停在缩写和缩写词上时就会显示完整内容

```html
<abbr title="attribute">attr</abbr>

<abbr title="HyperText Markup Language" class="initialism">HTML</abbr>
```
通过属性title 标识，通过.initialism 类美化


## 地址

```HTML
<address>
  <strong>Twitter, Inc.</strong><br>
  1355 Market Street, Suite 900<br>
  San Francisco, CA 94103<br>
  <abbr title="Phone">P:</abbr> (123) 456-7890
</address>

<address>
  <strong>Full Name</strong><br>
  <a href="mailto:#">first.last@example.com</a>
</address>
```

## 引用

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.

```html
<blockquote>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
</blockquote>


<blockquote>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer>Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>


<blockquote class="blockquote-reverse">
  ...
</blockquote>

```

## 列表

### 无序和有序列表
```HTML
<ul>
  <li>...</li>
</ul>

<ol>
  <li>...</li>
</ol>
```

内联列表

```HTML
<ul class="list-inline">
  <li>...</li>
</ul>
```

### 短语列表

```HTML
<dl>
  <dt>...</dt>
  <dd>...</dd>
</dl>

<dl class="dl-horizontal">
  <dt>...</dt>
  <dd>...</dd>
</dl>
```
