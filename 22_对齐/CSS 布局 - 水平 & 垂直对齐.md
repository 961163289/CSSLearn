## CSS 布局 - 水平 & 垂直对齐

<img src="D:\Programs\Typora\img\img17.png" alt="img17" style="zoom:80%;" />

### 元素居中对齐

要水平居中对齐一个元素(如 <div>), 可以使用 **margin: auto;**。

设置到元素的宽度将防止它溢出到容器的边缘。

元素通过指定宽度，并将两边的空外边距平均分配：

```css
.center {
    margin: auto;
    width: 50%;
    border: 3px solid green;
    padding: 10px;
}
```

**注意:** 如果没有设置 **width** 属性(或者设置 100%)，居中对齐将不起作用。

### 文本居中对齐

如果仅仅是为了文本在元素内居中对齐，可以使用 **text-align: center;**

![img18](D:\Programs\Typora\img\img18.png)

```css
.center {
    text-align: center;
    border: 3px solid green;
}
```

**提示:** 更多文本对齐实例，请参阅 [CSS 文本](https://www.runoob.com/css/css-text.html) 章节。

### 图片居中对齐

要让图片居中对齐, 可以使用 **margin: auto;** 并将它放到 **块** 元素中:

<img src="D:\Programs\Typora\img\img19.png" alt="img19" style="zoom:80%;" />

```css
img {
    display: block;
    margin: auto;
    width: 40%;
}
```

### 左右对齐 - 使用定位方式

![img20](D:\Programs\Typora\img\img20.png)

```css
.right {
    position: absolute;
    right: 0px;
    width: 300px;
    border: 3px solid #73AD21;
    padding: 10px;
}
```

注释：绝对定位元素会被从正常流中删除，并且能够交叠元素。

**提示:** 当使用 **position** 来对齐元素时, 通常 **<body>** 元素会设置 **margin** 和 **padding** 。 这样可以避免在不同的浏览器中出现可见的差异。

当使用 position 属性时，IE8 以及更早的版本存在一个问题。如果容器元素（在我们的案例中是 <div class="container">）设置了指定的宽度，并且省略了 !DOCTYPE 声明，那么 IE8 以及更早的版本会在右侧增加 17px 的外边距。这似乎是为滚动条预留的空间。当使用 position 属性时，请始终设置 !DOCTYPE 声明：

```css
body {
    margin: 0;
    padding: 0;
}
 
.container {
    position: relative;
    width: 100%;
}
 
.right {
    position: absolute;
    right: 0px;
    width: 300px;
    background-color: #b0e0e6;
}
```

### 左右对齐 - 使用 float 方式

我们也可以使用 **float** 属性来对齐元素:

```css
.right {
    float: right;
    width: 300px;
    border: 3px solid #73AD21;
    padding: 10px;
}
```

当像这样对齐元素时，对 <body> 元素的外边距和内边距进行预定义是一个好主意。这样可以避免在不同的浏览器中出现可见的差异。

*注意：如果子元素的高度大于父元素，且子元素设置了浮动，那么子元素将溢出，这时候你可以使用 "**clearfix**(清除浮动)" 来解决该问题。*

我们可以在父元素上添加 overflow: auto; 来解决子元素溢出的问题:

```css
.clearfix {
    overflow: auto;
}
```

当使用 float 属性时，IE8 以及更早的版本存在一个问题。如果省略 !DOCTYPE 声明，那么 IE8 以及更早的版本会在右侧增加 17px 的外边距。这似乎是为滚动条预留的空间。当使用 float 属性时，请始终设置 !DOCTYPE 声明：

```css
body {
    margin: 0;
    padding: 0;
}
 
.right {
    float: right;
    width: 300px;
    background-color: #b0e0e6;
}
```

### 垂直居中对齐 - 使用 padding

CSS 中有很多方式可以实现垂直居中对齐。 一个简单的方式就是头部顶部使用 **padding**:

<img src="D:\Programs\Typora\img\img21.png" alt="img21" style="zoom:80%;" />

```css
.center {
    padding: 70px 0;
    border: 3px solid green;
}
```

如果要水平和垂直都居中，可以使用 **padding** 和 **text-align: center**:

<img src="D:\Programs\Typora\img\img22.png" alt="img22" style="zoom:80%;" />

```css
.center {
    padding: 70px 0;
    border: 3px solid green;
    text-align: center;
}
```

### 垂直居中 - 使用 line-height

<img src="D:\Programs\Typora\img\img23.png" alt="img23" style="zoom:80%;" />

```css
.center {
    line-height: 200px;
    height: 200px;
    border: 3px solid green;
    text-align: center;
}
 
/* 如果文本有多行，添加以下代码: */
.center p {
    line-height: 1.5;
    display: inline-block;
    vertical-align: middle;
}
```

### 垂直居中 - 使用 position 和 transform

除了使用 **padding** 和 **line-height** 属性外,我们还可以使用 **transform** 属性来设置垂直居中:

```css
.center { 
    height: 200px;
    position: relative;
    border: 3px solid green; 
}
 
.center p {
    margin: 0;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
```

**提示:** 更多 transform 属性内容可以参阅 [2D 翻转章节](https://www.runoob.com/css/css3-2dtransforms.html)。

### 更多实例

[CSS 使用 margin 让 div 居中对齐](https://c.runoob.com/codedemo/3360)

[CSS 使用绝对定位 让 div 右对齐](https://c.runoob.com/codedemo/3361)

### 笔记

设置容器上下 padding 相同实现垂直居中和使用 line-height=height 实现垂直居中仅对单行文本有效，当文本行数超过单行时：

-  1）**padding**：文本仍然处于容器垂直居中的位置，但是容器的 height 会随着文本行数的增加而增大；
-  2）**line-height=height**：容器的 height 不变，line-height 是文本的行间距，文本会溢出容器显示；

多行文本可使用 **vertical-align: middle;** 来实现元素的垂直居中，但是如果子元素的内容体积大于父元素的内容体积时，仍然会溢出，后面需要使用文字溢出处理来解决。
