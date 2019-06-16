|主流浏览器			|内核		|	
|------				|------ 	|
|IE					|trident	
|Firefox			|Gecko		|	
|Google chrome		|Webkit/blink|	
|Safari				|Webkit		|	
|Opera				|Presto		|	

#### css权重
**！important > 行间样式的优先级 > 引入样式 > 大于页面样式。**

|选择器          |css权重值|  
|--------		|-------|
|!important		|Infinity|				
|行间样式		|1000	|			
|id				|100	|
|class/属性/伪类	|10		|		
|标签/伪元素		|1		|		
|通配符			|0		|

*其中权重值采用的是256进制*  

### HTML 元素
*定义:指的是从开始标签（start tag）到结束标签（end tag）的所有代码。*

>HTML 元素以开始标签起始  
HTML 元素以结束标签终止  
元素的内容是开始标签与结束标签之间的内容  
某些 HTML 元素具有空内容（empty content）  
空元素在开始标签中进行关闭（以开始标签的结束而结束）  
大多数 HTML 元素可拥有属性  
大多数 HTML 元素可以嵌套（可以包含其他 HTML元素）  
在开始标签中添加斜杠，比如 \<br />，是关闭空元素的正确方法  
即使 \<br> 在所有浏览器中都是有效的，但使用\ <br /> 其实是更长远的保障。  

<small>推荐所有的标签都使用小写!</small>

### HTML元素的全局属性:  
- `accesskey 	   ` 规定激活元素的快捷键。  
- `class 		 ` 规定元素的一个或多个类名（引用样式表中的类）。   
- `contenteditable` 规定元素内容是否可编辑。  
- `contextmenu  ` 规定元素的上下文菜单。上下文菜单在用户点击元素时显示。  
- `data-* 	  ` 	用于存储页面或应用程序的私有定制数据。  
- `dir 		 ` 规定元素中内容的文本方向。  
- `draggable 	 ` 规定元素是否可拖动。  
- `dropzone 	 ` 规定在拖动被拖动数据时是否进行复制、移动或链接。   
- `hidden 	  ` 	规定元素仍未或不再相关。  
- `id 		  ` 	规定元素的唯一 id。   
- `lang 		 ` 规定元素内容的语言。  
- `spellcheck   ` 	规定是否对元素进行拼写和语法检查。  
- `style 		 ` 规定元素的行内 CSS 样式。  
- `tabindex 	 ` 规定元素的 tab 键次序。  
- `title 		 ` 规定有关元素的额外信息。  
- `translate 	 ` 规定是否应该翻译元素内容。  

### 文本格式化标签     
- `<b>`			    <b>粗体</b>    
- `<big>`			<big>大号字</big>    
- `<em>` 			<em>强调文字并以斜体显示</em>  
- `<i>` 			<i>定义斜体字</i>  	
- `<small> `		<small>定义小号字</small>  
- `<strong>` 		<strong>定义加重语气</strong>       
- `<sub>`			<sub>定义下标字</sub>         
- `<sup>`			<sup>定义上标字</sup>      
- `<ins>`			<ins>定义插入字</ins>      
- `<del>`			<del>定义删除字</del>      
- `<s>` 			<s>不赞成使用,使用\<del>代替</s>       
- `<strike>` 		<strike>不赞成使用,使用\<del>代替</strike>        
- `<u>` 			<u>不赞成使用,使用样式(style)代替</u>     

### 引用和术语类标签      
- `<abbr>`        	<abbr>定义缩写(添加上title属性后当将鼠标指针置于缩略词上的时候,浏览器会显示title属性里所描述的完整的内容)</abbr>  
- `<acronym>`      	<acronym>定义首字母缩写。</acronym>    
- `<address>`   		<address>定义地址。(即类似于电话簿上联系人等各种信息)此元素通常以斜体显示。大多数浏览器会在此元素前后添加折行。</address>    
- `<bdo>`			    <bdo>定义文字方向。(源代码中的文字在浏览器中的显示顺序)</bdo>	  
- `<blockquote>`	    <blockpuote>定义长的引用。</blockpuote>	  
- `<q>`			    <q>定义短的引用语。该标签内的文本显示时两端会被浏览器带上引号	 注意:这与直接在文本中输入""的效果是不同的</q>	  
- `<cite>`			<cite>定义著作,文章等的标题</cite>	
- `<dfn>`			    <dfn>定义一个定义项目。添加title属性后会获得跟abbr一样的效果,但因为有了dfn的标记	,使得该项目能够为浏览器、翻译系统以及搜索引擎提供更加有用的信息。</dfn>	          

### 计算机输出格式化标签    
- `<code>`		<code>定义计算机代码。本身不会保留源代码中的空格和空行,所以可结合\<pre>标签使用,该标签使得源代码中的空格,换行等在浏览器中都能得以保留并正常显示,所以非常适合用来插入一段代码(甚至只使用pre也行,我没看出什么区别)</code>    
- `<kbd>` 		<kbd>定义键盘文本用于与普通文本区别开来,提示该文本是需要从键盘上键入的,常用于与计算机相关的文档或手册中</kbd>    
- `<var>` 		<var>定义(数学)变量是计算机文档中应用的另一个小窍门,用来显示计算机编程代码范例及类似方面的特定元素。常与code和pre标签连用,且被其标记的文本通常显示为斜体</var>    
- `<samp>`		<samp>定义计算机代码样本,即输出示例</samp>    
- `<tt>` 			<tt>定义打字机代码。</tt>                 
- `<pre>`			<pre>定义预格式文本。</pre>    
- `<listing>`     不赞成使用。使用\<pre>代替。     
- `<plaintext>`	不赞成使用。使用\<pre>代替。     
- `<xmp>`			不赞成使用。使用\<pre>代替。    