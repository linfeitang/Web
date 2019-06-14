```
<form action="action_page.php">
	<input type="" name="">  
</form>
```	  

### 1. \<form>的可选属性
- action
属性定义在提交表单时执行的动作。     
向服务器提交表单的通常做法是使用提交按钮。   
通常，表单会被提交到 web 服务器上的网页。    
如果省略 action 属性，则 action 会被设置为当前页面。         
- method
规定在提交表单时所用的 HTTP方法,其值为GET或POST     
	- 何时使用GET:               
	没有说明时的默认方法       
	此方法在表单提交时是被动的(比如搜索引擎查询),并且最好不要包含敏感信息，因为当您使用GET时，表单数据在页面地址栏中是可见的。GET 最适合少量数据的提交。浏览器会设定容量限制。    
	- 何时使用POST:                      
	如果表单正在更新数据，或者包含敏感信息（例如密码），应当使用此方法。因为POST的安全性更佳，在页面地址栏中被提交的数据是不可见的 
- accept-charset  
规定在被提交表单中使用的字符集（默认：页面字符集）。     
- autocomplete    
规定浏览器应该自动完成表单（默认：开启）。  
- enctype         
规定被提交数据的编码（默认：url-encoded）。    
- method          
规定在提交表单时所用的 HTTP 方法（默认：GET）。   
- name            
规定识别表单的名称（对于 DOM 使用：document.forms.name）。  
- novalidate      
规定浏览器不验证表单。    
- target          
规定 action 属性中地址的目标（默认:self）

### 2. \<form>底下可包含的表单元素:
####  ( 1 ) \<select>元素
定义下拉列表,例如:
```
<select name="城市">
    <option value="上海">上海</option>   
    <option value="北京" selected>北京</option>    
    <option value="巴黎">巴黎</option>     
    <option value="伦敦">伦敦</option>     
</select>
```
<select name="城市">
    <option value="上海">上海</option>   
    <option value="北京" selected>北京</option>    
    <option value="巴黎">巴黎</option>     
    <option value="伦敦">伦敦</option>     
</select>
*其中\<option>元素定义待选择的选项。     
列表通常会把首个选项显示为被选选项。     
您能够通过添加 **selected** 属性来定义预定义选项(例如第二行)*
   

#### ( 2 ) \<input>元素
最为常用,其所有属性如下:
- **tpye,name***这两个是必须的*

 	name可以自定义，tpye的值包含如下：
	- text  
	- password  
  	- reset   定义重置按钮,点击后表中其他已填写的数据被清空  
	- sublimt 定义提交表单数据至表单处理程序的按钮。表单处理程序（form-handler）通常是包含处理输入数据的脚本的服务器页面。在表单的 action 属性中规定表单处理程序（form-handler)  
	- radio   定义单选按钮(通常表现为一个圆那种),如性别的选择  
	- checkbox定义复选框,允许用户进行一个或多个选项    
	- botton  定义按钮  
	- html5新增: 
		- color   定义一个拾色器    
		- email   定义用于Email地址的字段     
		- image   定义图像作为提交按钮     
		- date    定义date控件(年月日)   
		- datetime 定义 date 和 time 控件（包括年、月、日、时、分、秒、几分之一秒，基于 UTC 时区）  
		- datetime-local 同上,但是不带时区   
		- month   定义year和month控件  
		- number  定义用于输入数字的字段  
		- ranger  定义用于精确值不重要的输入数字的控件（比如 slider 控件）。  
		- search  定义用于输入搜索字符串的文本字段。  
		- tel     定义用于输入电话号码的字段。  
		- time    定义用于输入时间的控件（不带时区）。  
		- url     定义用于输入 URL 的字段。  
		- week    定义 week 和 year 控件（不带时区）。  
- value           
规定输入字段的初始值
- readonly        
规定输入字段为只读 
- disabled        
规定输入字段是禁用的。
被禁用的元素是不可用和不可点击的。
被禁用的元素不会被提交
(readonly和disabled不需要有值,直接加上即可)
- size            
规定输入字段的尺寸(以字符计)
- maxlength       
规定输入字段允许的最大长度
如设置 maxlength 属性，则输入控件不会接受超过所允许数的字符。该属性不会提供任何反馈。如果需要提醒用户，则必须编写JavaScript代码。  
*注：输入限制并非万无一失。JavaScript提供了很多方法来增加非法输入。如需安全地限制输入，则接受者（服务器）必须同时对限制进行检查*    
- alt             
定义图像输入的替代文本
- checked         
规定此input元素首次加载时应该被选中(即用户点击之前的默认选择)

- html5新增属性:
	- autocomplete	
	- autofocus	
	- form 	
	- formaction 	
	- formenctype 	
	- formmethod 	
	- formnovalidate 	
	- formtarget 	
	- height 和 width 	
	- list 	
	- min 和 max 	 	
	- multiple 	
	- pattern (regexp) 	
	- placeholder 	
	- required 	
	- step	

### 3. 关于属性的一些输入限制:
- disabled    规定输入字段应该被禁用。   
- max         规定输入字段的最大值。   
- maxlength   规定输入字段的最大字符数。   
- min         规定输入字段的最小值。   
- pattern     规定通过其检查输入值的正则表达式     
- readonly    规定输入字段为只读（无法修改）。   
- required    规定输入字段是必需的（必需填写）     
- size        规定输入字段的宽度（以字符计）    
- step        规定输入字段的合法数字间隔。     
- value       规定输入字段的默认值。       