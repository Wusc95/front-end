# 特殊的IMG标签
> 写这篇文章源自我之前的一次面试，题目便是问img标签属于块级元素还是行内元素，当时想都没想就说了是行内(inline)元素，经过面试官的指点和解释，才知道自己是如此的无知。

## 阅读本文您将收获
* `<img />`标签的基本使用
* MDN关于元素的定义
* 特殊的可替换元素

## `<img />` 标签的基本使用
### 浏览器支持
* 所有主流浏览器都支持 `<img>` 标签

### 标签定义及使用说明
* `<img>` 标签定义 HTML 页面中的图像
* `<img>` 标签有两个必需的属性：src 和 alt
* 我们强烈推荐您在文档的每个图像中都使用 alt 属性。这样即使图像无法显示，用户还是可以看到关于丢失了什么东西的一些信息。而且对于残疾人来说，alt 属性通常是他们了解图像内容的唯一方式

## 元素的定义
* 从元素本身的特点来讲，可以分为不可替换元素和替换元素

### 不可替换元素
* `(X)HTML` 的大多数元素是不可替换元素，即其内容直接表现给用户端(例如浏览器)
* 如：`<h1>我是标题</h1>`

### 可替换元素
* 浏览器根据元素的标签和属性，来决定元素的具体显示内容
* 例如浏览器会根据 `<img>` 标签的src属性的值来读取图片信息并显示出来，而如果查看(X)HTML代码，则看不到图片的实际内容；又例如根据 `<input>` 标签的type属性来决定是显示输入框，还是单选按钮等
* (X)HTML中的 `<img>、<input>、<textarea>、<select>、<object>` 都是替换元素。这些元素往往没有实际的内容，即是一个空元素
* 如：`<img src="tigger.jpg"/>`、`<input type="submit" name="Submit" value="提交"/>`

## 特殊的可替换元素
* `<img>`属于可替换元素
* `<img>`同时具有行内元素，行内块，和块级元素的特性
* 替换元素一般有内在尺寸，所以具有 `width` 和 `height`，可以设定
	* 例如你不指定 `<img>` 的 `width` 和 `height` 时，就按其内在尺寸显示，也就是图片被保存的时候的宽度和高度
* 对于表单元素，浏览器也有默认的样式，包括宽度和高度
* `<img>、<input>`属于行内替换元素。`height/width/padding/margin`均可用。效果等于块元素