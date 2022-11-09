# HTML

~~~markdown
HTML属于前端技术，主要是进行前端网页的开发，使用HTML开发出来的是一个静态页面。
~~~

## 一、HTML简介

~~~markdown
HTML俗称网页，只要我们打开浏览器访问一个网站，看到的所有内容都是HTML页面提供的（或者是与HTML技术相关的技术提供的）

HTML全称为HyperText Markup Language，译为超文本标记语言。所谓的超文本就是不仅仅只有文本内容，包括视频、图片、音频、链接等内容。所谓标记语言，简单来说就是元素构成。也就是说，HTML提供一系列的元素来构成一个页面中最基础的内容。
~~~

~~~markdown
# HTML 被称为超文本标记语言
	1. 超文本
			普通文件：huan.txt 只能显示字符，但是超文本可以
	2. 标记语言：
			不是编程语言：python、C、C艹、C艹艹
			编辑语言的基本元素称为标记或者标签。<html>???</html>
~~~

### 当你保存HTML文件时，你既可以使用.htm也可以使用.html文件后缀

~~~markdown
# 1. 使用浏览器来运行html文件
		- google Chrome浏览器
		- firefox 火狐浏览器
		- edge（win10）
		- IE 永远别用：用来下载其他的浏览器
# 2. 编写HTML文件的工具
		- 记事本（不要用）
		-Hbuilder-写前段的工具，很好用
		-sublimetxt-很好用
		-DW
		----------------真正的前端开发人员----------------
		WebStorm
~~~

## 二、第一张网页

一个页面有且只有一个根标签是html，元素一般包含头标签和尾标签

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>我是秦欢欢</title>
</head>
<body>
<input type="text"></input>
</body>
</html>
~~~

- HTML标签：由尖括号包围
- 成对出现：<p></p>，即开标签和闭标签
- 属性：定义在开标签中，如input标签中的type属性
- 注释：使用注释标签 <!--哈哈哈哈-->
- HTML文档在浏览器中被解释运行，展示的不是源码而是渲染后的效果
- 简写：开闭标签之间的内容直接就是标签体，如果标签体为空，则可以简写

~~~markdown
# 1. 标准的HTML文件的结构
	1. 需要有HTML的根标签<html>xxx</html>
	2. 在根标签内部包含了两个子标签 head和body
	3. head表示头部信息，主要用于对网页进行说明描述的，比如网页的标签、编码等
	4. body表示主题内容，主要用于展示给客户一些信息
# 2. 网页的标题
	head标签中的title标签，
	<title>这里写标题</title>
# 3. 刷新网页
	1. 点击地址栏左边的刷新按钮
	2. ctrl+r
	3. F5
	4. ctrl+F5，强制刷新---不加载缓存
# 4. 字符集：避免中文乱码
	<meta charset"utf-8">
# 5. 标签、标记、元素
	<html>
	<title>
# 6. 标签的分类：
	双标签：<html></html> 有结束
	单标签：<meta>
# 7. 所有的标签都可以添加属性
	<input type="text">
	<input qinhuanhuan="haokan">
# 8. HTML中的注释
	ctrl + /
	<!-- 被注释的内容 -->
# 9. 当运行html文件时，在页面中，并不会展示标签本身，显示的是标签的内容或者是标签所对应的样式
~~~

## 三、HTML的头部

<head>元素包含了当前HTML中的所有头部元素，在<head>内必须定义<title>元素，还可以定义<script>、<link>等等元素。

这些HTML的头部元素定义了当前也免得标题、编码、使用的脚本或者样式等信息



#### 1. title元素

规定标题

#### 2. meta元素

该元素提供了HTML页面的元数据(Metadata)，元数据是指存储数据的信息

通常用于设置页面的编码、描述、关键词、作者等信息

元素不会显示在页面中，但是会被浏览器解析

##### 2.1 定义网页内容的编码格式

~~~html
<meta charset="utf-8">
~~~

##### 2.2 定义HTML页面的描述

~~~markdown
<meta name="description" content="谁访问我，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁，我就拉黑谁"
~~~

##### 2.3 定义HTML页面的作者

~~~html
<mata name="author" content="xx">
~~~

~~~markdown
1. 目前在学习的过程中，head标签，只需要添加title和meta charset就行了，关键字，作者，描述可以不加
2. 后续学习，在head标签中，还有有两个标签，script和style
~~~

### 四、HTML主体

#### 1、 body元素

标签定义文档的主体

元素包含文档的所有内容（比如文本、超链接、图片、音视频、表格、列表）。body元素中的包含内容，用户是可以看到的。

一个HTML文件，只能存在一个body标签

#### 2、 HTML元素的基本构成

##### 2.1 元素类型

HTML是标记语言，所谓标记指的就是页面中的元素（元素也可以称为标签）。一个完整的HTML页面由许多不同的元素构成。

###### 闭合元素：必须包含开始元素和结束元素，如果没有结束元素就会产生意料之外的错误

~~~html
闭合元素
<title>Hello world</title>
<p>
    你好
</p>
~~~

###### 空元素：也可以叫做单元素，只需要开始元素，不需要结束元素

~~~html
<meta name="description" content="你好">
<br/>
~~~

###### HTML的属性

属性是设置在HTML的元素中的，用于为元素添加附加信息。属性一般都是定义在开始元素中，并且是以“名称/值”对出现

~~~html
<input type="text" value="默认的填充文字">

<input type="button" value="点我">
~~~

### 五、HTML文本

#### 1、 标题元素

HTML提供了6个标题元素，由大到小依次为<h1>到<h6>

~~~html
<h1>
  这是一级标题
</h1>
<h2>
  这是二级标题
</h2>
<h3>
  这是三级标题
</h3>
<h4>
  这是四级标题
</h4>
~~~

#### 2、段落

元素定义段落

浏览器会自动的在段落的前后加空行

# 图像与链接

### 1. 图像元素

#### 1.1 src属性

​	src属性（必须），表示引入图像的url地址

 ~~~html
 <img src="???">
 ~~~

图像的地址可以是本地地址，也可以是网络地址

~~~html
<img src="https://img1.baidu.com/it/u=661483414,812703350&fm=253&fmt=auto&app=138&f=JPEG?w=375&h=500">
~~~

#### 1.2 图像的大小

~~~Html
<img src="static/img/jio.jpg" height="800" width="1600">
~~~

#### 1.3 图像定位

align 属性用于设置图像显示的位置。

- left：水平方向居左
- right：水平方向居右
- top：垂直方向居上
- bottom：垂直方向居下
- middle：居中

~~~markdown
<img src="static/img/jio.jpg" height="200" width="200" align="right">
~~~

#### 1.4 alt属性

~~~html
<img src="static/img/jio.pg" height="200" width="200" align="right" alt="略略略">
~~~

### 2. 超链接

#### 2.1 用法

href属性（必需），表示制定跳转的url地址

~~~html
<a href="https://img1.baidu.com/it/u=661483414,812703350&fm=253&fmt=auto&app=138&f=JPEG?w=375&h=500">
    <img src="static/img/jio.jpg">
</a>
~~~

#### 2. 2 打开方式

元素target属性设置链接的打开方式

- _blank：在新窗口打开该链接
- _self：在当前窗口打开链接

~~~html
<a href="https://img1.baidu.com/it/u=661483414,812703350&fm=253&fmt=auto&app=138&f=JPEG?w=375&h=500" target="_blank">
    <img src="static/img/jio.jpg">
</a>
~~~

#### 2.3 锚点

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>
<a id="dingbu"></a>
<a id="ding">乔鼎</a><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>


<a href="#dingbu">返回顶部</a>
</body>
</html>
~~~

### 2.4 回到顶部的空链接

PASS



# CSS样式表

## 一、 概述

### 1. CSS是什么？

~~~markdown
层叠样式表，定制html元素的显示样式，美化页面，对于前端页面的搭建十分重要
~~~

### 2. 为什么要使用CSS？

~~~markdown
定义如何显示HTML的样式通常存在样式表中
把样式添加到HTML中，是为了解决将内容和表现分离的问题
1. 为了美化页面，给各个标签添加样式
2. 使用CSS可以让内容和表现分离
~~~

## 二、初识CSS

### 1. 第一个CSS样式

~~~css
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
  <style type="text/css">
    p{
      color: white;
      font-size: 30px;
      background-color: purple;
        width: 500px;
    }
  </style>
</head>
<body>

<p>糖葫芦真好吃！</p>
</body>
</html>
~~~

### 2. 如何插入样式表

当浏览器读到了一个样式表的时候，浏览器会根据样式表来格式化HTML文档。在HTML文档中插入样式表的方法有三种：、

- 外部样式表

~~~html
<link href="CSS/index.css" rel="stylesheet" type="text/css">
~~~

- 内部样式表(位于<head>标签内部)

~~~html
<style type="text/css">
    p{
      color: white;
      font-size: 30px;
      background-color: purple;
        width: 500px;
    }
</style>
~~~

- 内联样式

~~~markdown
<p style="color: blue;background-color: black;">糖葫芦真好吃！</p>
~~~

#### 样式表的优先级：内联>内部>外部

~~~markdown
1. 外部样式：新建一个.css文件，在head标签中使用link标签引入
2. 内部样式：在head标签中，加入一个style标签
3. 内联样式-行内样式：在开始标签中，直接加入style属性
~~~

### 3. 基本语法

CSS语法由三部分构成：选择器、属性和值

~~~markdown
body{background-color:red; }
~~~

#### 注意：多个样式之间要用;隔开（英文分号)

## 三、选择器的种类

### 1. 元素选择器

~~~html
p{
      color: white;
      font-size: 30px;
      background-color: purple;
        width: 500px;
}
# 使用元素选择器的时候，页面中的所有该元素都会被统一为一个样式
~~~

### 2. 类选择器

类选择器可以为标有特定的class属性的HTML元素指定特定的样式。可以用于区分不同的HTML元素。

类选择器使用“.”来定义

HTML：

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
    <link href="CSS/index.css" rel="stylesheet" type="text/css">
</head>
<body>

<p style="color: blue; background-color: black; ">糖葫芦真好吃！</p>
<p class="p1">但是不能天天吃！</p>
<p class="p2">但是不能天天天吃！</p>
<p class="p3">但是不能天天天天吃！</p>

</body>
</html>

~~~

CSS：

~~~css
.p1{
    background-color: green;
}
.p2{
    background-color: gray;
}
.p3{
    background-color: gold;
}
~~~

### 3. ID选择器

ID选择器可以为标有特定的id的HTML元素制定特定的样式

ID选择器以“#”来定义

HTML：

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
    <link href="CSS/index.css" rel="stylesheet" type="text/css">
</head>
<body>

<p style="color: blue; background-color: black; ">糖葫芦真好吃！</p>
<p id="one">但是不能天天吃！</p>
<p id="two">但是不能天天天吃！</p>
<p id="three">但是不能天天天天吃！</p>

</body>
</html>
~~~

CSS:

~~~css
#one{
    background-color: green;
}
#two{
    background-color: gray;
}
#three{
    background-color: gold;
}
~~~

~~~markdown
1. 类选择器：给某一类元素设置样式，作用的元素更多一些
2. id选择器给某一个元素设置样式，作用于一个元素
3. 类选择器class属性值可以重复，而id值不可以重复
注意：ID的属性值不能以数字开头
~~~

### 4. 派生选择器

派生选择器允许你根据文档的上下文关系来确定某个标签的样式。

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
  <link href="CSS/index.css" rel="stylesheet" type="text/css">
</head>
<body>
<div>
  <p>烦</p>
</div>
<p>更烦</p>
</body>
</html>
~~~

~~~css
div p{color: purple}
~~~

### 5. 选择器继承

HTML：

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
  <link href="CSS/index.css" rel="stylesheet" type="text/css">
</head>
<body>
  <div>
    <p>哈哈哈</p>
    <b>呵呵呵</b>
  </div>
</body>
</html>
~~~

CSS

~~~css
div{
    color: green;
}
~~~

### 6. 选择器联合使用

同时对多个元素设置同一个样式：

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
  <link href="CSS/index.css" rel="stylesheet" type="text/css">
</head>
<body>
<h1>哈哈</h1>
<h2>呵呵</h2>
<h3>嘿嘿</h3>
</body>
</html>
~~~

~~~css
h1,h2,h3{
    color: grey;
}
~~~

### 7. 伪类选择器

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
  <style>
    #txt:focus{
      background-color: red;
    }
    #btn:hover{
      background-color: red;
    }cv   
  </style>
</head>
<body>
<input type="text" id="txt">
<input type="button" value="按钮" id="btn">
</body>
</html>
~~~

# JavaScript

## 一、简介

~~~markdown
JavaScript是一种直译式脚本语言，是一种动态类型、弱类型、基于原型的语言。它的解释器统称为JavaScript引擎，为浏览器的一部分，广泛用于客户端的脚本语言，最早在HTML上使用，用来给HTML网页增加动态功能。
~~~

~~~markdown
1. JS是一个脚本型语言，解释型的语言
2. 可以使用浏览器直接来解释运行JS的代码
3. JavaScript和Java没有直接练习，蹭热度
~~~

JavaScript被数以百万级的网页用来改进设计、验证表单、检测浏览器、创建cookies、以及更多的应用

~~~markdown
1. 以前不使用JS的时候，有一个用户登录的操作，用户输入了用户名和密码，点击登录，把用户名和密码发送给服务器，服务器来验证用户名和密码是否正确。
	问题：不管用户输入的用户名是否规范，都会交给服务器。
2. 有了JS后，可以在将用户名和密码交给服务器之前，做一些验证（密码长度是否合法、格式是否符合要求）验证成功之后交给服务器，会缓解服务器压力。
~~~

## 二、第一个程序

### 1、 初识JavaScript

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
  <script type="text/javascript">
    // 警告弹窗，有阻塞
    alert("Hello world!")
    // 向开发者工具的console中输出日志
    console.log("战士的意志要象礁石一样坚定，战士的性格要象和风一样温柔。")
  </script>
</head>
<body>
</body>
</html>
~~~

- HTML的<scipt>标签用于把JavaScript代码插入到HTML中；
- script标签可以出现在head和body位置，一般常放在head中
- 也可以引入外部的JS文件<script src="http://www.baidu.com/static/js/xxxx.js"></script>

~~~markdown
其中在head中和在body中添加script标签的区别：
		在head中添加script，在页面显示之前就执行了这段代码
		在body中添加script，在页面显示之后执行这段代码
~~~

### 2. 注释

- 单行注释：//
- 多行注释：/* .... */

## 三、 变量和数据类型

### 1. 变量

JS是一个弱类型的语言，在定义变量的时候不需要指定类型，直接使用let关键字定义即可

~~~javascript
var a = 'abc';
var b = 'cde';
console.log(a+b);
~~~

### 2. 数据类型

~~~markdown
字符串(String)、数字(Number)、布尔(Boolean)、数组(Array)、对象(Object)、空(null)、未定义类型(Undefined)
~~~

#### 2.1 字符串

- 声明字符串

~~~javascript
var a = 'abc';
console.log(a);
~~~

- 大小写转换

~~~markdown
var lower = a.toLowerCase()
var upper = a.toUpperCase()
console.log(lower);
console.log(upper);
~~~

- 分割字符串

~~~markdown
var r = a.split(' ')
console.log(r[0])
console.log(r[1])
console.log(r[2])
~~~

#### 2.2 数字

JavaScript不区分整数类型和浮点类型

~~~javascript
var age = 18;
var price = 18.99;
console.log(typeof age);
console.log(typeof price); // =>number
~~~

#### 2.3 布尔类型

~~~javascript
var y = true;
console.log(typeof y)
~~~

#### 2.4 数组

~~~html
<script type="text/javascript">
  var arr = [1,2,3,4,5,6,7,8]
  for (var i=0;i<arr.length;i++){
    console.log(arr[i])
  }

  arr[8] = 9
  console.log(arr)

  arr.push(10)
  console.log(arr)
</script>
~~~

## 四、 Math对象

### 1. Math对象的属性

~~~markdown
1. E:返回常量e
2. ln2:返回2的自然对数
.......
.......
~~~

## 五、 运算符

- 算数运算符(+ - * / % )
- 比较运算符(> < >= <= != === ==)
- 逻辑运算符(&& || !)
- 赋值运算符(+=)

## 六、 流程控制

### 1、 条件语句

#### 1.1 if语句

~~~javascript
var a = 10;
var b = '10';
//  PEP8
if (a == b){
    console.log('哈哈哈');
}
~~~

#### 1.2 if-else语句

~~~javascript
var a = 10;
var b = '10';
//  PEP8
if (a === b) {
    console.log('哈哈哈');
} else {
    console.log('呵呵呵')
}
~~~

#### 1.3 else-if语句

~~~javascript
var a = 1;
if(a == 1){
    console.log('请登录');
}else if (a==2){
    console.log('请注册');
}else{
    console.log('拜拜');
}
~~~

#### 1.4 switch case语句(python中没有)

~~~javascript
var choose = 2;
switch (choose){
    case 1:console.log('哈哈哈');break;
    case 2:console.log('呵呵呵');break;
    case 3:console.log('哼哼哼');break;
}
~~~

### 2、 循环语句

#### 2.1 for语句

~~~javascript
for(var i = 0;i < 10;i++){
    for(var j = 0;j<10;j++){
        document.write(i*j);
    }
    document.write('\n');
}
~~~

#### 2.2 while语句

~~~javascript
var n=10;
while (n<=100){
    alert(n);
    n+=1;
}
~~~

~~~markdown
do……while和while的区别
1. while先判断循环条件，再执行循环体代码
2. do……while是无论如何都会先执行一次循环体，再判断条件
~~~

## 七、 函数

### 1、 基本语法

~~~markdown
fuction 方法名(形参1,形参2){
	…………
	return;
}
~~~

### 2、 匿名函数

~~~javascript
var fn = function (a){alert(a);}
fn(20);
~~~

## 八、 事件

### 1、 事件注册、绑定

~~~javascript
function click_fn() {
    console.log('电死我了！');
}
~~~

### 2、 可用事件

~~~markdown
自己品
~~~

### 3、 event对象

~~~javascript
<script type="text/javascript">
    function click_fn(a) {
    console.log(a);
    console.log(a.type);
    console.log(a.clientX);
    console.log(a.clientY);
    console.log(a.target);
    console.log(a.target.value);

}
</script>
~~~

### 4、 事件冒泡

~~~javascript
function click_btn(a) {
    console.log(a);
    console.log(a.type);
    console.log(a.clientX);
    console.log(a.clientY);
    console.log(a.target);
    console.log(a.target.value);
}
function click_div(a) {
    console.log('hhhhhhhhhhhhhhhhhhhhh');
}
// 一个标签触发事件以后，事件会向上传递给自己的父标签，然后父标签的父标签.....
// 当父元素和子元素都拥有同一个事件的时候(如：都拥有onclick)冒泡才会发生
~~~

# JQuery

## 一、 简介

### 1、 什么是JQuery

JavaScript框架，是一套工具库。简化了JavaScript的功能实现。可以使得开发者写更少的代码却做更多的事儿。-write less do more。

官网：[jQuery](https://jquery.com/)

~~~markdown
1. JQuery是一个js框架，是对js的进一步封装
2. 在js中获取一个标签
	document.getElementById("d1");
	在JQ
	$("#d1")
	上述的写法是JQ的一种语法，在底层实现上还是JS在实现
~~~

### 2、 JQuery的功能

- HTML元素选取
- HTML元素操作
- CSS操作
- HTML的事件函数
- JavaScript特效和动画
- HTML的DOM遍历和修改
- Ajax

### 3、 安装

有两个版本的JQ可供下载：

- Production Version-专业版本：用于实际的网站中，已经被精简和压缩 有min
- Development Version-用于测试和开发(代码未被压缩，是可读的代码) 没有min

~~~html
<head>
    <script src="jquery-3.6.1.min.js"></script>
</head>
~~~

### 4、 初识JQuery

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
    <script src="jquery-3.6.1.min.js"></script>
    <script type="text/javascript">
        function myclik() {
            $("#pid").hide(); //获取id为pid的标签，并且将其隐藏
        }
    </script>
</head>
<body>
<p id="pid">袁菲傻逼！</p>
<input type="button" name="hhh" value="点我改命" onclick="myclik()">
</body>
</html>
~~~

### 5、 JQuery选择器

JQ选择器基于元素的id、类、类型、属性、属性值进行HTML元素查找

JQ中所有的选择器都以doller符号开头:$()

#### 1、 基本选择器

##### 1.1 元素选择器

~~~html
$("h1").hide();
~~~

##### 1.2 #id选择器

~~~html
$("#yf").hide()
~~~

##### 1.3 .class选择器

~~~markdown
$(".yfc").css('color','red');
~~~

##### 1.4 全选择器

~~~html
$("*").css('color','purple');
~~~

#### 1.5 多选择器共用

~~~html
$("p.yfc2").css('color','purple');

$("p#yfc2").css('color','purple');

$("div p").css('color','purple');

$("h1,p").css('color','purple');
~~~

#### 1.6 JQuery对象和DOM对象的区别

DOM获取元素

~~~markdown
document.getElement.......    //返回DOM对象
~~~

JQuery获取元素

~~~markdown
$("选择器")       //返回JQuery对象
~~~

都是对一个或者多个标签的封装，都指向一个标签或者多个标签，只不过是支持的功能不一样，DOM对象和JQuery对象都有各自独特的方法。

~~~markdown
# JQuery对象和JS对象的区别：我对象说你真可爱，象不理我
1. $()获取的是JQ对象
2. document........获取的DOM对象

如果是JQ对象，操作标签的时候，需要使用JQ的语法
如果是DOM对象，操作标签的时候，需要使用原生的JS的DOM写法
~~~



- JQ对象与DOM对象的互相转换

  - DOM--->JQuery

    ~~~markdown
    var div = document.getElementById("div1");
    // console.log(div);
    var div_jq = $(div);
    console.log(div_jq);
    ~~~

  - JQuery--->DOM

    ~~~markdown
    var div = $("#div1");
    var div = div.get();
    console.log(div[0]);
    ~~~

    

## 二、 JQuery的事件

### 1. 事件注册的方式

- 基于标签：和之间JS中使用方式一致，JQ不干涉
- 基于编程：JQ提供了全新的API

~~~html
<script type="text/javascript">
    $(document).ready(function () {
    $("#btn_1").click(function (event) {
        console.log($(this).val()); //this为当前触发事件的标签的DOM对象
        console.log(this.value);
    })
})
</script>
~~~

- Ready事件

等价于onload的作用，用于保证代码的执行在页面加载完毕之后。

~~~html
$(document).ready(function(){.....})
$(function(){...})//简写
~~~

### 2. JQuery的事件函数

| 鼠标事件     | 键盘事件   | 表单事件 |
| ------------ | ---------- | -------- |
| click()      | keypress() | submit() |
| mouseover()  | keydown()  | change() |
| mousemove()  | keyup()    | focus()  |
| mouseout()   |            | blur()   |
| mouseenter() |            |          |
| toggle()     |            |          |
| hover()      |            |          |
|              |            |          |
|              |            |          |

~~~html
<script type="text/javascript">
    $(function(){
        $("#pid").hover(function(){
            this.style.backgroundColor="blue";   //mouseenter时触发
        },
                        function(){
            $(this).css({"background-color":"black"});//mouseout时触发
        },
                       )
    })
</script>
~~~

## 三、 JQuery DOM

JQ中提供了一系列与DOM相关的方法，这使得访问和操作元素和属性变得很容易

### 1. 获取内容

- text()-设置或者返回所选元素的文本内容
- html()-设置或返回所选元素的内容
- val()-设置或者返回表单的值

~~~html
<script type="text/javascript">
    $(function(){
        $("#pid").hover(function(){
            var a = $("#pid").text("段森浩！");
            console.log(a)
            // console.log(this.text)   //mouseenter时触发
        },
                        function(){
            $(this).css({"background-color":"black"});//mouseout时触发
        },
                       )
    })
</script>
~~~

### 2. 获取属性

JQ attr() 方法用于获取属性值

- attr("属性名")    获取属性名
- attr("属性名","属性值")  设置属性值
- attr({属性名1:属性值1,属性名2:属性值2........}) 一次设置多个属性值
- removeAttr("属性名") 删除标签的属性

### 3. 添加元素

- append() 在被选元素的最后一个位置插入内容
- prepend() 在被选元素的开头插入内容

- after() 在被选元素的后面插入内容
- before()  在被选元素的前面插入内容

### 4. 删除元素

- remove() 删除被选元素
- empty() 清空元素内容

~~~html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
    <script src="../static/JS/jquery-3.6.1.min.js"></script>
    <script type="text/javascript">
      $(function () {
        $("#btn").click(function () {
          // $("#duanduan").after("<p>我是季晨光，我喝多了，我要吐你枕套里！</p>")
          $("#duanduan3").remove()
          // $("#duanduan3").empty()
        })
      })
    </script>
</head>
<body>
<div id="div_1">
  <p id="duanduan1">我是段森浩1！</p>
  <p id="duanduan2">我是段森浩2！</p>
  <p id="duanduan3">我是段森浩3！</p>
  <p id="duanduan4">我是段森浩4！</p>
  <p id="duanduan5">我是段森浩5！</p>
  <p id="duanduan6">我是段森浩6！</p>

</div>
<input type="button" value="季晨光喝多了！" id="btn">
</body>
</html>
~~~

### 5. JQuery CSS类

- addClass() 向被选元素添加一个类
- removeClass() 向被选元素删除一个类

### 6. CSS()方法

- css("样式属性名") 获取样式的属性值
- css("样式属性名","样式属性值") 设置一个样式属性的值
- css({"样式属性名1":"样式属性值1","样式属性名2":"样式属性值2","样式属性名3":"样式属性值3",}) 设置多个样式的属性值

# 作业

~~~markdown
1. VMware
2. xshell类似的远程ftp工具
3. 服务器系统版本centos7 
~~~



















































































































