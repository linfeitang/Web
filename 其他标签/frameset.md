\<frameset cols="25%,75%">  
&emsp;\<frame src="frame_a.htm" noresize="noresize">  
&emsp;\<frame src="frame_b.htm">  
\</frameset>
---
**noresize属性可规定框架是否可调节大小**		

### 1. <frameset>,框架结构标签,定义如何将窗口分割为框架   	
>每个 frameset 定义了一系列行rows或列cols       	
>rows/columns(cols) 的值规定了每行或每列占据屏幕的面积   	     
>frameset是无法与body标签连用的      

>通过使用框架，你可以在同一个浏览器窗口中显示不止一个页面。每份HTML文档称为一个框架，并且每个框架都独立于其他的框架。    

>其中框架标签<frame>定义了放置在每个框架结构标签<frameset>中的html文档   
>其内的noresize属性的noresize值规定了显示在浏览器中的框架大小不可改变(这个我觉得还是蛮有用的)        

### 2. <iframe>,内联框架,一般用于在网页中显示网页,其可选属性包括如下:    
#### src                 
>规定在框架中要显示的网页的URL    
#### height,width  
>定义框架的大小  
#### frameborder  0或1,   
>规定是否显示框架周围的边框。  
#### marginheight        
>规定iframe顶部到底部的边距    
#### marginwidth         
>规定iframe左侧到右侧的边距    
#### name                
>定义该iframe的名字(当某个超链接的target值与该name相同时,超链接将在该框架内打开)   

********************************************