	<table border="" cellpadding="" cellspacing="" border="" bgclolr="" background="" frame="">	
	    <caption>表格的标题</caption>			
	    <tr>		
	        <td align="" rowspan="" colspan="">每个单元格中的数据</td>				
	    </tr>			
	</table>			

**每个表格由table标签开始     
表中的每一行由\<tr>标签(table row)开始,内嵌\<th>标签可用于定义表头(表现为粗体居中)      
行中的每一个数据由\<td>标签(table date)开始     
(数据单元格可以包含文本、图片、列表、段落、表单、水平线、表格等等** 

\<caption>标题\</caption> 属性可定义表格的标题	
### 1. \<table>属性	
#### border
>决定了表格边框的大小,如果不定义或者使border="0",则不显示边框      
#### cellpadding
>决定了表格单元格的边距      
#### cellspacing
>决定了表格单元格的间距      
#### bgcolor
>决定了表格的颜色,不设置则默认为透明           
#### background
>让表格带有背景图片     
#### frame
>表格的框架属性,其值可以为bo  x,above,below,hsides,vsides,            
>(具体可见http://www.w3school.com.cn/tiy/t.asp?f=html_table_frame)        
#### 2. 其中\<td>标签的可选属性有
##### align
>决定数据在单元格中的位置    
##### rowspan和colspan
>可对单元格进行合并,使得某一单元格可以跨越多行或多列单元格  

#### 3. 关于\<thead>,\<tfoot>,\<tbody>(一般很少使用)  
><thead> 标签定义表格的表头。该标签用于组合 HTML 表格的表头内容。  
>thead 元素应该与 tbody 和 tfoot 元素结合起来使用。  
>tbody 元素用于对 HTML 表格中的主体内容进行分组，     
>tfoot 元素用于对 HTML 表格中的表注（页脚）内容进行分组。     

>注释：如果您使用 thead、tfoot 以及 tbody 元素，您就必须使用全部的元素。它们的出现次序是：thead、tfoot、tbody    
>这样浏览器就可以在收到所有数据前呈现页脚了。您必须在 table 元素内部使用这些标签。   
>提示：在默认情况下这些元素不会影响到表格的布局。不过，您可以使用 CSS 使这些元素改变表格的外观。     
>thead、tfoot 以及 tbody 元素使您有能力对表格中的行进行分组。当您创建某个表格时，  
>您也许希望拥有一个标题行，一些带有数据的行，以及位于底部的一个总计行。    
>这种划分使浏览器有能力支持独立于表格标题和页脚的表格正文滚动。    
>当长的表格被打印时，表格的表头和页脚可被打印在包含表格数据的每张页面上。  