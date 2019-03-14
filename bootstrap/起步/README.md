# 起步

    HTML5结构
    视窗
    全局样式

Bootstrap使用Html5文档类型，屏幕自适应时以移动设备优先

## HTML5结构
bootstrap
```html
<!DOCTYPE html>
<html lang="zh-CN>
  ...
</html>
```

## 视窗

设置屏幕自适应，默认以移动设备优先
```html
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1">
</head>
```

若想在不同屏幕设备上保持原生应用，通过滚动屏幕来显示

可添加user-scalable=no 可以禁用其缩放（zooming）功能。

`<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">`

## 全局样式

Bootstrap 排版、链接样式设置了基本的全局样式。分别是：

1. 为 body 元素设置 background-color: #fff;
2. 使用 @font-family-base、@font-size-base 和 @line-height-base 变量作为排版的基本参数
3. 为所有链接设置了基本颜色 @link-color ，并且当链接处于 :hover 状态时才添加下划线

这些样式都能在 scaffolding.less 文件中找到对应的源码。
