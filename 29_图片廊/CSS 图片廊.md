## CSS 图片廊

以下是使用CSS创建图片廊：

<img src="D:\Programs\Typora\img\img34.png" alt="img34" style="zoom:80%;" />

### 图片廊

以下是使用 CSS 创建图片廊：

```html
<div class="responsive">
  <div class="img">
    <a target="_blank" href="http://static.runoob.com/images/demo/demo1.jpg">
      <img src="http://static.runoob.com/images/demo/demo1.jpg" alt="图片文本描述" width="300" height="200">
    </a>
    <div class="desc">这里添加图片文本描述</div>
  </div>
</div>
 
<div class="responsive">
  <div class="img">
    <a target="_blank" href="http://static.runoob.com/images/demo/demo2.jpg">
      <img loading="lazy" src="http://static.runoob.com/images/demo/demo2.jpg" alt="图片文本描述" width="300" height="200">
    </a>
    <div class="desc">这里添加图片文本描述</div>
  </div>
</div>
 
<div class="responsive">
  <div class="img">
    <a target="_blank" href="http://static.runoob.com/images/demo/demo3.jpg">
      <img loading="lazy" src="http://static.runoob.com/images/demo/demo3.jpg" alt="图片文本描述" width="300" height="200">
    </a>
    <div class="desc">这里添加图片文本描述</div>
  </div>
</div>
 
<div class="responsive">
  <div class="img">
    <a target="_blank" href="http://static.runoob.com/images/demo/demo4.jpg">
      <img loading="lazy" src="http://static.runoob.com/images/demo/demo4.jpg" alt="图片文本描述" width="300" height="200">
    </a>
    <div class="desc">这里添加图片文本描述</div>
  </div>
</div>
```

### 更多实例

响应式图片廊

```html
<div class="responsive">
  <div class="img">
    <a target="_blank" href="img_fjords.jpg">
      <img loading="lazy" src="http://www.runoob.com/wp-content/uploads/2016/04/img_fjords.jpg" alt="Trolltunga Norway" width="300" height="200">
    </a>
    <div class="desc">这里添加图片文本描述</div>
  </div>
</div>
 
 
<div class="responsive">
  <div class="img">
    <a target="_blank" href="img_forest.jpg">
      <img loading="lazy" src="http://www.runoob.com/wp-content/uploads/2016/04/img_forest.jpg" alt="Forest" width="600" height="400">
    </a>
    <div class="desc">这里添加图片文本描述</div>
  </div>
</div>
 
<div class="responsive">
  <div class="img">
    <a target="_blank" href="img_lights.jpg">
      <img loading="lazy" src="http://www.runoob.com/wp-content/uploads/2016/04/img_lights.jpg" alt="Northern Lights" width="600" height="400">
    </a>
    <div class="desc">这里添加图片文本描述</div>
  </div>
</div>
 
<div class="responsive">
  <div class="img">
    <a target="_blank" href="img_mountains.jpg">
      <img loading="lazy" src="http://www.runoob.com/wp-content/uploads/2016/04/img_mountains.jpg" alt="Mountains" width="600" height="400">
    </a>
    <div class="desc">这里添加图片文本描述</div>
  </div>
</div>
 
<div class="clearfix"></div>
 
<div style="padding:6px;">
  
  <h4>重置浏览器大小查看效果</h4>
</div>
```

