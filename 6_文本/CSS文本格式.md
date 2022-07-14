### CSS文本格式

![image-20220711213440402](C:\Users\win11\AppData\Roaming\Typora\typora-user-images\image-20220711213440402.png)

### 文本颜色

颜色属性被用来设置文字的颜色。

颜色是通过CSS最经常的指定：

* 十六进制值 - 如: **＃FF0000**
* 一个RGB值 - 如: **RGB(255,0,0)**
* 颜色的名称 - 如: **red**

参阅 [CSS 颜色值](https://www.runoob.com/cssref/css-colors-legal.html) 查看完整的颜色值。

一个网页的背景颜色是指在主体内的选择：

```css
body {color:red;}
h1 {color:#00ff00;}
h2 {color:rgb(255,0,0);}
```

对于W3C标准的CSS：如果你定义了颜色属性，你还必须定义背景色属性。

### 文本的对齐方式

文本的排列属性是用来设置文本的水平对齐方式。

文本可居中对齐到左和右，两端对齐。

当 text-align 设置为 “justify”，每一行被展示为宽度相等，左，右外边距是对齐（如杂志和报纸）。

```css
h1 {text-align:center;}
p.date {text-align:right;}
p.main {text-align:justify;}
```

### 文本修饰

text-decoration 属性用来设置或删除文本的装饰。

从设计的角度来看 text-decoration 属性主要是用来删除链接的下划线：

```css
a {text-decoration:none;}
```

也可以这样修饰文件：

```css
h1 {text-decoration:overline;}
h2 {text-decoration:line-through;}
h3 {text-decoration:underline;}
```

我们不建议强调指出不是链接的文本，因为这常常混淆用户。

### 文本转换

文本转换属性是用来指定在一个文本中的大写和小写字母。

可用于所有字句变成大写或小写字母，或每个单词的首字母大写。

```css
p.uppercase {text-transform:uppercase;}
p.lowercase {text-transform:lowercase;}
p.capitalize {text-transform:capitalize;}
```

### 文本缩进

文本缩进属性是用来指定文本的第一行的缩进。

```css
p {text-indent:50px;}
```

### 更多实例

[指定字符之间的空间](https://www.runoob.com/try/try.php?filename=trycss_letter-spacing)
这个例子演示了如何增加或减少字符之间的空间。

```css
letter-spacing: 2px;
或
letter-spacing: -3px;
```

[指定行与行之间的空间](https://www.runoob.com/try/try.php?filename=trycss_line-height)
这个例子演示了如何指定在一个段落中行之间的空间

```css
line-height: 70%;
或
line-height: 200%;
```

[设置元素的文本方向](https://www.runoob.com/try/try.php?filename=trycss_text-direction)
这个例子演示了如何改变元素的文本方向。

```css
<style type="text/css">
	div.ex1 {direction:rtl;}
</style>
```

[增加单词之间的空白空间](https://www.runoob.com/try/try.php?filename=trycss_text-word-spacing)
这个例子演示了如何增加一个段落中的单词之间的空白空间。

```css
<style type="text/css">
	p {word-spacing: 30px;}
</style>
```

[在元素内禁用文字环绕](https://www.runoob.com/try/try.php?filename=trycss_text-white-space)
这个例子演示了如何禁用一个元素内的文字环绕。一行显示全部文本,不自动换行。

```css
p {white-space:nowrap;}
```

[垂直对齐图像](https://www.runoob.com/try/try.php?filename=trycss_vertical-align)
这个例子演示了如何设置文本的垂直对齐图像。

```css
<style>
    img.top {vertical-align:text-top;}
    img.bottom {vertical-align:text-bottom;}
</style>
```

[添加文本阴影](https://www.runoob.com/try/try.php?filename=trycss_text-shadow)
这个例子演示了如何设置文本阴影。

```css
<style>
	h1 {text-shadow:2px 2px #FF0000;}
</style>
```

### 所有CSS文本属性。

| 属性            | 描述                     |
| :-------------- | ------------------------ |
| color           | 设置文本颜色             |
| direction       | 设置文本方向             |
| letter-spacing  | 设置字符间距             |
| line-height     | 设置行高                 |
| text-align      | 对齐元素中的文本         |
| text-decoration | 向文本添加修饰           |
| text-indent     | 缩进元素中文本的首行     |
| text-shadow     | 设置文本阴影             |
| text-transform  | 控制元素中的字母         |
| unicode-bidi    | 设置或返回文本是否被重写 |
| vertical-align  | 设置元素的垂直对齐       |
| while-space     | 设置元素中空白的处理方式 |
| word-spacing    | 设置字间距               |