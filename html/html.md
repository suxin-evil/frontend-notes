#  html

html的全称 **超文本标记语言** **(Hyper Text Markup Language)**。

##  文档结构

```html
<!DOCTYPE html> <!--文档类型，表明html的版本-->
<html lang="en"> <!--整个文档的根目录 lang代表文档的默认语言-->
    <head><!--头部标签-->
        <meta charset="UTF-8"><!--设置编码格式-->
        <title>Document</title><!--设置页面标题-->
    </head>
    <body>
        <!--主题内容-->
    </body>
</html>
```

##  html元素

* **开始标签(Opening tag)**包含元素的名称（本例为 p），被左、右角括号所包围。表示元素从这里开始或者开始起作用 
* **结束标签(Closing tag)**与开始标签相似，只是其在元素名之前包含了一个斜杠。这表示着元素的结尾
* **内容(content)**元素的内容，本例中就是所输入的文本本身。
* **元素**开始标签、结束标签与内容相结合，便是一个完整的元素。

##  元素属性

```html
<img src="" ><!--src属性为图片的地址-->
```

**属性应该包含：**

1. 在属性与元素名称（或上一个属性，如果有超过一个属性的话）之间的空格符。
2. 属性的名称，并接上一个等号。
3. 由引号所包围的属性值。

##  嵌套元素

也可以将一个元素置于其他元素之中 —— 称作**嵌套**。

```html
<p><strong>红</strong>色的气球</p>
```

必须保证元素嵌套次序正确：本例首先使用 [`<p>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/p) 标签，然后是 [`<strong>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/strong) 标签，因此要先结束 [`<p>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/strong) 标签，最后再结束 [`<strong>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/p) 标签。

##  空元素

不包含任何内容的元素称为空元素。比如 [`<img>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/img) 元素：

```html
<img src="./images/1.png" alt="加载失败">
```

本元素包含两个属性，但是并没有 `</img>` 结束标签，元素里也没有内容。这是因为图像元素不需要通过内容来产生效果，它的作用是向其所在的位置嵌入一个图像。

##  常用元素（标签）

### h1-h6标题标签

```html
		<h1>1</h1>
		<h2>2</h2>
		<h3>3</h3>
		<h4>4</h4>
		<h5>5</h5>
		<h6>6</h6>
```

###  段落标签

```html
<p>
    超文本标记语言（标准通用标记语言下的一个应用，外语缩写HTML），是迄今为止网络上应用最为广泛的语言，也是构成网页文档的主要语言。HTML文本是由HTML命令组成的描述性文本，HTML命令可以说明文字、图形、动画、声音、表格、链接等。HTML的结构包括头部（Head）、主体（Body）两大部分，其中头部描述浏览器所需的信息，而主体则包含所要说明的具体内容。
</p>
```

`<p>`标签定义段落

###  换行标签

```html
<!--文字换行-->
<p>
    超文本标记语言（标准通用标记语言下的一个应用，外语缩写HTML），<br>是迄今为止网络上应用最为广泛的语言。
</p>
<!--标签换行-->
<input type="text"/> <br> <input type="text" />
```

###  预格式化文本

```html
<pre>
	床前明月光，
	疑是地上霜。
	举头望明月，
	低头思故乡。
</pre>
```

###  水平分割线

```html
<pre>
	床前明月光，
	疑是地上霜。
	<hr>
	举头望明月，
	低头思故乡。
</pre>
```

###  字体加粗标签

```html
<p>
    <b>超文本标记语言</b>（标准通用标记语言下的一个应用，外语缩写HTML），是迄今为止网络上应用最为广泛的语言。
</p>
```

###  字体倾斜

**把文本定义为强调内容**

```html
<p>
    <em>超文本标记语言</em>（标准通用标记语言下的一个应用，外语缩写HTML），是迄今为止网络上应用最为广泛的语言。
</p>
```

###  强调内容

`<strong>`**把文本定义为语气更强的强调的内容。**

```html
<p>
    <strong>超文本标记语言</strong>（标准通用标记语言下的一个应用，外语缩写HTML），是迄今为止网络上应用最为广泛的语言。
</p>
```

###  字体小号

`<small>`**标签呈现小号字体效果。**

```html
<p>
    <small>超文本标记语言</small>（标准通用标记语言下的一个应用，外语缩写HTML），是迄今为止网络上应用最为广泛的语言。
</p>
```

###  定义删除的文本

`<del>`**定义文档中已被删除的文本。**

```html
<p>
    <del>超文本标记语言</del>（标准通用标记语言下的一个应用，外语缩写HTML），是迄今为止网络上应用最为广泛的语言。
</p>
```
###  定义插入的文本

`<ins>`**定义插入的文本**

```html
<p>
    <del>超文本语言</del><ins>超文本标记语言</ins>（标准通用标记语言下的一个应用，外语缩写HTML），是迄今为止网络上应用最为广泛的语言。
</p>
```



###  突出显示文本

`<mark>`**标签定义带有记号的文本。**

```html
<p>
    <mark>超文本标记语言</mark>（标准通用标记语言下的一个应用，外语缩写HTML），是迄今为止网络上应用最为广泛的语言。
</p>
```

###  div标签

*  `<div>`可定义文档中的分区或节(division/section)。

* `<div>`标签可以把文档分割为独立的、不同的部分。它可以用作严格的组织工具，并且不使用任何格式与其关联。

* 如果用 id 或 class 来标记 `<div>`，那么该标签的作用会变得更加有效。

###  span标签

`<span>`标签被用来组合行内元素。

> **span 没有固定的格式表现。当对它应用样式时，它才会产生视觉上的变化。**

```html
<p>
    <span>超文本标记语言</span>（标准通用标记语言下的一个应用，外语缩写HTML），是迄今为止网络上应用最为广泛的语言。
</p>
```

> **如果不对 span 应用样式，那么 span 元素中的文本与其他文本不会任何视觉上的差异。尽管如此，上例中的 span 元素仍然为 p 元素增加了额外的结构。**
>
> **可以为 span 应用 id 或 class 属性，这样既可以增加适当的语义，又便于对 span 应用样式。**

###  图片标签

`<img>`元素用于在页面中嵌入图像，该元素是一个空元素。

**必要属性：**

- src：该属性指定图片文件所在的位置，可以是相对路径，也可以是绝对路径。
- alt：该属性指定一段文本，用来作为该图片的提示信息。

**可选属性：**

- height：指定图片的高度，属性值可以是百分比，也可以是像素值。
- width：指定图片的宽度，属性值可以是百分比，也可以是像素值。

###  链接

####   锚点跳转

```html
		<a href="#tip">跳转</a>
		<p id="tip">........</p>
```

####  页面跳转

```html
		<a href="second.html" target="_blank">_blank</a>
		<a href="second.html" target="_self">_self</a>
		<a href="second.html" target="_parent">_parent</a>
		<a href="second.html" target="_top">_top</a>
```

> * **_blank:**浏览器总在一个新打开、未命名的窗口中载入目标文档。
> * **_self:**这个目标的值对所有没有指定目标的 `<a>` 标签是默认目标，它使得目标文档载入并显示在相同的框架或者窗口中作为源文档。这个目标是多余且不必要的，除非和文档标题 `<base>` 标签中的 target 属性一起使用。
> * **_parent:**这个目标使得文档载入父窗口或者包含来超链接引用的框架的框架集。如果这个引用是在窗口或者在顶级框架中，那么它与目标 _self 等效。
> * **_top:**这个目标使得文档载入包含这个超链接的窗口，用 _top 目标将会清除所有被包含的框架并将文档载入整个浏览器窗口。
>

**target="view_window"**

被指向的超链接使得创建高效的浏览工具变得很容易。例如，一个简单的内容文档的列表，可以将文档重定向到一个单独的窗口：

```html
<h3>Table of Contents</h3>
<ul>
  <li><a href="pref.html" target="view_window">Preface</a></li>
  <li><a href="chap1.html" target="view_window">Chapter 1</a></li>
  <li><a href="chap2.html" target="view_window">Chapter 2</a></li>
  <li><a href="chap3.html" target="view_window">Chapter 3</a></li>
</ul>
```

当用户第一次选择内容列表中的某个链接时，浏览器将打开一个新的窗口，将它标记为 "view_window"，然后在其中显示希望显示的文档内容。如果用户从这个内容列表中选择另一个链接，且这个 "view_window" 仍处于打开状态，浏览器就会再次将选定的文档载入那个窗口，取代刚才的那些文档。

在整个过程中，这个包含了内容列表的窗口是用户可以访问的。通过单击窗口中的一个连接，可使另一个窗口的内容发生变化。

**target="view_frame"**

不用打开一个完整的浏览器窗口，使用 target 更通常的方法是在一个`<frameset>`显示中将超链接内容定向到一个或者多个框架中。可以将这个内容列表放入一个带有两个框架的文档的其中一个框架中，并用这个相邻的框架来显示选定的文档：

```html
<frameset cols="100,*">
  <frame src="toc.html">
  <frame src="pref.html" name="view_frame">
</frameset> 
```

toc.html的内容:

```html
<h3>Table of Contents</h3>
<ul>
  <li><a href="pref.html" target="view_frame">Preface</a></li>
  <li><a href="chap1.html" target="view_frame">Chapter 1</a></li>
  <li><a href="chap2.html" target="view_frame">Chapter 2</a></li>
  <li><a href="chap3.html" target="view_frame">Chapter 3</a></li>
</ul>
```

在文档 "toc.html" 中，每个链接的目标都是 "view_frame"，也就是右边的框架。

当用户从左边框架中的目录中选择一个链接时，浏览器会将这个关联的文档载入并显示在右边这个 "view_frame" 框架中。当其他链接被选中时，右边这个框架中的内容也会发生变化，而左边这个框架始终保持不变。

