#前端开发规范  by Manstro-FE-Team
> 最佳原则：坚持制定更高的代码规范。
> 无论团队人数多少，代码应该同出一门。
> 如果你发现本规范中有任何错误，敬请指正。

##目录
<ul>
    <li><a href="#name-rule">命名规则</a>
        <ul>
            <li><a href="#name-rule1">项目命名</a></li>
            <li><a href="#name-rule2">目录命名</a></li>
            <li><a href="#name-rule3">HTML文件命名</a></li>
            <li><a href="#name-rule4">CSS文件命名</a></li>
            <li><a href="#name-rule5">JS文件命名</a></li>
        </ul>
    </li>   
    <li><a href="#html-rule">HTML</a>
        <ul>
            <li><a href="#html-rule1">语法</a></li>
            <li><a href="#html-rule2">HTML5 doctype</a></li>
            <li><a href="#html-rule3">lang属性</a></li>
            <li><a href="#html-rule4">字符编码</a></li>
            <li><a href="#html-rule5">IE兼容模式</a></li>
            <li><a href="#html-rule6">引入CSS，JS</a></li>
            <li><a href="#html-rule7">属性顺序</a></li>
            <li><a href="#html-rule8">boolean属性</a></li>
            <li><a href="#html-rule9">JS生成标签</a></li>
            <li><a href="#html-rule10">减少标签数量</a></li>
            <li><a href="#html-rule11">使用高于完美</a></li>
        </ul>
    </li>   
    <li><a href="#css-rule">CSS</a>
        <ul>
            <li><a href="#css-rule1">缩进</a></li>
            <li><a href="#css-rule2">分号</a></li>
            <li><a href="#css-rule3">空格</a></li>
            <li><a href="#css-rule4">空行</a></li>
            <li><a href="#css-rule5">换行</a></li>
            <li><a href="#css-rule6">注释</a></li>
            <li><a href="#css-rule7">引号</a></li>
            <li><a href="#css-rule8">命名</a></li>
            <li><a href="#css-rule9">属性声明顺序</a></li>
            <li><a href="#css-rule10">颜色</a></li>
            <li><a href="#css-rule11">媒体查询</a></li>
            <li><a href="#css-rule12">杂项</a></li>
        </ul>
    </li>   
    <li><a href="#js-rule">JavaScript</a>
        <ul>
            <li><a href="#js-rule1">缩进</a></li>
            <li><a href="#js-rule2">单行长度</a></li>
            <li><a href="#js-rule3">分号</a></li>
            <li><a href="#js-rule4">空格</a></li>
            <li><a href="#js-rule5">空行</a></li>
            <li><a href="#js-rule6">换行</a></li>
            <li><a href="#js-rule7">单行注释</a></li>
            <li><a href="#js-rule8">多行注释</a></li>
            <li><a href="#js-rule9">文档注释</a></li>
            <li><a href="#js-rule10">引号</a></li>
            <li><a href="#js-rule11">变量命名</a></li>
            <li><a href="#js-rule12">变量声明</a></li>
            <li><a href="#js-rule13">函数</a></li>
            <li><a href="#js-rule14">数组、对象</a></li>
            <li><a href="#js-rule15">括号</a></li>
            <li><a href="#js-rule16">null</a></li>
            <li><a href="#js-rule17">undefined</a></li>
            <li><a href="#js-rule18">jshint</a></li>
            <li><a href="#js-rule19">杂项</a></li>
        </ul>
    </li>   
</ul>


<h1 id="name-rule">命名规则</h1>
<h2 id="name-rule1">项目命名</h2>
>全部采用大驼峰命名。
>例：SmartCamp

<h2 id="name-rule1">目录命名</h2>
>全部采用小写方式，命名较长时以中横线分隔。
> 例：ui、js、css、public-module

<h2 id="name-rule2">HTML文件命名</h2>
>参照目录命名规则。
>例：public.html、public-module.html

<h2 id="name-rule3">CSS文件命名</h2>
>参照目录命名规则。
>例：public.css、public-module.css

<h2 id="name-rule4">JS文件命名</h2>
>参照目录命名规则。
>例：public.js、public-module.js


<h1 id="html-rule">HTML</h1>

<h2 id="html-rule1">语法</h2>
<ul>
    <li>缩进使用soft tab（4个空格）；</li>
    <li>嵌套的节点应该缩进；</li>
    <li>在属性上，使用双引号，不要使用单引号；</li>
    <li>属性名全小写，用中划线做分隔符；</li>
    <li>不要在自动闭合标签结尾处使用斜线（HTML5 规范 指出他们是可选的）；</li>
    <li>不要忽略可选的关闭标签，例：&lt;/li&gt; 和 &lt;/body&gt;。</li>
</ul>
<pre>
&lt;!DOCTYPE html&gt;
&lt;html&gt;
    &lt;head&gt;
        &lt;title&gt;Page title&lt;/title&gt;
    &lt;/head&gt;
    &lt;body&gt;
        &lt;img src="images/company_logo.png" alt="Company"&gt;
        &lt;h1 class="hello-world"&gt;Hello, world!&lt;/h1&gt;
    &lt;/body&gt;
&lt;/html&gt;
</pre>


<h2 id="html-rule2">HTML5 doctype</h2>
在页面开头使用这个简单地doctype来启用标准模式，使其在每个浏览器中尽可能一致的展现；
虽然doctype不区分大小写，但是按照惯例，doctype大写 (
关于html属性，大写还是小写）。

<pre>
<code>
&lt;!DOCTYPE html&gt;
&lt;html&gt;
    ...
&lt;/html&gt;
</code>
</pre>


<h2 id="html-rule3">lang属性</h2>
根据HTML5规范：
应在html标签上加上lang属性。这会给语音工具和翻译工具帮助，告诉它们应当怎么去发音和翻译。
更多关于 lang 属性的说明<a href="http://w3c.github.io/html/semantics.html#the-html-element">在这里</a>；
在sitepoint上可以查到<a href="https://www.sitepoint.com/web-foundations/iso-2-letter-language-codes/">语言列表</a>；
但sitepoint只是给出了语言的大类，例如中文只给出了zh，但是没有区分香港，台湾，大陆。而微软给出了一份更加<a href="https://msdn.microsoft.com/en-us/library/ms533052(v=vs.85).aspx">详细的语言列表</a>，其中细分了zh-cn, zh-hk, zh-tw。

<pre>
&lt;!DOCTYPE html&gt;
&lt;html lang="en-us"&gt;
    ...
&lt;/html&gt;
</pre>

<h2 id="html-rule4">字符编码</h2>
通过声明一个明确的字符编码，让浏览器轻松、快速的确定适合网页内容的渲染方式，通常指定为'UTF-8'。

<pre>
&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;head&gt;
&lt;meta charset="UTF-8"&gt;
&lt;/head&gt;
...
&lt;/html&gt;
</pre>

<h2 id="html-rule5">IE兼容模式</h2>
用 &lt;meta&gt; 标签可以指定页面应该用什么版本的IE来渲染；
不同doctype在不同浏览器下会触发不同的渲染模式（<a href="https://hsivonen.fi/doctype/">这篇文章</a>总结的很到位）。

<pre>
&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;head&gt;
    &lt;meta http-equiv="X-UA-Compatible" content="IE=Edge"&gt;
&lt;/head&gt;
    ...
&lt;/html&gt;
</pre>

<h2 id="html-rule6">引入CSS，JS</h2>
根据HTML5规范, 通常在引入CSS和JS时不需要指明 type，因为 text/css 和 text/javascript 分别是他们的默认值。

<pre>
&lt;!-- External CSS --&gt;
&lt;link rel="stylesheet" href="code_guide.css"&gt;

&lt;!-- In-document CSS --&gt;
&lt;style&gt;
    ...
&lt;/style&gt;

&lt;!-- External JS --&gt;
&lt;script src="code_guide.js">&lt;/script&gt;

&lt;!-- In-document JS --&gt;
&lt;script&gt;
    ...
&lt;/script&gt;
</pre>

<h2 id="html-rule7">属性顺序</h2>
属性应该按照特定的顺序出现以保证易读性；
<ul>
    <li>class</li>
    <li>id</li>
    <li>name</li>
    <li>data-*</li>
    <li>src, for, type, href, value , max-length, max, min, pattern</li>
    <li>placeholder, title, alt</li>
    <li>aria-*, role</li>
    <li>required, readonly, disabled</li>
</ul>
class是为高可复用组件设计的，所以应处在第一位；
id更加具体且应该尽量少使用，所以将它放在第二位。

<pre>
&lt;a class="..." id="..." data-modal="toggle" href="#">Example link&lt;/a&gt;
&lt;input class="form-control" type="text"&gt;
&lt;img src="..." alt="..."&gt;
</pre>


<h2 id="html-rule8">boolean属性</h2>
boolean属性z值不需要声明取值的属性，XHTML需要每个属性声明取值，但是HTML5并不需要；
更多内容可以参考 <a href="https://html.spec.whatwg.org/multipage/infrastructure.html#boolean-attributes">WhatWG section on boolean attributes：</a>
boolean属性的存在表示取值为true，不存在则表示取值为false。

<pre>
&lt;input type="text" disabled&gt;
&lt;input type="checkbox" value="1" checked&gt;
&lt;select&gt;
    &lt;option value="1" selected&gt;1&lt;/option&gt;
&lt;/select&gt;
</pre>

<h2 id="html-rule9">JS生成标签</h2>
在JS文件中生成标签让内容变得更难查找，更难编辑，性能更差。应该尽量避免这种情况的出现。

<h2 id="html-rule10">减少标签数量</h2>
在编写HTML代码时，需要尽量避免多余的父节点；
很多时候，需要通过迭代和重构来使HTML变得更少。

<pre>
&lt;!-- Not well --&gt;
&lt;span class="avatar"&gt;
    &lt;img src="..."&gt;
&lt;/span&gt;

&lt;!-- Better --&gt;
&lt;img class="avatar" src="..."&gt;
</pre>

<h2 id="html-rule11">使用高于完美</h2>
尽量遵循HTML标准和语义，但是不应该以浪费实用性作为代价；

任何时候都要用尽量小的复杂度和尽量少的标签来解决问题。



<h1 id="css-rule">CSS</h1>

<h2 id="css-rule1">缩进</h2>
使用soft tab（4个空格）。

<pre>
.element {
    position: absolute;
    top: 10px;
    left: 10px;
    border-radius: 10px;
    width: 50px;
    height: 50px;
}
</pre>

<h2 id="css-rule2">分号</h2>
每个属性声明末尾都要加分号。

<pre>
.element {
    width: 20px;
    height: 20px;
    background-color: red;
}
</pre>

<h2 id="css-rule3">空格</h2>
以下几种情况不需要空格：
<ul>
    <li>属性名后</li>
    <li>多个规则的分隔符','前</li>
    <li>!important '!'后</li>
    <li>属性值中'('后和')'前</li>
    <li>行末不要有多余的空格</li>
</ul>
以下几种情况需要空格：
<ul>
    <li>属性值前</li>
    <li>选择器'>', '+', '~'前后</li>
    <li>'{'前</li>
    <li>@else 前后</li>
    <li>属性值中的','后</li>
    <li>注释'/ *'后和'* /'前</li>
</ul>

<pre>

/* not good */
.element {
    color :red! important;
    background-color: rgba(0,0,0,.5);
}

/* good */
.element {
    color: red !important;
    background-color: rgba(0, 0, 0, .5);
}

/* not good */
.element ,
.dialog{
    ...
}

/* good */
.element,
.dialog {

}

/* not good */
.element>.dialog{
    ...
}

/* good */
.element > .dialog{
    ...
}

/* not good */
.element{
    ...
}

/* good */
.element {
    ...
}

/* not good */
@if{
    ...
}@else{
    ...
}

/* good */
@if {
    ...
} @else {
    ...
}


</pre>


<h2 id="css-rule4">空行</h2>
以下几种情况需要空行：
<ul>
    <li>文件最后保留一个空行</li>
    <li>'}'后最好跟一个空行，包括scss中嵌套的规则</li>
    <li>属性之间需要适当的空行，具体见<a href="#">属性声明顺序</a></li>
</ul>

<pre>

/* not good */
.element {
    ...
}
.dialog {
    color: red;
    &:after {
        ...
    }
}

/* good */
.element {
    ...
}

.dialog {
    color: red;

    &:after {
        ...
    }
}


</pre>


<h2 id="css-rule5">换行</h2>
以下几种情况不需要换行：
<ul>
    <li>'{'前</li>
</ul>
以下几种情况需要换行：
<ul>
    <li>'{'后和'}'前</li>
    <li>每个属性独占一行</li>
    <li>多个规则的分隔符','后</li>
</ul>

<pre>
/* not good */
.element
{color: red; background-color: black;}

/* good */
.element {
    color: red;
    background-color: black;
}

/* not good */
.element, .dialog {
    ...
}

/* good */
.element,
.dialog {
    ...
}


</pre>


<h2 id="css-rule6">注释</h2>
注释统一用'/* */'（scss中也不要用'//'），具体参照下边的写法；
缩进与下一行代码保持一致；
可位于一个代码行的末尾，与代码间隔一个空格。 

<pre>
/* Modal header */
.modal-header {
    ...
}

/*
 * Modal header
 */
.modal-header {
    ...
}

.modal-header {
    /* 50px */
    width: 50px;

    color: red; /* color red */
}

</pre>


<h2 id="css-rule7">引号</h2>
最外层统一使用双引号；
url的内容要用引号；
属性选择器中的属性值需要引号。

<pre>
.element:after {
    content: "";
    background-image: url("logo.png");
}

li[data-type="single"] {
    ...
}
</pre>

<h2 id="css-rule8">命名</h2>
<ul>
    <li>类名使用小写字母，以中划线分隔</li>
    <li>id使用小写字母，以中划线分隔</li>
    <li>scss中的变量、函数、混合、placeholder采用驼峰式命名</li>
</ul>

<pre>
/* class */
.element-content {
    ...
}

/* id */
#myDialog {
    ...
}

/* 变量 */
$colorBlack: #000;

/* 函数 */
@function pxToRem($px) {
    ...
}

/* 混合 */
@mixin centerBlock {
    ...
}

/* placeholder */
%myDialog {
    ...
}


</pre>


<h2 id="css-rule9">属性声明顺序</h2>
相关的属性声明按右边的顺序做分组处理，组之间需要有一个空行。

<pre>
.declaration-order {
    display: block;
    float: right;

    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    z-index: 100;

    border: 1px solid #e5e5e5;
    border-radius: 3px;
    width: 100px;
    height: 100px;

    font: normal 13px "Helvetica Neue", sans-serif;
    line-height: 1.5;
    text-align: center;

    color: #333;
    background-color: #f5f5f5;

    opacity: 1;
}

// 下面是推荐的属性的顺序
[
    [
        "display",
        "visibility",
        "float",
        "clear",
        "overflow",
        "overflow-x",
        "overflow-y",
        "clip",
        "zoom"
    ],
    [
        "table-layout",
        "empty-cells",
        "caption-side",
        "border-spacing",
        "border-collapse",
        "list-style",
        "list-style-position",
        "list-style-type",
        "list-style-image"
    ],
    [
        "-webkit-box-orient",
        "-webkit-box-direction",
        "-webkit-box-decoration-break",
        "-webkit-box-pack",
        "-webkit-box-align",
        "-webkit-box-flex"
    ],
    [
        "position",
        "top",
        "right",
        "bottom",
        "left",
        "z-index"
    ],
    [
        "margin",
        "margin-top",
        "margin-right",
        "margin-bottom",
        "margin-left",
        "-webkit-box-sizing",
        "-moz-box-sizing",
        "box-sizing",
        "border",
        "border-width",
        "border-style",
        "border-color",
        "border-top",
        "border-top-width",
        "border-top-style",
        "border-top-color",
        "border-right",
        "border-right-width",
        "border-right-style",
        "border-right-color",
        "border-bottom",
        "border-bottom-width",
        "border-bottom-style",
        "border-bottom-color",
        "border-left",
        "border-left-width",
        "border-left-style",
        "border-left-color",
        "-webkit-border-radius",
        "-moz-border-radius",
        "border-radius",
        "-webkit-border-top-left-radius",
        "-moz-border-radius-topleft",
        "border-top-left-radius",
        "-webkit-border-top-right-radius",
        "-moz-border-radius-topright",
        "border-top-right-radius",
        "-webkit-border-bottom-right-radius",
        "-moz-border-radius-bottomright",
        "border-bottom-right-radius",
        "-webkit-border-bottom-left-radius",
        "-moz-border-radius-bottomleft",
        "border-bottom-left-radius",
        "-webkit-border-image",
        "-moz-border-image",
        "-o-border-image",
        "border-image",
        "-webkit-border-image-source",
        "-moz-border-image-source",
        "-o-border-image-source",
        "border-image-source",
        "-webkit-border-image-slice",
        "-moz-border-image-slice",
        "-o-border-image-slice",
        "border-image-slice",
        "-webkit-border-image-width",
        "-moz-border-image-width",
        "-o-border-image-width",
        "border-image-width",
        "-webkit-border-image-outset",
        "-moz-border-image-outset",
        "-o-border-image-outset",
        "border-image-outset",
        "-webkit-border-image-repeat",
        "-moz-border-image-repeat",
        "-o-border-image-repeat",
        "border-image-repeat",
        "padding",
        "padding-top",
        "padding-right",
        "padding-bottom",
        "padding-left",
        "width",
        "min-width",
        "max-width",
        "height",
        "min-height",
        "max-height"
    ],
    [
        "font",
        "font-family",
        "font-size",
        "font-weight",
        "font-style",
        "font-variant",
        "font-size-adjust",
        "font-stretch",
        "font-effect",
        "font-emphasize",
        "font-emphasize-position",
        "font-emphasize-style",
        "font-smooth",
        "line-height",
        "text-align",
        "-webkit-text-align-last",
        "-moz-text-align-last",
        "-ms-text-align-last",
        "text-align-last",
        "vertical-align",
        "white-space",
        "text-decoration",
        "text-emphasis",
        "text-emphasis-color",
        "text-emphasis-style",
        "text-emphasis-position",
        "text-indent",
        "-ms-text-justify",
        "text-justify",
        "letter-spacing",
        "word-spacing",
        "-ms-writing-mode",
        "text-outline",
        "text-transform",
        "text-wrap",
        "-ms-text-overflow",
        "text-overflow",
        "text-overflow-ellipsis",
        "text-overflow-mode",
        "-ms-word-wrap",
        "word-wrap",
        "-ms-word-break",
        "word-break"
    ],
    [
        "color",
        "background",
        "filter:progid:DXImageTransform.Microsoft.AlphaImageLoader",
        "background-color",
        "background-image",
        "background-repeat",
        "background-attachment",
        "background-position",
        "-ms-background-position-x",
        "background-position-x",
        "-ms-background-position-y",
        "background-position-y",
        "-webkit-background-clip",
        "-moz-background-clip",
        "background-clip",
        "background-origin",
        "-webkit-background-size",
        "-moz-background-size",
        "-o-background-size",
        "background-size"
    ],
    [
        "outline",
        "outline-width",
        "outline-style",
        "outline-color",
        "outline-offset",
        "opacity",
        "filter:progid:DXImageTransform.Microsoft.Alpha(Opacity",
        "-ms-filter:\\'progid:DXImageTransform.Microsoft.Alpha",
        "-ms-interpolation-mode",
        "-webkit-box-shadow",
        "-moz-box-shadow",
        "box-shadow",
        "filter:progid:DXImageTransform.Microsoft.gradient",
        "-ms-filter:\\'progid:DXImageTransform.Microsoft.gradient",
        "text-shadow"
    ],
    [
        "-webkit-transition",
        "-moz-transition",
        "-ms-transition",
        "-o-transition",
        "transition",
        "-webkit-transition-delay",
        "-moz-transition-delay",
        "-ms-transition-delay",
        "-o-transition-delay",
        "transition-delay",
        "-webkit-transition-timing-function",
        "-moz-transition-timing-function",
        "-ms-transition-timing-function",
        "-o-transition-timing-function",
        "transition-timing-function",
        "-webkit-transition-duration",
        "-moz-transition-duration",
        "-ms-transition-duration",
        "-o-transition-duration",
        "transition-duration",
        "-webkit-transition-property",
        "-moz-transition-property",
        "-ms-transition-property",
        "-o-transition-property",
        "transition-property",
        "-webkit-transform",
        "-moz-transform",
        "-ms-transform",
        "-o-transform",
        "transform",
        "-webkit-transform-origin",
        "-moz-transform-origin",
        "-ms-transform-origin",
        "-o-transform-origin",
        "transform-origin",
        "-webkit-animation",
        "-moz-animation",
        "-ms-animation",
        "-o-animation",
        "animation",
        "-webkit-animation-name",
        "-moz-animation-name",
        "-ms-animation-name",
        "-o-animation-name",
        "animation-name",
        "-webkit-animation-duration",
        "-moz-animation-duration",
        "-ms-animation-duration",
        "-o-animation-duration",
        "animation-duration",
        "-webkit-animation-play-state",
        "-moz-animation-play-state",
        "-ms-animation-play-state",
        "-o-animation-play-state",
        "animation-play-state",
        "-webkit-animation-timing-function",
        "-moz-animation-timing-function",
        "-ms-animation-timing-function",
        "-o-animation-timing-function",
        "animation-timing-function",
        "-webkit-animation-delay",
        "-moz-animation-delay",
        "-ms-animation-delay",
        "-o-animation-delay",
        "animation-delay",
        "-webkit-animation-iteration-count",
        "-moz-animation-iteration-count",
        "-ms-animation-iteration-count",
        "-o-animation-iteration-count",
        "animation-iteration-count",
        "-webkit-animation-direction",
        "-moz-animation-direction",
        "-ms-animation-direction",
        "-o-animation-direction",
        "animation-direction"
    ],
    [
        "content",
        "quotes",
        "counter-reset",
        "counter-increment",
        "resize",
        "cursor",
        "-webkit-user-select",
        "-moz-user-select",
        "-ms-user-select",
        "user-select",
        "nav-index",
        "nav-up",
        "nav-right",
        "nav-down",
        "nav-left",
        "-moz-tab-size",
        "-o-tab-size",
        "tab-size",
        "-webkit-hyphens",
        "-moz-hyphens",
        "hyphens",
        "pointer-events"
    ]
]


</pre>


<h2 id="css-rule10">颜色</h2>
颜色16进制用小写字母；

颜色16进制尽量用简写。

<pre>
/* not good */
.element {
    color: #ABCDEF;
    background-color: #001122;
}

/* good */
.element {
    color: #abcdef;
    background-color: #012;
}


</pre>

<h2 id="css-rule11">属性简写</h2>
属性简写需要你非常清楚属性值的正确顺序，而且在大多数情况下并不需要设置属性简写中包含的所有值，所以建议尽量分开声明会更加清晰；

margin 和 padding 相反，需要使用简写；

常见的属性简写包括：
<ul>
    <li>font</li>
    <li>background</li>
    <li>transition</li>
    <li>animation</li>
</ul>

<pre>


/* not good */
.element {
    transition: opacity 1s linear 2s;
}

/* good */
.element {
    transition-delay: 2s;
    transition-timing-function: linear;
    transition-duration: 1s;
    transition-property: opacity;
}


</pre>


<h2 id="css-rule12">媒体查询</h2>
尽量将媒体查询的规则靠近与他们相关的规则，不要将他们一起放到一个独立的样式文件中，或者丢在文档的最底部，这样做只会让大家以后更容易忘记他们。

<pre>
.element {
    ...
}

.element-avatar{
    ...
}

@media (min-width: 480px) {
    .element {
        ...
    }

    .element-avatar {
        ...
    }
}


</pre>

<h2 id="css-rule13">杂项</h2>
不允许有空的规则；

元素选择器用小写字母；

去掉小数点前面的0；

去掉数字中不必要的小数点和末尾的0；

属性值'0'后面不要加单位；

同个属性不同前缀的写法需要在垂直方向保持对齐，具体参照右边的写法；

无前缀的标准属性应该写在有前缀的属性后面；

不要在同个规则里出现重复的属性，如果重复的属性是连续的则没关系；

不要在一个文件里出现两个相同的规则；

用 border: 0; 代替 border: none;；

选择器不要超过4层（在scss中如果超过4层应该考虑用嵌套的方式来写）；

发布的代码中不要有 @import；

尽量少用'*'选择器。

<pre>
/* not good */
.element {
}

/* not good */
LI {
    ...
}

/* good */
li {
    ...
}

/* not good */
.element {
    color: rgba(0, 0, 0, 0.5);
}

/* good */
.element {
    color: rgba(0, 0, 0, .5);
}

/* not good */
.element {
    width: 50.0px;
}

/* good */
.element {
    width: 50px;
}

/* not good */
.element {
    width: 0px;
}

/* good */
.element {
    width: 0;
}


/* not good */
.element {

    border-radius: 3px;
    -webkit-border-radius: 3px;
    -moz-border-radius: 3px;

    background: linear-gradient(to bottom, #fff 0, #eee 100%);
    background: -webkit-linear-gradient(top, #fff 0, #eee 100%);
    background: -moz-linear-gradient(top, #fff 0, #eee 100%);
}

/* good */
.element {

    -webkit-border-radius: 3px;
       -moz-border-radius: 3px;
            border-radius: 3px;

    background: -webkit-linear-gradient(top, #fff 0, #eee 100%);
    background:    -moz-linear-gradient(top, #fff 0, #eee 100%);
    background:         linear-gradient(to bottom, #fff 0, #eee 100%);
}

/* not good */
.element {
    color: rgb(0, 0, 0);
    width: 50px;
    color: rgba(0, 0, 0, .5);
}

/* good */
.element {
    color: rgb(0, 0, 0);
    color: rgba(0, 0, 0, .5);
}

</pre>


<h1 id="js-rule">JavaScript</h1>

<h2 id="js-rule1">缩进</h2>
使用soft tab（4个空格）。

<pre>
var x = 1,
y = 1;

if (x &lt; y) {
    x += 10;
} else {
    x += 1;
}
</pre>

<h2 id="js-rule2">单行长度</h2>
不要超过80，但如果编辑器开启word wrap可以不考虑单行长度。

<h2 id="js-rule3">分号</h2>
以下几种情况后需加分号：
<ul>
<li>变量声明</li>
<li>表达式</li>
<li>return</li>
<li>throw</li>
<li>break</li>
<li>continue</li>
<li>do-while</li>
</ul>

<pre>
/* var declaration */
var x = 1;

/* expression statement */
x++;

/* do-while */
do {
    x++;
} while (x < 10);
</pre>

<h2 id="js-rule4">空格</h2>
以下几种情况不需要空格：
<ul>
<li>对象的属性名后</li>
<li>前缀一元运算符后</li>
<li>后缀一元运算符前</li>
<li>函数调用括号前</li>
<li>无论是函数声明还是函数表达式，'('前不要空格</li>
<li>数组的'['后和']'前</li>
<li>对象的'{'后和'}'前</li>
<li>运算符'('后和')'前</li>
</ul>
以下几种情况需要空格：
<ul>
<li>二元运算符前后</li>
<li>三元运算符'?:'前后</li>
<li>代码块'{'前</li>
<li>下列关键字前：else, while, catch, finally</li>
<li>下列关键字后：if, else, for, while, do, switch, case, try, catch, finally, with, return, typeof</li>
<li>单行注释'//'后（若单行注释和代码同行，则'//'前也需要），多行注释'*'后</li>
<li>对象的属性值前</li>
<li>for循环，分号后留有一个空格，前置条件如果有多个，逗号后留一个空格</li>
<li>无论是函数声明还是函数表达式，'{'前一定要有空格</li>
<li>函数的参数之间</li>
</ul>

<pre>
// not good
var a = {
    b :1
};

// good
var a = {
    b: 1
};

// not good
++ x;
y ++;
z = x?1:2;

// good
++x;
y++;
z = x ? 1 : 2;

// not good
var a = [ 1, 2 ];

// good
var a = [1, 2];

// not good
var a = ( 1+2 )*3;

// good
var a = (1 + 2) * 3;

// no space before '(', one space before '{', 
//one space between function parameters
var doSomething = function(a, b, c) {
    // do something
};

// no space before '('
doSomething(item);

// not good
for(i=0;i&lt;6;i++){
    x++;
}

// good
for (i = 0; i &lt; 6; i++) {
    x++;
}
</pre>

<h2 id="js-rule5">空行</h2>
以下几种情况需要空行：
<ul>
<li>变量声明后（当变量声明在代码块的最后一行时，则无需空行）</li>
<li>注释前（当注释在代码块的第一行时，则无需空行）</li>
<li>代码块后（在函数调用、数组、对象中则无需空行）</li>
<li>文件最后保留一个空行</li>
</ul>

<pre>
// need blank line after variable declaration
var x = 1;

// not need blank line when variable declaration is last expression in 
the current block
if (x >= 1) {
    var y = x + 1;
}

var a = 2;

// need blank line before line comment
a++;

function b() {
// not need blank line when comment is first line of block
return a;
}

// need blank line after blocks
for (var i = 0; i < 2; i++) {
if (true) {
    return false;
}

continue;
}

var obj = {
foo: function() {
    return 1;
},

bar: function() {
    return 2;
}
};

// not need blank line when in argument list, array, object
func(
2,
function() {
    a++;
},
3
);

var foo = [
2,
function() {
    a++;
},
3
];


var foo = {
a: 2,
b: function() {
    a++;
},
c: 3
};
</pre>

<h2 id="js-rule6">换行</h2>
换行的地方，行末必须有','或者运算符；
以下几种情况不需要换行：
<ul>
    <li>下列关键字后：else, catch, finally</li>
    <li>代码块'{'前</li>
</ul>
以下几种情况需要换行：
<ul>
    <li>代码块'{'后和'}'前</li>
    <li>变量赋值后</li>
</ul>

<pre>
// not good
var a = {
b: 1
, c: 2
};

x = y
? 1 : 2;

// good
var a = {
b: 1,
c: 2
};

x = y ? 1 : 2;
x = y ?
1 : 2;

// no need line break with 'else', 'catch', 'finally'
if (condition) {
...
} else {
...
}

try {
...
} catch (e) {
...
} finally {
...
}

// not good
function test()
{
...
}

// good
function test() {
...
}

// not good
var a, foo = 7, b,
c, bar = 8;

// good
var a,
foo = 7,
b, c, bar = 8;
</pre>

<h2 id="js-rule7">单行注释</h2>
双斜线后，必须跟一个空格；
缩进与下一行代码保持一致；
可位于一个代码行的末尾，与代码间隔一个空格。 

<pre>
if (condition) {
    // if you made it here, then all security checks passed
    allowed();
}

var zhangsan = 'zhangsan'; // one space after code
</pre>

<h2 id="js-rule8">多行注释</h2>
最少三行, '*'后跟一个空格，具体参照右边的写法；
建议在以下情况下使用： 
<ul>
    <li>难于理解的代码段</li>
    <li>可能存在错误的代码段</li>
    <li>浏览器特殊的HACK代码</li>
    <li>业务逻辑强相关的代码</li>
</ul>

<pre>
/*
 + one space after '*'
 */
var x = 1;
</pre>


<h2 id="js-rule9">文档注释</h2>
各类标签@param, @method等请参考<a href="http://usejsdoc.org/">usejsdoc</a>和<a href="http://yuri4ever.github.io/jsdoc/">JSDoc Guide</a>；

建议在以下情况下使用：
<ul>
    <li>所有常量</li>
    <li>所有函数</li>
    <li>所有类</li>
</ul>

<pre>
/**
 + @func
 + @desc 一个带参数的函数
 + @param {string} a - 参数a
 + @param {number} b=1 - 参数b默认值为1
 + @param {string} c=1 - 参数c有两种支持的取值 1—表示x 2—表示xx
 + @param {object} d - 参数d为一个对象
 + @param {string} d.e - 参数d的e属性
 + @param {string} d.f - 参数d的f属性
 + @param {object[]} g - 参数g为一个对象数组
 + @param {string} g.h - 参数g数组中一项的h属性
 + @param {string} g.i - 参数g数组中一项的i属性
 + @param {string} [j] - 参数j是一个可选参数
 */
function foo(a, b, c, d, g, j) {
...
}
</pre>

<h2 id="js-rule10">引号</h2>
最外层统一使用单引号。

<pre>
// not good
var x = "test";

// good
var y = 'foo',
z = '&lt;div id="test"&gt;&lt;/div&gt;';
</pre>


<h2 id="js-rule11">变量命名</h2>
<ul>
    <li>标准变量采用驼峰式命名（除了对象的属性外，主要是考虑到cgi返回的数据）</li>
    <li>'ID'在变量名中全大写</li>
    <li>'URL'在变量名中全大写</li>
    <li>'Android'在变量名中大写第一个字母</li>
    <li>'iOS'在变量名中小写第一个，大写后两个字母</li>
    <li>常量全大写，用下划线连接</li>
    <li>构造函数，大写第一个字母</li>
    <li>jquery对象必须以'$'开头命名</li>
</ul>

<pre>
var thisIsMyName;
var goodID;
var reportURL;
var AndroidVersion;
var iOSVersion;
var MAX_COUNT = 10;

function Person(name) {
    this.name = name;
}

// not good
var body = $('body');

// good
var $body = $('body');
</pre>


<h2 id="js-rule12">变量声明</h2>
一个函数作用域中所有的变量声明尽量提到函数首部，用一个var声明，不允许出现两个连续的var声明。

<pre>
function doSomethingWithItems(items) {
    // use one var
    var value = 10,
        result = value + 10,
        i,
        len;

    for (i = 0, len = items.length; i < len; i++) {
        result += 10;
    }
}
</pre>


<h2 id="js-rule13">函数</h2>
无论是函数声明还是函数表达式，'('前不要空格，但'{'前一定要有空格；

函数调用括号前不需要空格；

立即执行函数外必须包一层括号；

不要给inline function命名；

参数之间用', '分隔，注意逗号后有一个空格。

<pre>
// no space before '(', but one space before'{'
var doSomething = function(item) {
    // do something
};

function doSomething(item) {
    // do something
}

// not good
doSomething (item);

// good
doSomething(item);

// requires parentheses around immediately invoked function expressions
(function() {
    return 1;
})();

// not good
[1, 2].forEach(function x() {
    ...
});

// good
[1, 2].forEach(function() {
    ...
});

// not good
var a = [1, 2, function a() {
    ...
}];

// good
var a = [1, 2, function() {
    ...
}];

// use ', ' between function parameters
var doSomething = function(a, b, c) {
    // do something
};
</pre>

<h2 id="js-rule14">数组、对象</h2>
对象属性名不需要加引号；

对象以缩进的形式书写，不要写在一行；

数组、对象最后不要有逗号。

<pre>
// not good
var a = {
    'b': 1
};

var a = {b: 1};

var a = {
    b: 1,
    c: 2,
};

// good
var a = {
    b: 1,
    c: 2
};
</pre>

<h2 id="js-rule15">括号</h2>
下列关键字后必须有大括号（即使代码块的内容只有一行）：if, else, for, while, do, switch, try, catch, finally, with。

<pre>
// not good
if (condition)
doSomething();

// good
if (condition) {
    doSomething();
}
</pre>

<h2 id="js-rule16">null</h2>
适用场景：
<ul>
    <li>初始化一个将来可能被赋值为对象的变量</li>
    <li>与已经初始化的变量做比较</li>
    <li>作为一个参数为对象的函数的调用传参</li>
    <li>作为一个返回对象的函数的返回值</li>
    </ul>
    不适用场景：
    <ul>
    <li>不要用null来判断函数调用时有无传参</li>
    <li>不要与未初始化的变量做比较</li>
</ul>

<pre>
// not good
function test(a, b) {
    if (b === null) {
        // not mean b is not supply
        ...
    }
}

var a;

if (a === null) {
    ...
}

// good
var a = null;

if (a === null) {
    ...
}
</pre>

<h2 id="js-rule17">undefined</h2>
永远不要直接使用undefined进行变量判断；

使用typeof和字符串'undefined'对变量进行判断。

<pre>
// not good
if (person === undefined) {
    ...
}

// good
if (typeof person === 'undefined') {
    ...
}
</pre>

<h2 id="js-rule18">jshint</h2>
用'===', '!=='代替'==', '!='；

for-in里一定要有hasOwnProperty的判断；

不要在内置对象的原型上添加方法，如Array, Date；

不要在内层作用域的代码里声明了变量，之后却访问到了外层作用域的同名变量；

变量不要先使用后声明；

不要在一句代码中单单使用构造函数，记得将其赋值给某个变量；

不要在同个作用域下声明同名变量；

不要在一些不需要的地方加括号，例：delete(a.b)；

不要使用未声明的变量（全局变量需要加到.jshintrc文件的globals属性里面）；

不要声明了变量却不使用；

不要在应该做比较的地方做赋值；

debugger不要出现在提交的代码里；

数组中不要存在空元素；

不要在循环内部声明函数；

不要像这样使用构造函数，例：new function () { ... }, new Object；

<pre>
// not good
if (a == 1) {
    a++;
}

// good
if (a === 1) {
    a++;
}

// good
for (key in obj) {
    if (obj.hasOwnProperty(key)) {
        // be sure that obj[key] belongs to the object and was not inherited
        console.log(obj[key]);
    }
}

// not good
Array.prototype.count = function(value) {
    return 4;
};

// not good
var x = 1;

function test() {
    if (true) {
        var x = 0;
    }

    x += 1;
}

// not good
function test() {
    console.log(x);

    var x = 1;
}

// not good
new Person();

// good
var person = new Person();

// not good
delete(obj.attr);

// good
delete obj.attr;

// not good
if (a = 10) {
    a++;
}

// not good
var a = [1, , , 2, 3];

// not good
var nums = [];

for (var i = 0; i < 10; i++) {
(function(i) {
    nums[i] = function(j) {
        return i + j;
    };
}(i));
}

// not good
var singleton = new function() {
var privateVar;

this.publicMethod = function() {
    privateVar = 1;
};

this.publicMethod2 = function() {
    privateVar = 2;
};
};


</pre>
 
<h2 id="js-rule19">杂项</h2>
不要混用tab和space；

不要在一处使用多个tab或space；

换行符统一用'LF'；

对上下文this的引用只能使用'_this', 'that', 'self'其中一个来命名；

行尾不要有空白字符；

switch的falling through和no default的情况一定要有注释特别说明；

不允许有空的代码块。

<pre>
// not good
var a   = 1;

function Person() {
// not good
var me = this;

// good
var _this = this;

// good
var that = this;

// good
var self = this;
}

// good
switch (condition) {
case 1:
case 2:
    ...
    break;
case 3:
    ...
// why fall through
case 4
    ...
    break;
// why no default
}

// not good with empty block
if (condition) {

}

</pre>