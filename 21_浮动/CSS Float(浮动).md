## CSS <span style="color:#64854c">Float(浮动)</span>

### 什么是 CSS Float（浮动）？

<img src="D:\Programs\Typora\img\img16.png" alt="img16" style="zoom:80%;" />

CSS 的 Float（浮动），会使元素向左或向右移动，其周围的元素也会重新排列。

Float（浮动），往往是用于图像，但它在布局时一样非常有用。

### 元素怎样浮动

元素的水平方向浮动，意味着元素只能左右移动而不能上下移动。

一个浮动元素会尽量向左或向右移动，直到它的外边缘碰到包含框或另一个浮动框的边框为止。

浮动元素之后的元素将围绕它。

浮动元素之前的元素将不会受到影响。

如果图像是右浮动，下面的文本流将环绕在它左边：

```css
img
{
    float:right;
}
```

### 彼此相邻的浮动元素

如果你把几个浮动的元素放到一起，如果有空间的话，它们将彼此相邻。

在这里，我们对图片廊使用 float 属性：

```css
.thumbnail 
{
    float:left;
    width:110px;
    height:90px;
    margin:5px;
}
```

### 清除浮动 - 使用 clear

元素浮动之后，周围的元素会重新排列，为了避免这种情况，使用 clear 属性。

clear 属性指定元素两侧不能出现浮动元素。

使用 clear 属性往文本中添加图片廊：

```css
.text_line
{
    clear:both;
}
```

### 更多实例

[为图像添加边框和边距并浮动到段落的右侧](https://www.runoob.com/try/try.php?filename=trycss_float2)

让我们为图像添加边框和边距并浮动到段落的右侧

[标题和图片向右侧浮动](https://www.runoob.com/try/try.php?filename=trycss_float3)

让标题和图片向右侧浮动。

[让段落的第一个字母浮动到左侧](https://www.runoob.com/try/try.php?filename=trycss_float4)

改变样式，让段落的第一个字母浮动到左侧。

[创建一个没有表格的网页](https://www.runoob.com/try/try.php?filename=trycss_float6)

使用 float 创建一个网页页眉、页脚、左边的内容和主要内容。

### CSS 中所有的浮动属性

"CSS" 列中的数字表示不同的 CSS 版本（CSS1 或 CSS2）定义了该属性。

| 属性                                                       | 描述                               | 值                                               | CSS  |
| :--------------------------------------------------------- | :--------------------------------- | :----------------------------------------------- | :--- |
| [clear](https://www.runoob.com/cssref/pr-class-clear.html) | 指定不允许元素周围有浮动元素。     | left <br/>right <br/>both <br/>none <br/>inherit | 1    |
| [float](https://www.runoob.com/cssref/pr-class-float.html) | 指定一个盒子（元素）是否可以浮动。 | left <br/>right <br/>none <br/>inherit           | 1    |

