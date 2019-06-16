## 复杂选择器
### 父子选择器/派生选择器
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

> ![](https://raw.githubusercontent.com/linfeitang/diary/master/Pictures/20190616154624.png?token=AH3FPOGSAZFQG2IINEEZ55C5AX5QM)

### 直接子元素选择器
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
可以看到只有直属于div的em才被样式化，而strong下的em没有生效。
>![](https://raw.githubusercontent.com/linfeitang/diary/master/Pictures/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20190616161305.png?token=AH3FPOBTZE7ZH5B3VRABXDS5AX5HI)

### 并列选择器
html代码：实现效果：只让内容456对样式生效
```
<div>123</div>
<div class="demo">456</div>
<p class="demo">789</p>
```
css代码：
```
div.demo{
	background-color: green;
}
```
![](https://raw.githubusercontent.com/linfeitang/diary/master/Pictures/20190616162922.png?token=AH3FPOEOLS7K37WD55MMHVS5AX7F4)