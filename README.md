# slickDome
轮播图切换
1、引入文件

<link rel="stylesheet" href="style/slick.css">
<script src="script/jquery.min.js"></script>
<script src="script/slick.min.js"></script>
2、HTML

<div class="slick">
    <div><a href="http://www.jq22.com"><img src="images/1.jpg" alt=""></a></div>
    <div><a href="http://www.jq22.com"><img src="images/2.jpg" alt=""></a></div>
    <div><a href="http://www.jq22.com"><img src="images/3.jpg" alt=""></a></div>
    <div><a href="http://www.jq22.com"><img src="images/4.jpg" alt=""></a></div>
    <div><a href="http://www.jq22.com"><img src="images/5.jpg" alt=""></a></div>
</div>
3、JavaScript

$(function(){
    $('.slick').slick({
        dots: true
    });
});
参数

accessibility	布尔值	true	启用Tab键和箭头键导航
autoplay	布尔值	false	自动播放
autoplaySpeed	整数	3000	自动播放间隔
centerMode	布尔值	false	中心模式
centerPadding	字符串	’50px’	中心模式左右内边距
cssEase	字符串	‘ease’	CSS3 动画
customPaging	function	n/a	自定义分页
dots	布尔值	false	指示点
draggable	布尔值	true	启用桌面拖动
easing	字符串	‘linear’	animate() fallback easing
fade	布尔值	false	淡入淡出
arrows	布尔值	true	左右箭头
infinite	布尔值	true	循环播放
lazyLoad	字符串	‘ondemand’	延迟加载，可选 ondemand 和 progressive
onBeforeChange(this, index)	method	null	开始切换前的回调函数
onAfterChange(this, index)	method	null	切换后的回调函数
onInit(this)	method	null	第一次初始化后的回调函数
onReInit(this)	method	null	再次初始化后的回调函数
pauseOnHover	布尔值	true	鼠标悬停暂停自动播放
responsive	object	null	断点触发设置
slide	字符串	‘div’	滑动元素查询
slidesToShow	整数	1	幻灯片每屏显示个数
slidesToScroll	整数	1	幻灯片每次滑动个数
x	整数	300	滑动时间
swipe	布尔值	true	移动设备滑动事件
touchMove	布尔值	true	触摸滑动
touchThreshold	整数	5	滑动切换阈值，即滑动多少像素后切换
useCSS	布尔值	true	使用 CSS3 过度
vertical	布尔值	false	垂直方向
方法

slick()	options : object	初始化 slick
unslick()	

销毁 slick
slickNext()	

切换下一张
slickPrev()	

切换上一张
slickPause()	

暂停自动播放
slickPlay()	

开始自动播放
slickGoTo()	index : int	切换到第 x 张
slickCurrentSlide()	

返回当前幻灯片索引
slickAdd()	element : html or DOM object, index: int, addBefore: bool	Add a slide. If an index is provided, will add at that index, or before if addBefore is set. If no index is provided, add to the end or to the beginning if addBefore is set. Accepts HTML String
slideRemove()	index: int, removeBefore: bool	Remove slide by index. If removeBefore is set true, remove slide preceding index, or the first slide if no index is specified. If removeBefore is set to false, remove the slide following index, or the last slide if no index is set.
slickFilter()	filter : selector or function	Filters slides using jQuery .filter syntax
slickUnfilter()	

Removes applied filter
slickSetOption(option,value,refresh)	option : string(option name), value : depends on option, refresh : 布尔值	Sets an option live. Set refresh to true if it is an option that changes the display

