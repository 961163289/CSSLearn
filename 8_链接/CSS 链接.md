### CSS 链接

不同的链接可以有不同的样式.

### 链接样式

链接的样式，可以使用任何CSS属性（如颜色，字体，背景等）。

特别的链接，可以有不同的样式，这取决于他们是什么状态。

这四个链接的状态是：

* a:link - 正常，未访问过的链接
* a:visited - 用户已访问过的链接
* a:hover - 当用户鼠标放在链接上时
* a:active - 链接被点击的那一刻

```css
a:link {color:#000000;}     /* 未访问链接*/
a:visited {color:#00FF00;}  /* 已访问链接 */
a:hover {color:#FF00FF;}  	/* 鼠标移动到链接上 */
a:active {color:#0000FF;}  	/* 鼠标点击时 */
```

当设置为若干链路状态的样式，也有一些顺序规则：

* a:hover 必须跟在 a:link 和 a:visited 后面
* a:active 必须跟在 a:hover 后面

### 常见的链接样式

根据上述链接的颜色变化的例子，看他是在说明状态。

让我们通过一些其他常见的方式转到链接样式：

### 文本修饰

text-decoration 属性主要用于删除链接中的下划线：

```css
a:link {text-decoration:none;}
a:visited {text-decoration:none;}
a:hover {text-decoration:underline;}
a:active {text-decoration:underline;}
```

### 背景颜色

背景颜色属性指定链接背景色：

```css
a:link {background-color:#B2FF99;}
a:visited {background-color:#FFFF85;}
a:hover {background-color:#FF704D;}
a:active {background-color:#FF704D;}
```

### 更多实例

[添加不同样式的超链接](https://www.runoob.com/try/try.php?filename=trycss_link2)
这个例子演示了如何为超链接添加其他样式。

[高级 - 创建链接框](https://www.runoob.com/try/try.php?filename=trycss_link_advanced)
这个例子演示了一个更高级的例子，我们结合若干CSS属性显示为方框。

### 链接样式的顺序记忆

```css
L(link)OV(visited)E  and  H(hover)A(active)TE
```

