# 功用

    边框 - border
    大小 - sizing
    边界 - margin padding
    颜色 - color
    关闭图标 - close


## 边框 - border

使用边框样式来设置边框分格，可以应用按钮，图像，其他任何元素。

格式：`border-{position}-{value}`

```html
<span class="border"></span>
<span class="border-top"></span>
<span class="border-right"></span>
<span class="border-bottom"></span>
<span class="border-left"></span>

<span class="border-0"></span>
<span class="border-top-0"></span>
<span class="border-right-0"></span>
<span class="border-bottom-0"></span>
<span class="border-left-0"></span>

<span class="border border-primary"></span>
<span class="border border-secondary"></span>
<span class="border border-success"></span>
<span class="border border-danger"></span>
<span class="border border-warning"></span>
<span class="border border-info"></span>
<span class="border border-light"></span>
<span class="border border-dark"></span>
<span class="border border-white"></span>

<img src="..." alt="..." class="rounded">
<img src="..." alt="..." class="rounded-top">
<img src="..." alt="..." class="rounded-right">
<img src="..." alt="..." class="rounded-bottom">
<img src="..." alt="..." class="rounded-left">
<img src="..." alt="..." class="rounded-circle">
<img src="..." alt="..." class="rounded-0">
```

## 大小 - sizing

使用宽度和高度功用来设置元素的宽度和高度（相对父元素的宽度和高度）

```html
<div class="w-25 p-3" style="background-color: #eee;">Width 25%</div>
<div class="w-50 p-3" style="background-color: #eee;">Width 50%</div>
<div class="w-75 p-3" style="background-color: #eee;">Width 75%</div>
<div class="w-100 p-3" style="background-color: #eee;">Width 100%</div>

<div style="height: 100px; background-color: rgba(255,0,0,0.1);">
  <div class="h-25 d-inline-block" style="width: 120px; background-color: rgba(0,0,255,.1)">Height 25%</div>
  <div class="h-50 d-inline-block" style="width: 120px; background-color: rgba(0,0,255,.1)">Height 50%</div>
  <div class="h-75 d-inline-block" style="width: 120px; background-color: rgba(0,0,255,.1)">Height 75%</div>
  <div class="h-100 d-inline-block" style="width: 120px; background-color: rgba(0,0,255,.1)">Height 100%</div>
</div>
```

## 边界 - margin padding

通过外边界和内边界的功效来设置元素的外观

格式：`{property}{sides}-{size}`

```
{property}
m - for classes that set margin
p - for classes that set padding

{sides}
t - for classes that set margin-top or padding-top
b - for classes that set margin-bottom or padding-bottom
l - for classes that set margin-left or padding-left
r - for classes that set margin-right or padding-right
x - for classes that set both *-left and *-right
y - for classes that set both *-top and *-bottom

{size}
0 - for classes that eliminate the margin or padding by setting it to 0
1 - (by default) for classes that set the margin or padding to $spacer * .25
2 - (by default) for classes that set the margin or padding to $spacer * .5
3 - (by default) for classes that set the margin or padding to $spacer
4 - (by default) for classes that set the margin or padding to $spacer * 1.5
5 - (by default) for classes that set the margin or padding to $spacer * 3
auto - for classes that set the margin to auto
```

实例
```HTML

```

## 颜色 - color

```html
<p class="text-primary">.text-primary</p>
<p class="text-secondary">.text-secondary</p>
<p class="text-success">.text-success</p>
<p class="text-danger">.text-danger</p>
<p class="text-warning">.text-warning</p>
<p class="text-info">.text-info</p>
<p class="text-light bg-dark">.text-light</p>
<p class="text-dark">.text-dark</p>
<p class="text-muted">.text-muted</p>
<p class="text-white bg-dark">.text-white</p>

背景颜色

<div class="p-1 mb-2 bg-primary">.bg-primary</div>
<div class="p-1 mb-2 bg-secondary">.bg-secondary</div>
<div class="p-1 mb-2 bg-success">.bg-success</div>
<div class="p-1 mb-2 bg-danger">.bg-danger</div>
<div class="p-1 mb-2 bg-warning">.bg-warning</div>
<div class="p-1 mb-2 bg-info">.bg-info</div>
<div class="p-1 mb-2 bg-light">.bg-light</div>
<div class="p-1 mb-2 bg-dark">.bg-dark</div>
<div class="p-1 mb-2 bg-white">.bg-white</div>

```


## 关闭图标 - close

使用通用关闭图标来消除模态和警报等内容。

```html
<button type="button" class="close" aria-label="Close">
  <span aria-hidden="true">&times;</span>
</button>
```
