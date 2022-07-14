### CSS <span style="color:#64854c">字体</span>

CSS字体属性定义字体，加粗，大小，文字样式。

### serif 和 sans-serif 字体之间的区别
<img src="https://www.runoob.com/images/serif.gif">

在计算机屏幕上，sans-serif 字体被认为是比serif字体容易阅读

### CSS 字形

在css中，有两种类型的字体系列名称：

* **通用字体系列** - 拥有相似外观的字体系统组合（如“Serif”或“Monospace”）
* **特定字体系列** - 一个特定的字体系列（如“Times”或“Courier”）

| Generic family | 子体系列                | 说明 |
| -------------- | ----------------------- | ---- |
| Serif          | <span style="font-family:Times New Roman">Times New Roman</span> <br/><span style="font-family:Georgia">Georgia</span> | Serif字体中字符在行的末端拥有额外的装饰 |
| Sans-serif     | <span style="font-family:Arial">Arial </span><br><span style="font-family:Verdana">Verdana</span> | "Sans"是指无 - 这些字体在末端没有额外的装饰 |
| Monospace | <span style="font-family:Courier New">Courier New</span> <br/><span style="font-family:Lucida Console">Lucida Console</span> | 所有的等宽字符具有相同的宽度 |

### 字体系列

font-family 属性设置文本的字体样式

font-family 属性应该设置几个字体名称作为一种"后备"机制，如果浏览器不支持第一种字体，他将尝试下一种字体。

**注意**: 如果字体系列的名称超过一个字，它必须用引号，如Font Family："宋体"。

多个字体系列是用一个逗号分隔指明：

```css
p{font-family:"Times New Roman", Times, serif;}
```

对于较常用的字体组合，看看我们的 [Web安全字体组合](https://www.runoob.com/cssref/css-websafe-fonts.html)。

### 字体样式

主要是用于指定斜体文字的字体样式属性。

这个属性有三个值：

* 正常 - 正常显示文本
* 斜体 - 以斜体字显示的文本
* 倾斜的文字 - 文字向一边倾斜（和斜体非常类似，但不太支持）

```css
p.normal {font-style:normal;}
p.italic {font-style:italic;}
p.oblique {font-style:oblique;}
```

### 字体大小

font-size 属性设置文本的大小。

能否管理文字的大小，在网页设计中是非常重要的。但是，你不能通过调整字体大小使段落看上去像标题，或者使标题看上去像段落。

请务必使用正确的HTML标签，就&lt;h1&gt; - &lt;h6&gt;表示标题和&lt;p&gt;表示段落：

字体大小的值可以是绝对或相对的大小。

绝对大小：

* 设置一个指定大小的文本
* 不允许用户在所有浏览器中改变文本大小
* 确定了输出的物理尺寸时绝对大小很有用

相对大小：

* 相对于周围的元素来设置大小
* 允许用户在浏览器中改变文字大小

如果你不指定一个字体的大小，默认大小和普通文本段落一样，是16像素（16px = 1em）

### 设置字体大小像素

设置文字的大小与像素，让您完全控制文字大小：

```css
h1 {font-size:40px;}
h2 {font-size:30px;}
p {font-size:14px;}
```

上面的例子可以在 Internet Explorer 9, Firefox, Chrome, Opera, 和 Safari 中通过缩放浏览器调整文本大小。

虽然可以通过浏览器的缩放工具调整文本大小，但是，这种调整是整个页面，而不仅仅是文本。

### 用em来设置字体大小

为了避免Internet Explorer 中无法调整文本的问题，许多开发者使用 em 单位代替像素。

em的尺寸单位由W3C建议。

1em和当前字体大小相等。在浏览器中默认的文字大小是16px。

因此，1em的默认大小是16px。可以通过下面这个公式将像素转换为em：**px/16=em**

```css
h1 {font-size:2.5em;} /* 40px/16=2.5em */
h2 {font-size:1.875em;} /* 30px/16=1.875em */
p {font-size:0.875em;} /* 14px/16=0.875em */
```

### 使用百分比和EM组合

在所有浏览器的解决方案中，设置 <body>元素的默认字体大小的是百分比：

```css
body {font-size:100%;}
h1 {font-size:2.5em;}
h2 {font-size:1.875em;}
p {font-size:0.875em;}
```

我们的代码非常有效。在所有浏览器中，可以显示相同的文本大小，并允许所有浏览器缩放文本的大小。

### 更多实例

[设置字体加粗](https://www.runoob.com/try/try.php?filename=trycss_font-weight)
这个例子演示了如何设置字体的加粗。

[可以设置字体的转变](https://www.runoob.com/try/try.php?filename=trycss_font-variant)
这个例子演示了如何设置字体的转变。

[在一个声明中的所有字体属性](https://www.runoob.com/try/try.php?filename=trycss_font)
本例演示如何使用简写属性将字体属性设置在一个声明之内。

### 所有CSS字体属性

| Property     | 描述                             |
| ------------ | -------------------------------- |
| font         | 在一个声明中设置所有的字体属性   |
| font-family  | 指定文本的字体系列               |
| font-size    | 指定文本的字体大小               |
| font-style   | 指定文本的字体样式               |
| font-variant | 以小型大写字体或正常字体显示文本 |
| font-weight  | 指定字体的粗细                   |


