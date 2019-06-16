## 复杂选择器
### 1.父子选择器/派生选择器
html代码
```
<div class="red">
	<p>123</p>
</div>
<p>456</p>
```
css代码
```
div p{
	background-color:red;
}
```
![](https://github.com/linfeitang/diary/blob/master/Pictures/20190616215515.jpg)

*注：只要能体现出父子关系就可以，不一定非要用标签表示，也可以用标签所对应的class或者id来表示父子关系*  
所以css还可以这样写：
```
[class="123"] p{
	background-color: red;

}
```

### 2.直接子元素选择器
html代码
```
<div>
	<em>123</em>
	<strong>
		<em>456</em>
	</strong>
</div>
```

css代码：
```
div > em{
	background-color: green;
}
```
![](https://github.com/linfeitang/diary/blob/master/Pictures/20190616214243.jpg)
可以看到只有直属于div的em才被样式化，而strong下的em没有生效。

### 3.并列选择器
html代码：实现效果：只让内容456对样式生效
```
<div>123</div>
<div class="demo">456</div>
<p class="demo">789</p>
```
css代码：
```
div.demo{
	background-color: red;
}
```
![](https://github.com/linfeitang/diary/blob/master/Pictures/20190616220056.jpg)
