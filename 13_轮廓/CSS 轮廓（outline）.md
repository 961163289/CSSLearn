## CSS 轮廓（outline）

轮廓（outline）是绘制于元素周围的一条线，位于边框边缘的外围，可起到突出元素的作用。

轮廓（outline）属性指定元素轮廓的样式、颜色和宽度。

### 轮廓（outline）实例

[在元素周围画线](https://www.runoob.com/try/try.php?filename=trycss_outline)
本例演示使用outline属性在元素周围画一条线。

[设置轮廓的样式](https://www.runoob.com/try/try.php?filename=trycss_outline-style)
本例演示如何设置轮廓的样式。

[设置轮廓的颜色](https://www.runoob.com/try/try.php?filename=trycss_outline-color)
本例演示如何设置轮廓的颜色。

[设置轮廓的宽度](https://www.runoob.com/try/try.php?filename=trycss_outline-width)
本例演示如何设置轮廓的宽度。

### CSS 轮廓（outline）

轮廓（outline）是绘制于元素周围的一条线，位于边框边缘的外围，可起到突出元素的作用。

CSS outline 属性规定元素轮廓的样式、颜色和宽度。

<img src="D:\WebLearn\CSSLearn\resources\img\img10.png" style="zoom:80%;" >

### 所有CSS轮廓（outline）属性

“CSS”列中的数字表示哪个CSS版本定义了该属性（CSS1 或者 CSS2）

| 属性                                                         | 说明                           | 值                                                           | CSS  |
| :----------------------------------------------------------- | :----------------------------- | :----------------------------------------------------------- | :--- |
| [outline](https://www.runoob.com/cssref/pr-outline.html)     | 在一个声明中设置所有的轮廓属性 | outline-color <br/>outline-style <br/>outline-width <br/>inherit | 2    |
| [outline-color](https://www.runoob.com/cssref/pr-outline-color.html) | 设置轮廓的颜色                 | color-name<br/>hex-number <br/>rgb-number <br/>invert <br/>inherit | 2    |
| [outline-style](https://www.runoob.com/cssref/pr-outline-style.html) | 设置轮廓的样式                 | none <br/>dotted <br/>dashed <br/>solid <br/>double <br/>groove <br/>ridge <br/>inset <br/>outset <br/>inherit | 2    |
| [outline-width](https://www.runoob.com/cssref/pr-outline-width.html) | 设置轮廓的宽度                 | thin <br/>medium <br/>thick <br/>length <br/>inherit         | 2    |

**注意：**

1.outline是不占空间的，既不会增加额外的width或者height（这样不会导致浏览器渲染时出现reflow或是repaint）

2.outline有可能是非矩形的（火狐浏览器下）

