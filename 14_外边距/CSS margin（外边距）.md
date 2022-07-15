## CSS <span style="color:#64854c">margin（外边距）</span>

CSS margin（外边距）属于定义元素周围的空间。

### margin

margin 清除周围（外边框）元素区域。margin 没有背景颜色，是完全透明的。

margin 可以单独改变元素的上，下，左，右边距，也可以一次改变所有的属性。

<img src="D:\WebLearn\CSSLearn\resources\img\img11.png" style="zoom:80%;" >

### 可能的值

| 值       | 说明                                        |
| :------- | :------------------------------------------ |
| auto     | 设置浏览器边距。 这样做的结果会依赖于浏览器 |
| *length* | 定义一个固定的margin（使用像素，pt，em等）  |
| *%*      | 定义一个使用百分比的边距                    |

Margin可以使用负值，重叠的内容。

### Margin - 单边外边距属性

在CSS中，它可以指定不同的侧面不同的边距：

```css
margin-top:100px;
margin-bottom:100px;
margin-right:50px;
margin-left:50px;
```

### Margin - 简写属性

为了缩短代码，有可能使用一个属性中margin指定所有的边距属性，这就是所谓的简写属性。

所有边距属性的简写属性是：**margin:**

```css
margin:100px 50px;
```

margin属性可以有一到四个值：

- **margin:25px 50px 75px 100px;**
  - 上边距为25px
  - 右边距为50px
  - 下边距为75px
  - 左边距为100px
- **margin:25px 50px 75px;**
  - 上边距为25px
  - 左右边距为50px
  - 下边距为75px
- **margin:25px 50px;**
  - 上下边距为25px
  - 左右边距为50px
- **margin:25px;**
  - 所有的4个边距都是25px

### 更多实例

[文本的上边距设置使用厘米值](https://www.runoob.com/try/try.php?filename=trycss_margin-top)
这个例子演示了如何设置一个使用厘米值的文本的顶部margin。

[Set 使用百分比值设置文本的下边距](https://www.runoob.com/try/try.php?filename=trycss_margin-bottom_percent)
这个例子演示了如何设置使用百分比值的下边距，相对于包含的元素的宽度。

### 所有的CSS边距属性

| 属性                                                         | 描述                                       |
| :----------------------------------------------------------- | :----------------------------------------- |
| [margin](https://www.runoob.com/cssref/pr-margin.html)       | 简写属性。在一个声明中设置所有外边距属性。 |
| [margin-bottom](https://www.runoob.com/cssref/pr-margin-bottom.html) | 设置元素的下外边距。                       |
| [margin-left](https://www.runoob.com/cssref/pr-margin-left.html) | 设置元素的左外边距。                       |
| [margin-right](https://www.runoob.com/cssref/pr-margin-right.html) | 设置元素的右外边距。                       |
| [margin-top](https://www.runoob.com/cssref/pr-margin-top.html) | 设置元素的上外边距。                       |

