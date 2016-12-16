# CSS3盒模型

- **盒模型分类**

1. **W3C标准的盒模型** 

   内盒（元素大小）=`content+padding+border`

   外盒（元素空间尺寸）=`content+padding+border+margin`

   `height`和`width`表示`content`

2. **IE传统盒模型**

   内盒（元素大小）=`content（contain+padding+margin）`

   外盒（元素空间尺寸）=`content+margin`

   `height`和`width`表示`content+padding+border`

- **属性**

  1.`box-sizing`:`content-box`||`border-box`||`inherit`(`content-box`为默认)

  > `content-box`:`height`和`width`表示`content`
  >
  > `border-box`：`height`和`width`表示`content`+`padding`+`border`
  >
  > `inherit`：继承父元素
  >
  > > 兼容性：主流和ie8+

  2.`overflow-x&overflow-y:visible|hidden|scroll|auto|no-display|no-content`(`visible`默认)

  > `visible`:内容溢出
  >
  > `auto`:溢出时自动添加滚动条
  >
  > `hidden`:内容溢出时，溢出内容隐藏，不显示滚动条
  >
  > `scroll`:不管内容有没有溢出，都会出现滚动条
  >
  > `no-display`:内容溢出时，不显示元素，相当于`display：none`
  >
  > `no-content`:内容溢出时，不显示内容，相当于`visibility:hidden`
  >
  > > 兼容：主流和ie6+

  3.`resize:none|both|horizontal|vertical|inherit`(`none`为默认)

  > `none`:用户不能拖动修改元素
  >
  > `both`:可以拖动元素，修改宽高
  >
  > `horizontal`:可以拖动元素，只可以修改宽
  >
  > `vertical`:可以拖动元素，只可以修改高
  >
  > `inherit`:继承父元素
  >
  > > 兼容：ie不行

  4.`outline:outline-color|outline-style|outline-width|outline-offset|inherit`

  > - 元素可以达到border效果，但是不占据实际空间，不影响布局
  > - outline只能全包围，不能单独修改某一边
  >
  > > 兼容：ie8+

- **实战**

  ![样例](C:\Users\Administrator\Desktop\layout.PNG)

  ```html
  <!DOCTYPE html>
  <html lang="en-US">
  <head>
  <meta charset="utf-8">
  <title>ok</title>
  <style>
  *{
  	margin:0;
  	padding:0;
  	box-sizing:border-box;
  }
  .wrapper{
  	width:960px;
  	margin:auto;
  	text-align:center;

  }
  .header{
  	height:100px;
  	padding-bottom:10px;
  	background-color: aqua;
  }
  .sidebar{
  	float:left;
  	width:220px;
  	height: 100px;
  	margin-right:20px;
  	padding-bottom:10px;
  	background-color: aquamarine;
  }
  .content{
  	float:left;
  	height: 100px;
  	width:720px;
  	padding-bottom:10px;
  	background-color: antiquewhite;
  }
  .footer{
  	height:100px;
  	clear:both;
  	background-color: burlywood;
  }
  </style>
  </head>
  <body>
  	<div class="wrapper">
  		<div class="header">header</div>
  		<div class="sidebar">sidebar</div>
  		<div class="content">content</div>
  		<div class="footer">footer</div>
  	</div>
  </body>
  </html>
  ```

  ​

  ​

  ​