# HTML5规则

#### 规则1：文档里不能出现废弃标签
```html
centent,font,s,strike,b,u,isindex,basefont,dir,applet（error）
```
#### 规则2：html标签
html标签是用于创建一个HTML文档，必须得包含head、body两个标签，如果没有就是错误的。

下面我们建立一个简单的HTML5的文档
```html
<html>
  <head>
    <meta charset="UTF-8">
    <title>文档标题</title>
  </head>
  <body>
  文档内容
  </body>
</html>
```
#### 规则3：head标签
head标签是HTML文档的头部，包含了meta标签、title标签，使用脚本，样式等标签

注：meta和title标签是必须的
```html
<head>
  <meta charset="UTF-8">
  <title>文档标题</title>
  <link href="css/style.css" rel="stylesheet">
  <script src="js/js.js"></script>
</head>
```
#### 规则4：meta标签
meta标签是定义关于HTML的元信息，它的必须属性是content
```html
<meta name="keywords" content="HTML5">
```
#### 规则5：link标签
link标签是链接外部资源的，必须属性是src、rel
```html
<link src="css/style.css" rel="stylesheet">
```
#### 规则6：script标签
script标签有两种写法

第一种是链接外部资源，下面写法是链接外部资源的
```html
<script src="js/js.js"></script>
```
第二种是在script标签里面直接js脚本代码
```html
<script>
document.write("Hello World!");
</script>
```
