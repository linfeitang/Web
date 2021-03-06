## \<div>
1. \<div> 元素是块级元素，它是可用于组合其他 HTML 元素的容器。 
2. \<div> 元素没有特定的含义。除此之外，由于它属于块级元素，浏览器会在其前后显示折行。如果与 CSS 一同使用，可以通过 \<div> 的 class 或 id 应用额外的样式。   
3. \<div>元素可用于对大的内容块设置样式属性。     
4. \<div> 元素的另一个常见的用途是文档布局。它取代了使用表格定义布局的老式方法		
使用\<table> 元素进行文档布局不是表格的正确用法。\<table> 元素的作用是显示表格化的数据。   
5. \<div> 可定义文档中的分区或节（division/section）。
6. \<div>标签可以把文档分割为独立的、不同的部分。它可以用作严格的组织工具,并且不使用任何格式与其关联。如果用id或 class来标记<div>,那么该标签的作用会变得更加有效

>不必为每一个 \<div> 都加上类或 id，虽然这样做也有一定的好处。
>可以对同一个 \<div> 元素应用 class 或 id 属性，但是更常见的情况是只应用其中一种。这两者的主要差异是，class 用于元素组（类似的元素，或者可以理解为某一类元素），而 id 用于标识单独的唯一的元素。 

**关于其两个属性class和id,在同一个 HTML 文档中，可以使用多次 class(且class的值可以相同)，但只能使用一次 id。**

#### id的规则:  
>id 值必须以字母或者下划线开始；不能以数字开始。虽然 W3C 验证不会捕获这个错误,但是 XML 解析器会的。    
>同时，如果你将 id 与 JavaScript 在表单中配合使用，那么 id 名称和值必须是合法的 JavaScript变量。    
>空格和连字号，特别是连字号，是不被允许的。不仅如此，将下划线用于 class 或者 id 名都不是个好主意，这是由于在CSS2.0（以及某些浏览器）中的限制。      

**************************************