# HTML5规则

#### 规则1：文档里不能出现废弃标签（error）
```html
centent,font,s,strike,b,u,isindex,basefont,dir,applet
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


