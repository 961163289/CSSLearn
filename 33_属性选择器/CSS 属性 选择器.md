## CSS <span style="color:#64854c">属性 </span>选择器

### 具有特定属性的HTML元素样式

具有特定属性的HTML元素样式不仅仅是class和id。

**注意：**IE7和IE8需声明!DOCTYPE才支持属性选择器！IE6和更低的版本不支持属性选择器。

### 属性选择器

下面的例子是把包含标题（title）的所有元素变为蓝色：

```css
[title]
{
    color:blue;
}
```

### 属性和值选择器

下面的实例改变了标题title='runoob'元素的边框样式:

```css
[title=runoob]
{
    border:5px solid green;
}
```

### 属性和值的选择器 - 多值

下面是包含指定值的title属性的元素样式的例子，使用（~）分隔属性和值:

```css
[title~=hello] { color:blue; }
```

下面是包含指定值的lang属性的元素样式的例子，使用（|）分隔属性和值:

```css
[lang|=en] { color:blue; }
```

### 表单样式

属性选择器样式无需使用class或id的形式:

```css
input[type="text"]
{
    width:150px;
    display:block;
    margin-bottom:10px;
    background-color:yellow;
}
input[type="button"]
{
    width:120px;
    margin-left:35px;
    display:block;
}
```

## 笔记

### CSS 属性选择器 ~=, |=, ^=, $=, *= 的区别

**先上总结:**

**"value 是完整单词"** 类型的比较符号: **~=**, **|=**

**"拼接字符串**" 类型的比较符号: ***=**, **^=**, **$=**

**1.attribute 属性中包含 value:**　

[attribute~=value] 属性中包含独立的单词为 value，例如：

```
[title~=flower]  -->  <img src="/i/eg_tulip.jpg" title="tulip flower" />
```

[attribute*=value] 属性中做字符串拆分，只要能拆出来 value 这个词就行，例如：

```
[title*=flower]   -->  <img src="/i/eg_tulip.jpg" title="ffffflowerrrrrr" />
```

**2.attribute 属性以 value 开头:**

[attribute|=value] 属性中必须是完整且唯一的单词，或者以 **-** 分隔开：，例如：

```
[lang|=en]     -->  <p lang="en">  <p lang="en-us">
```

[

attribute^=value] 属性的前几个字母是 value 就可以，例如：

```
[lang^=en]    -->  <p lang="ennn">
```

**3.attribute 属性以 value 结尾:**

```
[attribute$=value] 属性的后几个字母是 value 就可以，例如：
a[src$=".pdf"]
```

> 更多内容参考：[CSS 选择器](https://www.runoob.com/cssref/css-selectors.html)


