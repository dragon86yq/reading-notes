### 什么是 HTML？
HTML是用来**描述**网页的一种语言。
-  HTML是超文本标记
-  HTML不是编程语言，而是一种语言标记
-  标记语言是一套标记标签
-  HTML使用**标记标签**来描述网页

#### HTML标签
- HTML标签是由尖括号包围的关键词，例如<html>
- HTML标签通常是成对出现，例如<b>和</b>
- 标签对中第一个标签是开始标签，第二个标签是结束标签


### HTML文档 = 网页
- HTML文档**描述网页**
- HTML文档**包含HTML标签和纯文本**
- HTML文档也被称为**网页**

#### HTML标签
-   HTML标题标签：<h1>-<h6>
-   例子：<h1>这是第一个主题</h1>
-   整个HTML文档标签：<html>
-   例子：<html>   </html>
-   HTML文档的主体标签：<body>
-   例子：<body>  </body>
-   HTML段落标签：<p>
    - 例子：<p>这是段落</p>
-   HTML链接标签：<a>
    - 例子：<a href = "http://www.w3school.com.cn">这是一个链接</a>
-   HTML图像标签：<img>
    - 例子：<img src="w3school.jpg" width="104" height="142" />

#### HTML元素语法
-   HTML元素以开始标签起始
-   HTML元素以结束标签终止
-   元素内容是在开始标签和结束标签之间的内容
-   大多数HTML元素拥有属性
-   大多数HTML源于可以嵌套
    -   例子：
        >  <html>
        >  <body>
        >  <p> 这是我的第一个HTML</p>
        >  </body>
        >  </html>

#### 元素定位
- 元素id属性
- 元素类属性
- 元素树状索引
- 标签遍历

#### HTML属性
- HTML标签可以拥有**属性**，属性可以提供HTML元素更多的信息
- 属性总是以**名称/值对**的形式出现，例如：name = "value"
- 属性总是在HTML元素的开始标签中规定。
- 属性值应该始终被包括在引号内。双引号最常用，也可以用单引号
- 适用于大多数HTML元素的属性：
  属性 ---------- 值 ------------------ 描述
  class      classname         规定元素的类名
  id                   id                 规定元素的唯一id
  style     style_definition  规定元素的行内样式
  title               text              规定元素的额外信息

#### HTML水平线
<hr/>标签在HTML页面中创建水平线，hr元素可用于分隔内容

#### HTML 注释
<!-- 这是一段注释。注释不会在浏览器中现实。-->

#### HTML段落
段落通过<p>标签定义。
在段落内换行使用<br/>


#### HTM文本格式化
##### 文本格式化标签
标签          描述
<b>          定义粗体文本
<big>       定义大号字
<em>       定义着重文字
<i>            定义斜体字
<small>   定义小号字
<strong> 定义加重语气
<sub>      定义下标字
<sup>      定义上标字
<ins>       定义插入字
<del>       定义删除字

##### 计算机输出标签
<code>      定义计算机代码
<kbd>        定义键盘码
<samp>     定义计算机代码样本
<tt>            定义打字机代码
<var>         定义变量
<pre>         定义预格式化文本

##### 引用和术语定义
<abbr>             定义缩写
<acronym>      定义首字母缩写
<address>       定义地址
<bdo>              定义文字方向
<blockquote>   定义长的引用
<q>                  定义短的引用
<cite>              定义引用、引证
<dfn>              定义一个定义项目

#### 样式
<style>           定义样式定义
<link>             定义资源引用
<div>              定义文档中的节或区域
<span>          定义文档中的行内的小块或区域

#### 实例
- HTML中的样式
```
<html>
<head>
<style type = "text/css">
h1 {color:red}
p {color:blue}
</style>
<body>
<h1> header 1</h1>
<p>A paragraph.</p>
</body>
</html>
```

#### HTML CCS
三种样式表：
- **外部样式表**：当样式被应用到多个页面时，使用外部样式表，修改一个文件就可以改变整个站点。
- **内部样式表**：当需要修改单个文件时，可以使用内部样式表
- **内联样式**：当特别的样式需要应用到个别元素时，可以使用内联样式。


#### HTML链接
**HTML超链接**：可以是一个字，一个词，或者一组词，也可以是一幅图像，可以点击这些内容来跳转到新的内容。可以使用<a>标签在HTML中创建链接。（a=anchor）
**两种使用<a>标签的方式**：
1. 通过使用href属性——创建指向另一个文档的链接。
2. 通过使用name属性——创建文档内的书签。

**HTML链接语法**：
> <a href = "url">Link test</a>
> href属性规定链接的目标，开始标签和结束标签之间的文字被作为超级链接显示。

**HTML链接——target属性**：
使用target属性可以定义被链接的文档在何处显示。
> <a href="http://www.w3school.com.cn/" target="_blank"> Visit W3School</a>

**HTML链接——name属性**：
- name属性规定anchor的名称。
- 使用name属性创建HTML页面中的书签，书签不会以任何特殊方式显示，它对读者是不可见的。
- 当使用命名锚（name anchors）时，我们可以创建直接跳至该命名锚的链接，这样使用者就不用不停的滚动鼠标寻找他们需要的信息。
- 使用id属性代替name属性，命名锚同样有效。
- **命名锚的语法**：
> <a name="lable">锚（显示在页面上的文本）</a>

```
首先进行锚命名（创建一个书签）：
> <a name="tips">基本的注意事项</a>
然后在同一个文档中创建指向该锚的链接：
> <a href="#tips">有用的提示</a>
也可以在其他页面中创建指向该锚的链接：
> <a href="http://www.w3school.com.cn/html/html_links.asp#tips">有用的提示</a>
```

#### HTML图像
**图像标签（<img>）和源属性（src）**：
- 在HTML中，图像由<img>标签定义
- <img>是空标签，只包含属性，没有闭合标签
- 要在页面中显示图像，需要使用源属性（src）。src指"source“。源属性的值是图像的URL地址
- 定义图像的语法：
> "<img src="url" />"

- 替换属性（Alt）：<img src="" alt="Big Boat">


#### HTML表格
- 表格由<table>标签定义。
- 每个表格均有若干行（由<tr>标签定义），每行被分割为若干单元格（由<td>标签定义）
- 字母td指表格数据（table data），即数据单元格的内容。数据单元格包含文本、图片、列表、段落、表单、水平线、表格等等。
- 表格的表头使用<th>标签定义
```
<table border="1">
<tr>
<th>Heading</th>
<th>Another Heading</th>
</tr>
<tr>
<td>row 1, cell 1</td>
<td>row 1, cell 1</td>
</tr>
<tr>
<td>row 2, cell 2</td>
<td>row 2, cell 2</td>
</tr>
</table>
```

#### HTML 列表
- HTML列表分为无序列表和有序列表
- 无序列表使用标签<ul>和<li>
> <ul>
> <li> Coffee</li>
> <li>Milk</li>
> </ul>
- 有序列表使用标签<ol>和<li>
> <ol>
> <li> Coffee</li>
> <li>Milk</li>
> </0l>

#### HTML <div>和<span>
- 大多数HTML元素被定义为块级元素和内联元素。
- 块级元素通常以新行开始：<h1>, <p>, <ul>, <table>
- 内联元素通常不会以新行开始：<b>, <td>, <a>, <img>
- <div>元素是块级元素，它能够用作其他HTML元素的容器，设置<div>元素的类，使我们能够为相同的<div>元素设置相同的类。
- <span>元素时内联元素。

#### HTML框架
- 通过使用框架，可以在同一个浏览器窗口中显示不止一个页面。
- 使用框架的坏处：
    - 开发人员必须同时跟踪更多的HTML文档
    - 很难打印整张页面
- 框架标签<frameset>，rows/columns规定每行或每列占据屏幕的面积


#### chrome开发者工具
- Element
     - 页面加载的文章文档信息
     - 所有的内容元素：样式、脚本、图像、音乐、文档内容等
     - 选择标签元素会显示完成的元素标签路径

- console
     - 查看页面加载过程中的消息，包括告警、错误及输出等
     - 执行自定义的js操作
     - 开发调试

- source
     - 页面文档所引用的资源

- network
     - 页面加载过程中所有涉及到的资源











