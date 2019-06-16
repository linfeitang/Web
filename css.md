## 复杂选择器
- 父子选择器/派生选择器

html代码
```
<div>
	<p>这里的内容被样式化了</p>
</div>
<p>这里的内容没有被样式化</p>
```
css代码
```
div p{
	background-color:red;
}
```
*注：只要能体现出父子关系就可以，不一定非要用标签表示，也可以用标签所对应的class或者id来表示父子关系*

> ![](https://raw.githubusercontent.com/linfeitang/diary/master/Pictures/20190616154624.png?token=AH3FPOF7KT6RLWWEG3PY4PC5AX4TU)

- 直接子元素选择器

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
strong > em{
	background-color: red;
}
```
> ![](https://raw.githubusercontent.com/linfeitang/diary/master/Pictures/20190616160409.jpg?token=AH3FPOBG5IARMJGPYFOKMOK5AX4KK)
