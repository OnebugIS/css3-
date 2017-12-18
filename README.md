# css3-
对于css3常用的标签使用范围总结

元素垂直水平居中

1：行内块元素  display:inline-block
  父元素加：text-align:center
  特性：兼容性较好 父子的宽度都要已知
2：div.box{
  weight:200px;
  height:400px;
  <!--把元素变成定位元素-->
  position:absolute;
  <!--设置元素的定位位置，距离上、左都为50%-->
  left:50%;
  top:50%;
  <!--设置元素的相对于自身的偏移度为负50%(也就是元素自身尺寸的一半)-->
  transform:translate(-50%,-50%);
  }
3：div.box{
  weight:200px;
  height:400px;
  <!--把元素变成定位元素-->
  position:absolute;
  <!--设置元素的定位位置，距离上、下、左、右都为0-->
  left:0;
  right:0;
  top:0;
  bottom:0;
  <!--设置元素的margin样式值为 auto-->
  margin:auto;
  }
4：
center {
	width: 960px;
	margin-left: auto;
	margin-right: auto;
}
5:
 justify-content:center;
 align-items:center;
兼容性较好，缺点:不支持IE7以下的浏览器
 6.父:display:realtive
  子：transform:translate(-50%,-50%)
【此坑待填 敬请关注!!!】
