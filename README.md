# HTML5规则

#### 规则1：文档里不能出现废弃标签
```html
<centent>, <font>,s,strike,b,u,isindex,basefont,dir,applet
```
#### 规则2：html标签里必须包含`<head>`、`<body>`两个标签

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

#### 规则3：head标签
head标签是HTML文档的头部，包含了meta标签、title标签，使用脚本，样式等标签。

注：meta和title标签是必须的。
```html
<head>
  <meta charset="UTF-8">
  <title>文档标题</title>
  <link href="css/style.css" rel="stylesheet">
  <script src="js/js.js"></script>
</head>
```
#### 规则4：meta标签
meta标签是定义关于HTML的元信息，它的必须属性是content。
```html
<meta name="keywords" content="HTML5">
```
#### 规则5：link标签
link标签是链接外部资源的，必须属性是src、rel。
```html
<link src="css/style.css" rel="stylesheet">
```
#### 规则6：script标签
script标签有两种写法

第一种是链接外部资源，下面写法是链接外部资源的。
```html
<script src="js/js.js"></script>
```
第二种是在script标签里面直接js脚本代码。
```html
<script>
document.write("Hello World!");
</script>
```
#### 规则7：body标签
body标签是HTML文档的主体标签，是HTMl文档必不可少的一个标签。
```html5
<body>
我是主体
</body>
```
#### 规则8：section标签
section标签是定位文档中的节，比如章节、页眉、页脚或文档中的其他部分，是HTML5中的新标签。
```html
<section>
  <h1>PRC</h1>
  <p>The People's Republic of China was born in 1949...</p>
</section>
```
#### 规则9：article标签
article标签是定义文章，是HTML5中的新标签。
```html
<article>
  <h1>标题</h1>
  <p>文章内容</p>
</article>
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
#### 规则12：main标签
main标签是定义网站页面里面主体内容的，是HTML5中的新标签。

注：一个HTML文档里面只能出现一个main标签，不能出现多个，不能包含header标签、footer标签、article标签，否则就是错误的。
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
