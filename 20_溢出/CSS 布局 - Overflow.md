## CSS 布局 - Overflow

CSS overflow 属性用于控制内容溢出元素框时显示的方式。

<img src="D:\Desktop\Java\Web\CSS\CSSLearn\resources\img\img14.png" style="zoom:80%;" >

### CSS Overflow

CSS overflow 属性可以控制内容溢出元素框时在对应的元素区间内添加滚动条。

overflow属性有以下值：

| 值      | 描述                                                     |
| :------ | :------------------------------------------------------- |
| visible | 默认值。内容不会被修剪，会呈现在元素框之外。             |
| hidden  | 内容会被修剪，并且其余内容是不可见的。                   |
| scroll  | 内容会被修剪，但是浏览器会显示滚动条以便查看其余的内容。 |
| auto    | 如果内容被修剪，则浏览器会显示滚动条以便查看其余的内容。 |
| inherit | 规定应该从父元素继承 overflow 属性的值。                 |

**注意:**overflow 属性只工作于指定高度的块元素上。

**注意:** 在 OS X Lion ( Mac 系统) 系统上，滚动条默认是隐藏的，使用的时候才会显示 (设置 "overflow:scroll" 也是一样的)。

### overflow: visible

默认情况下，overflow 的值为 visible， 意思是内容溢出元素框：

<img src="D:\Desktop\Java\Web\CSS\CSSLearn\resources\img\img15.png" style="zoom:80%;" >

```css
div {
    width: 200px;
    height: 50px;
    background-color: #eee;
    overflow: visible;
}
```

