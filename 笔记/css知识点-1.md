#### display : block inline
 1. 设置ul 的li为inline,可设计水平菜单
 2. 设置max-width，能更好的适应小窗口(包括ie7)
####  盒模型
 1. 块元素水平居中 margin : 0 auto;
 2. 当你设置一个元素为 box-sizing: border-box; 时，此元素的内边距和边框不再会增加它的宽度。(支持ie8),可以给所用元素都加上* {-webkit-box-sizing: border-box;-moz-box-sizing: border-box;box-sizing: border-box;},能确保表现一致
#### position
	1. static 默认
	2. relative:在一个相对定位（position属性的值为relative）的元素上设置 top 、 right 、 bottom 和 left 属性会使其偏离其正常位置。其他的元素的位置则不会受该元素的影响发生位置改变来弥补它偏离后剩下的空隙。
	3. fixed:相对于浏览器视窗定位
	4. absolute:相对于父元素进行定位,父元素要设置position:relative
#### float
	1. clear属性被用于控制浮动,用于未被浮动的元素,有 left right both三种值
	2. overflow:(浮动元素高于父元素)auto被用于清除浮动,支持ie6要加上zoom: 1;
#### 百分比宽度

#### 媒体查询 能实现响应式布局
  移动端自适应:<meta name="viewport" content="width=320, initial-scale=0.5">

#### 创建很多网格
   1. 使用float,
   2. 使用display:inline-block;ie6,7需要特殊写法 <a href="https://blog.mozilla.org/webdev/2009/02/20/cross-browser-inline-block/"></a>
     *. 注意事项:vertical-align 属性会影响到 inline-block 元素，你可能会把它的值设置为 top 。
        你需要设置每一列的宽度。
        如果HTML源代码中元素之间有空格，那么列与列之间会产生空隙。

#### flex布局
    * 实现水平垂直居中
    	.vertical-container {
  		height: 300px;
  		display: -webkit-flex;
  		display:         flex;
  		-webkit-align-items: center;
         align-items: center;
  		-webkit-justify-content: center;
         justify-content: center;}

 
