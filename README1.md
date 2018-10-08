# HTML5规则

<!-- ## 规则1：文档里不能出现废弃标签

```html
<center>,<font>,<s>,<strike>,<b>,<i>,<tt>,<small>,<frame>,<acronym>,<big>,<u>,<isindex>,<basefont>,<dir>,<applet>
``` -->

<!-- ## 规则2：`<html>`里必须包含`<head>`，`<body>`

示例如下：

```html
<html lang="zh-Hans">
  <head>
    <meta charset="utf-8">
    <title>文档标题</title>
  </head>
  <body>
  文档内容
  </body>
</html>
``` -->

<!-- ## 规则3：`<title>`内容不能为空

示例如下：

```html
<title>文档标题</title>
``` -->

## 规则4：必须包含`charset`属性的`<meta>`元素

示例如下：

```html
<meta charset="utf-8">
```

## 规则5：`<link>`元素必须属性是`src`、`rel`

示例如下：

```html
<link src="css/style.css" rel="stylesheet">
```

## 规则6：`<script>`只能有`src`属性

示例如下：

```html
<script src="js/js.js"></script>
```

## 规则7：标签必须小写

正确：

```html
<body>文档内容</body>
```

错误

```html
<BODY>文档内容</BODY>
```

## 规则8：属性名必须小写

正确：

```html
<body id="index">文档内容</body>
```

错误

```html
<body ID="index">文档内容</body>
```

## 规则9：属性值必须小写

正确：

```html
<body id="index">文档内容</body>
```

错误

```html
<body id="INDEX">文档内容</body>
```

## 规则10：`id`只能是唯一

正确：

```html
<body>
  <p id="index">文档内容</p>
  <p id="home">文档内容</p>
</body>
```

错误

```html
<body>
  <p id="index">文档内容</p>
  <p id="home">文档内容</p>
</body>
```

## 规则11：`<h1>`只能出现一次

正确：

```html
<body>
  <h1>标题1</h1>
  <h2>标题2</h2>
</body>
```

错误

```html
<body>
  <h1>标题1</h1>
  <h1>标题1</h1>
</body>
```

## 规则12：`<p>`内容不能为空

示例如下：

```html
<p>我是第一个段路</p>
<p>我是第二个段路</p>
```

## 规则13：`<aside>`不能包含`<main>`

正确：

```html
<html lang="zh-Hans">
  <head>
    <meta charset="utf-8">
    <title>文档标题</title>
  </head>
  <body>
    <aside>侧边栏内容</aside>
    <main>主体内容</main>
  </body>
</html>
```

错误：

```html
<html lang="zh-Hans">
  <head>
    <meta charset="utf-8">
    <title>文档标题</title>
  </head>
  <body>
    <aside>
      侧边栏内容
      <main>主体内容</main>
    </aside>
  </body>
</html>
```

## 规则14：`<nav>`不能包含`<main>`、`<header>`、`<footer>`

正确：

```html
<html lang="zh-Hans">
  <head>
    <meta charset="utf-8">
    <title>文档标题</title>
  </head>
  <body>
    <header>页眉</header>
    <nav>链接</nav>
    <main>主体内容</main>
    <footer>页尾</footer>
  </body>
</html>
```

错误：

```html
<html lang="zh-Hans">
  <head>
    <meta charset="utf-8">
    <title>文档标题</title>
  </head>
  <body>
    <header>页眉</header>
    <nav>
      <main>主体内容</main>
    </nav>
    <footer>页尾</footer>
  </body>
</html>
```

## 规则15：`<main>`不带`hidden`只能出现一次

正确：

```html
<body>
  <main>主体内容</main>
  <main hidden>主体内容</main>
</body>
```

或

```html
<body>
  <main>主体内容</main>
</body>
```

错误：

```html
<body>
  <main>主体内容</main>
  <main>主体内容</main>
</body>
```

## 规则16：`<header>`不能包含`<main>`、`<footer>`、`<aside>`

正确：

```html
<header>
  <nav>
    <a href="index.html">home</a>
    <a href="about.html">About</a>
  </nav>
</header>
```

错误：

```html
<header>
  <nav>
    <a href="index.html">home</a>
    <a href="about.html">About</a>
  </nav>
  <aside>侧边栏</aside>
  <main>内容</main>
  <footer>页脚</footer>
</header>
```

## 规则17：`<footer>`不能包含`<main>`、`<header>`、`<aside>`

正确：

```html
<footer>
  <p>页脚内容</p>
</footer>
```

错误：

```html
<footer>
  <header>页眉</header>
  <main>内容</main>
  <aside>侧边栏</aside>
</footer>
```

## 规则18：`<a>`必须包含属性`href`

正确：

```html
<a href="http://www.baidu.com">百度</a>
```

错误

```html
<a>百度</a>
```

## 规则19：`<img>`必须包含属性`src`、`alt`

正确：

```html
<img src="login.img" alt="登陆">
```

错误：

```html
<img src="login.img">
```

## 规则20：`<input>`必须包含属性`type`

正确：

```html
<input type="text" value="文本">
```

错误：

```html
<input name="文本">
```

## 规则21：`<select>`只能包含`<option>`

正确：

```html
<select>
    <option>选项1</option>
    <option>选项2</option>
    <option>选项3</option>
</select>
```

错误：

```html
<select>
  <p>选项1</p>
</select>
```

## 规则22：`<ul>`只能且必须包含`<li>`

正确：

```html
<ul>
  <li>列表1</li>
</ul>
```

错误：

```html
<ul>
</ul>
```

## 规则23：`<ol>`只能且必须包含`<li>`

正确：

```html
<ol>
  <li>列表1</li>
</ol>
```

错误：

```html
<ol>
</ol>
```

## 规则24：`<dl>`只能且必须包含`<dt>`、`<dd>`

正确：

```html
<dl>
  <dt>标题</dt>
  <dd>描述</dd>
</dl>
```

错误：

```html
<dl>
</dl>
```

## 规则25：`<iframe>`必须包含属性`src`

正确：

```html
<iframe src="URL" name="iframe_a"></iframe>
```

错误：

```html
<iframe name="iframe_a"></iframe>
```

## 规则26：`<details>`建议包含`<summary>`

示例如下：

```html
<details>
<summary>Copyright 2011.</summary>
<p>All pages and graphics on this web site are the property of W3School.</p>
</details>
```

## 规则27：`<embed>`必须包含属性`src`

正确：

```html
<embed src="helloworld.swf" width="200" height="200" />
```

错误：

```html
<embed width="200" height="200" />
```

## 规则28：`<video>`必须包含属性`controls`并且必须包含`<source>`和`<source>`的`src`属性

正确：

```html
<video src="/i/movie.ogg" controls="controls">
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
your browser does not support the video tag
</video>
```

错误：

```html
<video>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
your browser does not support the video tag
</video>
```

## 规则29：`<audio>`必须包含属性`controls`并且必须包含`<source>`和`<source>`的`src`属性

正确：

```html
<audio controls="controls">
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
```

错误：

```html
<audio>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
```

## 规则30：双标签必须闭合

正确：

```html
<p>hello</p>
```

错误：

```html
<p>hello
```

## 规则31：`<html>`必须包含属性`lang`

正确：

```html
<html lang="zh-Hans">
  <head>
    <meta charset="utf-8">
    <title>文档标题</title>
  </head>  
  <body>文档内容</body>
</html>
```

错误：

```html
<html >
   <head>
    <meta charset="utf-8">
    <title>文档标题</title>
  </head>  
  <body>文档内容</body>
</html>
```

## 规则32：所有元素里不能出现重复属性

正确：

```html
<p class="index">段落</p>
```

错误：

```html
<p class="index" class="index1">段落</p>
```

## 规则33：`<input>`的`type`的属性值为`radio`的时候必须包含`name`属性

正确：

```html
<input type="radio" name="sex">男
<input type="radio" name="sex">女
```

错误：

```html
<input type="radio">男
<input type="radio">女
```

## 规则34：`<input>`的`type`的属性值为`img`的时候必须包含`src`、`alt`属性

正确：

```html
<input type="img" src="logo.png" alt="logo">
```

错误：

```html
<input type="img" src="logo.png">
```

## 规则35：不能出现废弃属性

示例如下：

| 属性 | 所属的元素 |
| ---- | ---- |
| manifest | html |
| xmlns | html,title |
| align | caption, iframe, img, input, object, legend, table, hr, div, h1, h2, h3, h4, h5, h6, p, col, colgroup, tbody, td, tfoot, th, thead and tr |
| alink | body |
| link | body |
| vlink | body |
| text | body |
| background | body |
| bgcolor | table, tr, td, th and body |
| border | table and object, img|
| char | col, colgroup, tbody, td, tfoot, th, thead and tr |
| charoff | col, colgroup, tbody, td, tfoot, th, thead and tr |
| compact | dl , ol and ul |
| frame | table |
| frameborder | iframe |
| hspace | img and object |
| nowrap | td and th|
| rules | table |
| type | li, ol and ul |
| value | li |
| valign | col, colgroup, tbody, td, tfoot, th, thead and tr |
| width | hr, table, td, th, col, colgroup and pre |
| accept | form |
| vspace | img |
| charset | a, link |
| coords | a |
| name | a |
| rev | a, link |
| shape |
| target | link |
| height | th, td |

## 规则36：内联元素不能包含块元素

正确：

```html
<a href="http://www.baidu.com"><img src="logo.png" alit="百度"></a>
```

错误：

```html
<a href="http://www.baidu.com"><p>百度</p></a>
```

## 规则37：`<output>`必须包含属性`name`、`for`

正确：

```html
<form oninput="x.value=parseInt(a.value)+parseInt(b.value)">0
   <input type="range" id="a" value="50">100
   +<input type="number" id="b" value="50">
   =<output name="x" for="a b"></output>
</form>
```

错误：

```html
<form oninput="x.value=parseInt(a.value)+parseInt(b.value)">0
   <input type="range" id="a" value="50">100
   +<input type="number" id="b" value="50">
   =<output for="a b"></output>
</form>
```

## 规则38：`<meter>`必须包含属性`value`

正确：

```html
<meter value="0.6">60%</meter>
```

错误：

```html
<meter>60%</meter>
```

## 规则39：`<progress>`必须包含属性`value`

正确：

```html
<<progress value="0.9">90%</progress>
```

错误：

```html
<progress>90%</progress>
```
