## CSS <span style="color:#64854c">伪类(pseudo-classes)</span>

CSS伪类是用来添加一些选择器的特殊效果。

### 语法

伪类的语法:

```css
selector:pseudo-class {property:value;}
```

CSS类也可以使用伪类:

```css
selector.class:pseudo-class {property:value;}
```

### anchor伪类

在支持 CSS 的浏览器中，链接的不同状态都可以以不同的方式显示

```css
a:link {color:#FF0000;}    /* 未访问的链接 */
a:visited {color:#00FF00;} /* 已访问的链接 */
a:hover {color:#FF00FF;}   /* 鼠标划过链接 */
a:active {color:#0000FF;}  /* 已选中的链接 */
```

**注意：** 在CSS定义中，a:hover 必须被置于 a:link 和 a:visited 之后，才是有效的。

**注意：** 在 CSS 定义中，a:active 必须被置于 a:hover 之后，才是有效的。

**注意：**伪类的名称不区分大小写。

### 伪类和CSS类

伪类可以与 CSS 类配合使用：

```css
a.red:visited {color:#FF0000;}
 
<a class="red" href="css-syntax.html">CSS 语法</a>
```

如果在上面的例子的链接已被访问，它会显示为红色。

### css: first-child 伪类

您可以使用 :first-child 伪类来选择父元素的第一个子元素。

**注意：**在IE8的之前版本必须声明[<!DOCTYPE>](https://www.runoob.com/tags/tag-doctype.html)，这样 :first-child 才能生效。

### 匹配第一个 &lt;p&gt; 元素

在下面的例子中，选择器匹配作为任何元素的第一个子元素的 &lt;p&gt; 元素：

```css
p:first-child
{
    color:blue;
}
```

### 匹配所有 &lt;p&gt; 元素中的第一个 &lt;i&gt; 元素

在下面的例子中，选择相匹配的所有 &lt;p&gt; 元素的第一个 &lt;i&gt; 元素：

```css
p > i:first-child
{
    color:blue;
}
```

### 匹配所有作为第一个子元素的 &lt;p&gt; 元素中的所有 &lt;i&gt; 元素

在下面的例子中，选择器匹配所有作为元素的第一个子元素的 <p> 元素中的所有 <i> 元素：

```css
p:first-child i
{
    color:blue;
}
```

### CSS - :lang 伪类

:lang 伪类使你有能力为不同的语言定义特殊的规则

**注意：**IE8必须声明[<!DOCTYPE>](https://www.runoob.com/tags/tag-doctype.html)才能支持;lang伪类。

在下面的例子中，:lang 类为属性值为 no 的q元素定义引号的类型：

```css
q:lang(no) {quotes: "~" "~";}
```

### 更多实例

[为超链接添加不同样式](https://www.runoob.com/try/try.php?filename=trycss_link2)
这个例子演示了如何为超链接添加其他样式。

[使用 :focus](https://www.runoob.com/try/try.php?filename=trycss_link_focus)
这个例子演示了如何使用 :focus伪类。

### 所有CSS伪类/元素

| 选择器                                                       | 示例                  | 示例说明                                      |
| :----------------------------------------------------------- | :-------------------- | :-------------------------------------------- |
| [:checked](https://www.runoob.com/cssref/sel-checked.html)   | input:checked         | 选择所有选中的表单元素                        |
| [:disabled](https://www.runoob.com/css/cssref/sel-disabled.html) | input:disabled        | 选择所有禁用的表单元素                        |
| [:empty](https://www.runoob.com/cssref/sel-empty.html)       | p:empty               | 选择所有没有子元素的 p 元素                   |
| [:enabled](https://www.runoob.com/cssref/sel-enable.html)    | input:enabled         | 选择所有启用的表单元素                        |
| [:first-of-type](https://www.runoob.com/cssref/sel-first-of-type.html) | p:first-of-type       | 选择的每个 p 元素是其父元素的第一个 p 元素    |
| [:in-range](https://www.runoob.com/cssref/sel-in-range.html) | input:in-range        | 选择元素指定范围内的值                        |
| [:invalid](https://www.runoob.com/cssref/sel-invalid.html)   | input:invalid         | 选择所有无效的元素                            |
| [:last-child](https://www.runoob.com/cssref/sel-last-child.html) | p:last-child          | 选择所有p元素的最后一个子元素                 |
| [:last-of-type](https://www.runoob.com/cssref/sel-last-of-type.html) | p:last-of-type        | 选择每个p元素是其母元素的最后一个p元素        |
| [:not(selector)](https://www.runoob.com/cssref/sel-not.html) | :not(p)               | 选择所有p以外的元素                           |
| [:nth-child(n)](https://www.runoob.com/cssref/sel-nth-child.html) | p:nth-child(2)        | 选择所有 p 元素的父元素的第二个子元素         |
| [:nth-last-child(n)](https://www.runoob.com/cssref/sel-nth-last-child.html) | p:nth-last-child(2)   | 选择所有 p 元素倒数的第二个子元素             |
| [:nth-last-of-type(n)](https://www.runoob.com/cssref/sel-nth-last-of-type.html) | p:nth-last-of-type(2) | 选择所有 p 元素倒数的第二个为 p 的子元素      |
| [:nth-of-type(n)](https://www.runoob.com/cssref/sel-nth-of-type.html) | p:nth-of-type(2)      | 选择所有 p 元素第二个为 p 的子元素            |
| [:only-of-type](https://www.runoob.com/cssref/sel-only-of-type.html) | p:only-of-type        | 选择所有仅有一个子元素为 p 的元素             |
| [:only-child](https://www.runoob.com/cssref/sel-only-child.html) | p:only-child          | 选择所有仅有一个子元素的 p 元素               |
| [:optional](https://www.runoob.com/cssref/sel-optional.html) | input:optional        | 选择没有"required"的元素属性                  |
| [:out-of-range](https://www.runoob.com/cssref/sel-out-of-range.html) | input:out-of-range    | 选择指定范围以外的值的元素属性                |
| [:read-only](https://www.runoob.com/cssref/sel-read-only.html) | input:read-only       | 选择只读属性的元素属性                        |
| [:read-write](https://www.runoob.com/cssref/sel-read-write.html) | input:read-write      | 选择没有只读属性的元素属性                    |
| [:required](https://www.runoob.com/cssref/sel-required.html) | input:required        | 选择有"required"属性指定的元素属性            |
| [:root](https://www.runoob.com/cssref/sel-root.html)         | root                  | 选择文档的根元素                              |
| [:target](https://www.runoob.com/cssref/sel-target.html)     | #news:target          | 选择当前活动#news元素(点击URL包含锚的名字)    |
| [:valid](https://www.runoob.com/cssref/sel-valid.html)       | input:valid           | 选择所有有效值的属性                          |
| [:link](https://www.runoob.com/cssref/sel-link.html)         | a:link                | 选择所有未访问链接                            |
| [:visited](https://www.runoob.com/cssref/sel-visited.html)   | a:visited             | 选择所有访问过的链接                          |
| [:active](https://www.runoob.com/cssref/sel-active.html)     | a:active              | 选择正在活动链接                              |
| [:hover](https://www.runoob.com/cssref/sel-hover.html)       | a:hover               | 把鼠标放在链接上的状态                        |
| [:focus](https://www.runoob.com/cssref/sel-focus.html)       | input:focus           | 选择元素输入后具有焦点                        |
| [:first-letter](https://www.runoob.com/cssref/sel-firstletter.html) | p:first-letter        | 选择每个 p 元素的第一个字母                   |
| [:first-line](https://www.runoob.com/cssref/sel-firstline.html) | p:first-line          | 选择每个 p 元素的第一行                       |
| [:first-child](https://www.runoob.com/cssref/sel-firstchild.html) | p:first-child         | 选择器匹配属于任意元素的第一个子元素的 p 元素 |
| [:before](https://www.runoob.com/cssref/sel-before.html)     | p:before              | 在每个 p 元素之前插入内容                     |
| [:after](https://www.runoob.com/cssref/sel-after.html)       | p:after               | 在每个 p 元素之后插入内容                     |
| [:lang(*language*)](https://www.runoob.com/cssref/sel-lang.html) | p:lang(it)            | 为 p 元素的 lang 属性选择一个开始值           |

