### CSS 背景
CSS 背景属性用于定义HTML元素的背景。

CSS 属性定义背景效果:
* background-color 
* background-image 
* background-repeat 
* background-attachment 
* background-position

### 背景颜色
background-color 属性定义了元素的背景颜色

页面的背景颜色使用在 body 选择器中:
```css
body {background-color:#b0c4de;}
```
CSS中，颜色值通常以以下方式定义:

* 十六进制 - 如："#ff0000"
* RGB - 如："rgb(255,0,0)"
* 颜色名称 - 如："red"

以下实例中, h1, p, 和 div 元素拥有不同的背景颜色:
```css
h1 {background-color:#6495ed;}
p {background-color:#e0ffff;}
div {background-color:#b0c4de;}
```
### 背景图像
background-image 属性描述了元素的背景图像.

默认情况下，背景图像进行平铺重复显示，以覆盖整个元素实体.

页面背景图片设置实例:

```css
body {background-image:url('paper.gif');}
```
### 背景图像 - 水平或垂直平铺
默认情况下 background-image 属性会在页面的水平或者垂直方向平铺。

一些图像如果在水平方向与垂直方向平铺，这样看起来很不协调，如下所示: 
```css
body
{
    background-image:url('gradient2.png');
}
```
如果图像只在水平方向平铺 (repeat-x), 页面背景会更好些:
```css
body
{
    background-image:url('gradient2.png');
    background-repeat:repeat-x;
}
```
### 背景图像- 设置定位与不平铺
Remark 让背景图像不影响文本的排版

如果你不想让图像平铺，你可以使用 background-repeat 属性:

```css
body
{
    background-image:url('img_tree.png');
    background-repeat:no-repeat;
}
```
以上实例中，背景图像与文本显示在同一个位置，为了让页面排版更加合理，不影响文本的阅读，我们可以改变图像的位置。

可以利用 background-position 属性改变图像在背景中的位置:
```css
body
{
    background-image:url('img_tree.png');
    background-repeat:no-repeat;
    background-position:right top;
}
```
### 背景-简写属性
在以上实例中我们可以看到页面的背景颜色通过了很多的属性来控制。

为了简化这些属性的代码，我们可以将这些属性合并在同一个属性中.

背景颜色的简写属性为 "background":
```css
body {background:#ffffff url('img_tree.png') no-repeat right top;}
```
当使用简写属性时，属性值的顺序为：:

1. background-color
2. background-image
3. background-repeat
4. background-attachment
5. background-position
以上属性无需全部使用，你可以按照页面的实际需要使用.
### 更多实例
如何设置固定的背景图像

本例演示如何设置固定的背景图像。图像不会随着页面的其他部分滚动。
```css
body {
    background-image: url("../resources/img/img5.png");
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-position: right top;
}
```
### CSS 背景属性

| Property              | 描述                     |
|:-----|:-----|
| background            | 简写属性，作用是将背景属性设置在一个声明中。 |
| background-attachment | 背景图像是否固定或者随着页面的其余部分滚动。 |
| background-color      | 设置元素的背景颜色。             |
| background-image      | 把图像设置为背景。              |
| background-position   | 设置背景图像的起始位置。           |
| background-repeat     | 设置背景图像是否及如何重复。         |
