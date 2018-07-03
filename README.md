# HTML5规则

#### 规则1：文档里不能出现废弃标签
```html
<centent>,<font>,<s>,<strike>,<b>,<u>,<isindex>,<basefont>,<dir>,<applet>
```
#### 规则2：`<html>`里必须包含`<head>`、`<body>`两个标签

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
```

#### 规则3：`<title>`内容不能为空

示例如下：

```html
<title>文档标题</title>
```

#### 规则4：charset属性是必须放到`<meta>`

示例如下：

```html
<meta charset="utf-8">
```

#### 规则5：`<link>`元素里必须属性是src、rel

示例如下：

```html
<link src="css/style.css" rel="stylesheet">
```

#### 规则6：`<script>`除里src属性外，不能有别的属性

示例如下：

```html
<script src="js/js.js"></script>
```

#### 规则7：所有标签、属性、属性值必须都是小写

示例如下：

```html
<html>
  <head>
    <meta charset="utf-8">
    <title>文档标题</title>
  </head>
  <body>
    <h1>我是第一个标题</h1>
    <p>我是第一个段落</p>
  </body>
</html>
```
#### 规则8：`<h1>`在HTML文档页面中只能出现一个，`<h2>～<h6>`是可以出现多个

示例如下：

```html
<body>
  <h1>标题1</h1>
  <h2>标题2</h2>
  <h2>标题2</h2>
</body>
```
#### 规则9：在HTML文档里面`<p>`内容不能为空

示例如下：

```html
<p>我是第一个段路</p>
<p>我是第二个段路</p>
```
#### 规则10：aside标签
aside标签是定义侧边栏，是HTML5中的新标签。
```html
<aside>主体内容之外的内容</aside>
```
#### 规则11：nav标签
nav定义导航链接的部分，是HTML5中的新标签。
```html
<nav>
  <a href="index.html">home</a>
  <a href="about.html">About</a>
</nav>
```
#### 规则12：一个HTML文档里面只能出现一个`<main>`，不能包含`<header>`、`<footer>`、`<article>`
```html
<body>
  <header>页眉</header>
  <main>
    <nav>
      <a href="index.html">home</a>
      <a href="about.html">About</a>
    </nav>
    <section>文档内容</section>
  </main>
  <footer>页尾</footer>
</body>
```
#### 规则13：header标签
header标签是定义文档的页脚，是HTML5中的新标签。
```html
<header>
  <nav>
    <a href="index.html">home</a>
    <a href="about.html">About</a>
  </nav>
</header>
```
#### 规则14：footer标签
footer标签是定义文档的页脚，是HTML5中的新标签。
```html
<footer>
  <p>页脚内容</p>
</footer>
```
#### 规则15：a标签
a标签定义是超链接，必须属性是href，可以链接本地文件、也可以链接外部资源，如果没有则是错误的。
```html
<a href="http://www.baidu.com"></a> 这是链接外部资源
<a href="index.html">home</a> 这是链接本地文件
```
#### 规则16：img标签
img标签是定义图像，必须属性是src、alt，src规定显示图片的URL，alt规定图像代替文本。
```html
<img src="login.img"> (error)
<img src="login.img" alt="登陆">
```
#### 规则17：input标签
input标签是定义输入控件，它必须属性type，可选属性value、name、placeholder、checked、disabled、autofocus等。
type 定义input元素的类型

value 定义input元素的值

name 定义input元素的名称

placeholder 用户填写输入文段的提示

checked 首次加载时被选中

disabled 禁用此元素

autofocus 首次加载自动获取焦点

type属性的值有：button、checkbox、file、hidden、image、password、radio、reset、submit、tel、email、date、month、week、time、number、rang、color、datetime-local、url、search、datetime、text

Button
```html
<input type="button" name="按钮" value="按钮">
```
Checkbox
```html
<input type="checkbox" name="复选框">
```
File
```html
<input type="file" name="文件上传">
```
Hidden
```html
<input type="hidden" name="隐藏">
```
Image
```html
<input type="image" name="图像" alt="图像">
```
Password
```html
<input type="password" name="密码" placeholder="请输入密码">
```
Radio
```html
<input type="radio" name="单选按钮" checked>
```
Reset
```html
<input type="reset" name="重置" disabled>
```
Submit
```html
<input type="submit" name="提交" value="提交">
```

Tel
```html
<input type="tel" name="电话" value="请输入电话">
```
Email
```html
<input type="email" name="邮箱" value="请输入邮箱">
```
Date
```html
<input type="date" name="日期">
```
Month
```html
<input type="month" name="月份">
```
Week
```html
<input type="week" name="周">
```
Time
```html
<input type="time" name="时间">
```
Number
```html
<input type="number" name="数字">
```
Rang
```html
<input type="rang" name="范围">
```
Color
```html
<input type="color" name="颜色">
```
datetime-local
```html
<input type="datetime-local" name="日期时间">
```
Url
```html
<input type="url" name="链接">
```
Search
```html
<input type="search" name="搜索">
```
datetime
```html
<input type="datetime" name="日期时间">
```
Texl
```html
<input type="text" name="文本" value="请输入文本信息" autofocus>
```
#### 规则18：p标签
p标签是定义段落
```html
<p>这是第一个段落</p>
```
#### 规则19：button标签
button标签是定义按钮，它的常用属性是type、value、name、autofocus、disabled

type属性的值分别有：button、submit、reset

Button
该按钮是可点击的按钮
```html
<button type=“button” value=“按钮”></button>
```
Submit
该按钮是可提交按钮
```html
<button type=“submit” value=“提交”></button>
```
Reset
该按钮是重置按钮（清除表单数据）
```html
<button type=“reset” value=“重置”></button>
```
#### 规则20：select标签
select标签是定义下拉列表，它里面必须得包含option标签，否则是错误的。
```html
<select>
    <option>选项1</option>
    <option>选项2</option>
    <option>选项3</option>
</select>
```
