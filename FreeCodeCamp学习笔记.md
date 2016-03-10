---
title: FreeCodeCamp学习笔记
date: 2016-2-19
categories: 技术
tags: [html,css,前端]
---

寒假将过，感觉不能荒废了，要找点事做，于是整理了一下这个。

额，先[介绍一下freecodecamp](http://weibo.com/p/1001593933059845084440?from=singleweibo&mod=recommand_article&sudaref=www.baidu.com)吧：
	
FreeCodeCamp 是一个基于 MEAN 架构的开源社区，它可以帮助人们学习编程以及构建他们的非盈利项目，内容以前端为主。

在GitHub上，FreeCodeCamp拥有超过5万Star， 而且还在持续增长之中，对于大多数项目而言，增加一个Star也不容易。2015年，在《软件开发时代》杂志(SD Times)总结的GitHub优秀项目中，FreeCodeCamp名列前十。目前，该社区有7159次代码提交和250个代码贡献者。

如此神奇的一个开源项目，到底有哪些优势呢？

1.学习编程技能，比如HTML5、CSS3、JavaScript、数据库、Git、Node.js、Angular.js和敏捷开发。

3.从事自由和开源项目。

5.获得实时帮助。

下面进入正题。

## HTML5 and CSS

### 1. Say Hello to HTML Elements 

```

<h1>Hello</h1>
```
### 2. Headline with the h2 Element 

添加一个h2元素：

```

<h1>Hello World</h1>
<h2>CatPhotoApp</h2>

```
### 3. Inform with the Paragraph Element

添加一个p元素：

```

<h1>Hello World</h1>
<h2>CatPhotoApp</h2>
<p>Hello Paragraph</p>
```
### 4. Uncomment HTML 

取消注释：

```

<!--
<h1>Hello World</h1>

<h2>CatPhotoApp</h2>

<p>Hello Paragraph</p>
-->
```
	去掉`<!--`和`-->`即可。

### 5. Comment out HTML 

注释h1和p：

```

<!--
<h1>Hello World</h1>
-->
<h2>CatPhotoApp</h2>
<!--
<p>Hello Paragraph</p>
-->
```
### 6. Fill in the Blank with Placeholder Text

把那段红色段落复制粘贴到p元素：

```

<p>Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>
```
### 7. Delete HTML Elements 

删除h1元素：

```

<h2>CatPhotoApp</h2>

<p>Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>
```
### 8. Change the Color of Text 

啊哈，进入CSS的部分了==
给h2上红色：

```

<h2 style="color: red">CatPhotoApp</h2>
```
### 9. Use CSS Selectors to Style Elements

这里删掉h2元素里的style，创建style元素，并为h2设置color属性为blue(然而例子中给的是red，还要自己修改一下- -！)

```
<style>
  h2 {color:blue;}
</style>
<h2>CatPhotoApp</h2>
```
### 10.	Use a CSS Class to Style an Element

给h2加个class属性，在style元素里吧h2换成.red-text，blue换成red：

```
<style>
  .red-text {
    color: red;
  }
</style>

<h2 class="red-text">CatPhotoApp</h2>`
```
### 11. Style Multiple Elements with a CSS Class 

给`<p>`加一个red-text的class属性

```
<style>
  .red-text {
    color: red;
  }
</style>
<p class="red-text">Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>

```
### 12. Change the Font Size of an Element 

设置字体大小font-size，没啥好说的

```
<style>
  p {
    font-size:16px;
  }
</style>
<p>Purr jump eat the grass rip the couch scratched sunbathe, shed everywhere rip the couch sleep in the sink fluffy fur catnip scratched.</p>

<p class="red-text">Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>
```
### 13. Set the Font Family of an Element 

设置字体font-family：

```
<style>

  p {
    font-size: 16px;
    font-family:Monospace;
  }
</style>
<p class="red-text">Kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>
<p>Purr jump eat the grass rip the couch scratched sunbathe, shed everywhere rip the couch sleep in the sink fluffy fur catnip scratched.</p>
```
### 14. Import a Google Font 

设置Lobster字体

```
<link href="http://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  h2 {
    font-family:Lobster;
  }
</style>

<h2 class="red-text">CatPhotoApp</h2>

```
### 15. Specify How Fonts Should Degrade 

设置字体降级,注释掉Google字体的请求，观察变化

```
<!--<link href="http://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">-->
<style>

  h2 {
    font-family: Lobster, Monospace;
  }

</style>

<h2 class="red-text">CatPhotoApp</h2>

```

### 16. Add Images to your Website 

添加图片：

```

<img src="https://bit.ly/fcc-relaxing-cat">

```
### 17. Size your Images

设置图片大小：

```

<style> 
  .smaller-image {
    width:100px;
  }
</style>


<img class="smaller-image" src="https://bit.ly/fcc-relaxing-cat">

```

### 18. Add Borders Around your Elements 

添加边线：

```

<style>
  .smaller-image {
    width: 100px;
  }
  .thick-green-border {
    border-color: green;
    border-width:10px;
    border-style:solid;
  }
</style>

<img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat">

```
### 19. Add Rounded Corners with a Border Radius

添加圆角border-radius：

```
<style>
  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius:10px;
  }

  .smaller-image {
    width: 100px;
  }
</style>
<img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat">

```

### 20. Make Circular Images with a Border Radius

制作圆形图片：

```

<style>
  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }
  .smaller-image {
    width: 100px;
  }
</style>
<img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat">

```
### 21. Link to External Pages with Anchor Elements

设置链接：

```
<a href="http://freecatphotoapp.com">cat photos</a>
```
### 22. Nest an Anchor Element within a Paragraph

使用嵌套：

```
<p>View more <a href="http://www.freecatphotoapp.com">cat photos</a></p>
```
### 23. Make Dead Links using the Hash Symbol

死链接：

```
<p>Click here for <a href="#">cat photos</a>.</p>
```
### 24. Turn an Image into a Link

把图片变成链接：

```
<a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat"></a>
```
### 25. Add Alt Text to an Image for Accessibility

给图片添加alt属性：

```
<a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back"></a>
```
### 26. Create a Bulleted Unordered List

创建子弹无序列表(中文是这样吗？好吧是项目符号无序列表),删除两个`<p>`，列表是三个cat喜欢的东西。

```
<ul>
  <li>milk</li>
  <li>cheese</li>
  <li>girl</li>
</ul>
```

### 27. Create an Ordered List

创建一个有序列表，内容是三个cat讨厌的东西:

```
<ol>
  <li>boy</li>
  <li>gays</li>
  <li>html</li>  
</ol>
```
### 28. Create a Text Field

创建一个文本字段：

```
<input type="text">
```

### 29. Add Placeholder Text to a Text Field

添加占位文本到一个文本字段:

```
<input type="text" placeholder="cat photo URL">
```

### 30. Create a Form Element

创建一个表单元素,嵌套input元素:

```
<form action="/submit-cat-photo"><input type="text" placeholder="cat photo URL"></form>
```

### 31. Add a Submit Button to a Form

为表单添加提交按钮：

```
<form action="/submit-cat-photo">
  <input type="text" placeholder="cat photo URL">
  <button type="submit">Submit</button>
</form>
```
### 32. Use HTML5 to Require a Field

使用HTML5需要一个字段(required):

```
<form action="/submit-cat-photo">
  <input type="text" placeholder="cat photo URL" required>
  <button type="submit">Submit</button>
</form>
```
### 33. Create a Set of Radio Buttons

设置单选框：

```
<label><input type="radio" name="indoor-outdoor"> indoor</label></br>
<label><input type="radio" name="indoor-outdoor"> outdoor</label>
```
### 34. Create a Set of Checkboxes

设置复选框：

```
<form action="/submit-cat-photo">
  <label><input type="radio" name="indoor-outdoor"> Indoor</label>
  <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
  <input type="text" placeholder="cat photo URL" required>
  <button type="submit">Submit</button>
  <label><input type="checkbox" name="personality"> Loving</label>
  <label><input type="checkbox" name="personality"> Loving</label>
  <label><input type="checkbox" name="personality"> Loving</label>
</form>
```
### 35. Check Radio Buttons and Checkboxes by Default

检查默认单选按钮和复选框(第一个单选和复选添加checked):

```
<label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
  <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
  <label><input type="checkbox" name="personality" checked> Loving</label>
```

### 36. Nest Many Elements within a Single Div Element

用简单的div元素嵌套一些元素：

```
<div>
<p>Things cats love:</p>
<ul>
  <li>cat nip</li>
  <li>laser pointers</li>
  <li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
  <li>flea treatment</li>
  <li>thunder</li>
  <li>other cats</li>
</ol>
</div>
```

### 37. Give a Background Color to a Div Element

为div元素设置背景色：

```
.gray-background{
    background-color:gray;
  }

<div class="gray-background">
```

### 38. Set the ID of an Element

为元素设置id：

```
<form id="cat-photo-form" action="/submit-cat-photo">
```

### 39. Use an ID Attribute to Style an Element

使用ID属性设计元素：

```
#cat-photo-form {
    background-color:green;
  }
```
### 40. Adjusting the Padding of an Element

设置内边距：

```
.green-box {
    background-color: green;
    padding: 20px;
  }
```
### 41. Adjust the Margin of an Element

设置内边距：

```
.green-box {
    background-color: green;
    padding: 20px;
    margin: 20px;
  }
```
### 43. Add a Negative Margin to an Element

设置负的外边距：

```
.green-box {
    background-color: green;
    padding: 20px;
    margin: -15px;
  }
```

### 44. 
