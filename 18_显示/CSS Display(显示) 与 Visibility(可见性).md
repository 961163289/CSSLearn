## CSS Display(显示) 与 Visibility(可见性)

display属性设置一个元素应如何显示，visibility属性指定一个元素应可见还是隐藏。

<img src="D:\Desktop\Java\Web\CSS\CSSLearn\resources\img\img13.png" style="zoom:80%;" >

### 隐藏元素 - display:none或visibility:hidden

隐藏一个元素可以通过把display属性设置为"none"，或把visibility属性设置为"hidden"。但是请注意，这两种方法会产生不同的结果。

visibility:hidden可以隐藏某个元素，但隐藏的元素仍需占用与未隐藏之前一样的空间。也就是说，该元素虽然被隐藏了，但仍然会影响布局。

```css
h1.hidden {visibility:hidden;}
```

display:none可以隐藏某个元素，且隐藏的元素不会占用任何空间。也就是说，该元素不但被隐藏了，而且该元素原本占用的空间也会从页面布局中消失。

```css
h1.hidden {display:none;}
```

### CSS Display - 块和内联元素

块元素是一个元素，占用了全部宽度，在前后都是换行符。

块元素的例子：

- <h1>
- <p>
- <div>

内联元素只需要必要的宽度，不强制换行。

内联元素的例子：

- <span>
- <a>

### 如何改变一个元素显示

可以更改内联元素和块元素，反之亦然，可以使页面看起来是以一种特定的方式组合，并仍然遵循web标准。

下面的示例把列表项显示为内联元素：

```css
li {display:inline;}
```

下面的示例把span元素作为块元素：

```css
span {display:block;}
```

**注意：**变更元素的显示类型看该元素是如何显示，它是什么样的元素。例如：一个内联元素设置为display:block是不允许有它内部的嵌套块元素。

### 更多实例

[如何显示元素的内联元素。](https://www.runoob.com/try/try.php?filename=trycss_display)

这个例子演示了如何显示一个元素的内联元素。

[如何显示元素的块元素。](https://www.runoob.com/try/try.php?filename=trycss_display_block)

这个例子演示了如何显示一个元素的块元素。

[如何使用一个表的collapse属性。](https://www.runoob.com/try/try.php?filename=trycss_visibility_collapse)

这个例子演示了如何使用表的collapse属性。

### 笔记

**块级元素(block)特性：**

- 总是独占一行，表现为另起一行开始，而且其后的元素也必须另起一行显示;
- 宽度(width)、高度(height)、内边距(padding)和外边距(margin)都可控制;

**内联元素(inline)特性：**

- 和相邻的内联元素在同一行;
- 宽度(width)、高度(height)、内边距的top/bottom(padding-top/padding-bottom)和外边距的top/bottom(margin-top/margin-bottom)都不可改变，就是里面文字或图片的大小;

**块级元素主要有：**

-  address , blockquote , center , dir , div , dl , fieldset , form , h1 , h2 , h3 , h4 , h5 , h6 , hr , isindex , menu , noframes , noscript , ol , p , pre , table , ul , li

**内联元素主要有：**

- a , abbr , acronym , b , bdo , big , br , cite , code , dfn , em , font , i , img , input , kbd , label , q , s , samp , select , small , span , strike , strong , sub , sup ,textarea , tt , u , var

**可变元素(根据上下文关系确定该元素是块元素还是内联元素)：**

- applet ,button ,del ,iframe , ins ,map ,object , script

**CSS中块级、内联元素的应用：**

利用CSS我们可以摆脱上面表格里HTML标签归类的限制，自由地在不同标签/元素上应用我们需要的属性。

主要用的CSS样式有以下三个：

- display:block -- 显示为块级元素
- display:inline -- 显示为内联元素
- display:inline-block -- 显示为内联块元素，表现为同行显示并可修改宽高内外边距等属性

我们常将所有<li>元素加上display:inline-block样式，原本垂直的列表就可以水平显示了。

