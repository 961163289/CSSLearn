## CSS 导航栏

**垂直**

<img src="D:\Programs\Typora\img\img24.png" alt="img24" style="zoom:80%;" />

**水平**

<img src="D:\Programs\Typora\img\img25.png" alt="img25" style="zoom:80%;" />

### 导航栏

熟练使用导航栏，对于任何网站都非常重要。

使用CSS你可以转换成好看的导航栏而不是枯燥的HTML菜单。

### 导航栏=链接列表

作为标准的HTML基础一个导航栏是必须的。

在我们的例子中我们将建立一个标准的HTML列表导航栏。

导航条基本上是一个链接列表，所以使用 &lt;ul&gt; 和 &lt;li&gt; 元素非常有意义：

```html
<ul>
  <li><a href="#home">主页</a></li>
  <li><a href="#news">新闻</a></li>
  <li><a href="#contact">联系</a></li>
  <li><a href="#about">关于</a></li>
</ul>
```

现在，让我们从列表中删除边距和填充：

```css
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}
```

例子解析：

- list-style-type:none - 移除列表前小标志。一个导航栏并不需要列表标记
- 移除浏览器的默认设置将边距和填充设置为0

上面的例子中的代码是垂直和水平导航栏使用的标准代码。

### 垂直导航栏

上面的代码，我们只需要 &lt;a&gt; 元素的样式，建立一个垂直的导航栏：

```css
a
{
    display:block;
    width:60px;
}
```

示例说明：

- display:block - 显示块元素的链接，让整体变为可点击链接区域（不只是文本），它允许我们指定宽度
- width:60px - 块元素默认情况下是最大宽度。我们要指定一个60像素的宽度

**提示：**查看 [完整样式的垂直导航栏的示例](https://www.runoob.com/try/try.php?filename=trycss_navbar_vertical_advanced)。

**注意：** 请务必指定 &lt;a&gt; 元素在垂直导航栏的的宽度。如果省略宽度，IE6可能产生意想不到的效果。

### 垂直导航条实例

创建一个简单的垂直导航条实例，在鼠标移动到选项时，修改背景颜色：

<img src="D:\Programs\Typora\img\img26.png" alt="img26" style="zoom:80%;" />

```css
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    width: 200px;
    background-color: #f1f1f1;
}
 
li a {
    display: block;
    color: #000;
    padding: 8px 16px;
    text-decoration: none;
}
 
/* 鼠标移动到选项上修改背景颜色 */
li a:hover {
    background-color: #555;
    color: white;
}
```

### 激活/当前导航条实例

在点击了选项后，我们可以添加 "active" 类来标准哪个选项被选中：

<img src="D:\Programs\Typora\img\img27.png" alt="img27" style="zoom:80%;" />

```css
li a.active {
    background-color: #4CAF50;
    color: white;
}
```

## 创建链接并添加边框

可以在 &lt;li&gt; or &lt;a&gt; 上添加**text-align:center** 样式来让链接居中。

可以在 **border** &lt;ul&gt; 上添加 **border** 属性来让导航栏有边框。如果要在每个选项上添加边框，可以在每个 &lt;li&gt; 元素上添加**border-bottom** :

```css
ul {
    border: 1px solid #555;
}
 
li {
    text-align: center;
    border-bottom: 1px solid #555;
}
 
li:last-child {
    border-bottom: none;
}
```

### 全屏高度的固定导航条

接下来我们创建一个左边是全屏高度的固定导航条，右边是可滚动的内容。

```css
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    width: 25%;
    background-color: #f1f1f1;
    height: 100%; /* 全屏高度 */
    position: fixed; 
    overflow: auto; /* 如果导航栏选项多，允许滚动 */
}
```

**注意:** 该实例可以在移动设备上使用。

### 水平导航栏

有两种方法创建横向导航栏。使用**内联(inline)**或**浮动(float)**的列表项。

这两种方法都很好，但如果你想链接到具有相同的大小，你必须使用浮动的方法。

### 内联列表项

建立一个横向导航栏的方法之一是指定元素， 下述代码是标准的内联:

```css
li
{
    display:inline;
}
```

实例解析：

- display:inline; - 默认情况下，**<li>** 元素是块元素。在这里，我们删除换行符之前和之后每个列表项，以显示一行。

**提示:** 查看 [完整样式的水平导航栏的示例](https://www.runoob.com/try/try.php?filename=trycss_navbar_horizontal_advanced)。

### 浮动列表项

在上面的例子中链接有不同的宽度。

对于所有的链接宽度相等，浮动  &lt;li&gt; 元素，并指定为 &lt;a&gt; 元素的宽度：

```css
li
{
    float:left;
}
a
{
    display:block;
    width:60px;
}
```

实例解析：

- float:left - 使用浮动块元素的幻灯片彼此相邻
- display:block - 显示块元素的链接，让整体变为可点击链接区域（不只是文本），它允许我们指定宽度
- width:60px - 块元素默认情况下是最大宽度。我们要指定一个60像素的宽度

**提示:**查看 [完全样式的横向导航栏的示例](https://www.runoob.com/try/try.php?filename=trycss_navbar_horizontal_float_advanced)。

### 水平导航条实例

创建一个水平导航条，在鼠标移动到选项后修改背景颜色。

```css
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #333;
}
 
li {
    float: left;
}
 
li a {
    display: block;
    color: white;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
}
 
/*鼠标移动到选项上修改背景颜色 */
li a:hover {
    background-color: #111;
}
```

### 激活/当前导航条实例

在点击了选项后，我们可以添加 "active" 类来标准哪个选项被选中：

```css
.active {
    background-color: #4CAF50;
}
```

### 链接右对齐

将导航条最右边的选项设置右对齐 (float:right;)：

```css
<ul>
  <li><a href="#home">主页</a></li>
  <li><a href="#news">新闻</a></li>
  <li><a href="#contact">联系</a></li>
  <li style="float:right"><a class="active" href="#about">关于</a></li>
</ul>
```

### 添加分割线

&lt;li&gt; 通过 **border-right** 样式来添加分割线:

```css
/* 除了最后一个选项(last-child) 其他的都添加分割线 */
li {
    border-right: 1px solid #bbb;
}
 
li:last-child {
    border-right: none;
}
```

### 固定导航条

可以设置页面的导航条固定在头部或者底部：

**固定在头部**

```css
ul {
    position: fixed;
    top: 0;
    width: 100%;
}
```

**固定在底部**

```css
ul {
    position: fixed;
    bottom: 0;
    width: 100%;
}
```

**注意:** 该实例可以在移动设备上使用。

### 灰色水平导航条

```css
ul {
    border: 1px solid #e7e7e7;
    background-color: #f3f3f3;
}
 
li a {
    color: #666;
}
```

### 更多实例

- [响应式顶部导航 - 如何使用 CSS3 媒体查询来创建一个响应式导航。](https://c.runoob.com/codedemo/3513)
- [响应式边栏导航 - 如何使用 CSS3 媒体查询来创建一个边栏导航。](https://c.runoob.com/codedemo/3514)
- [导航下拉菜单 - 在导航条内部设置下拉菜单](https://c.runoob.com/codedemo/452)
- [导航图标 - 使用图标作为导航栏的选项](https://www.runoob.com/w3cnote/css-nav-bar.html)

