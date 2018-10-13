### 原子类
``` css
/*文字排版*/  
.f12{font-size:12px;}  
.f20{font-size:20px;}  
.fb{font-weight:bold}  
.fn{font-weight:normal;}  
.t2{text-indent:2em;}  
.lh150{line-height:150%;}  
.unl{text-decoration:underlline;}
.no_unl{text-decoration:none;}  
  
/*定位*/  
.tl{text-align:left;}  
.tc{text-align:center;}  
.tr{text-align:right;}  
.bc{margin-left:0;margin-right:0;}  
.fl{float:left;display:inline;}  
.fr{float:right;display:inline;}  
.cb{clear:both;}  
.cl{clear:left;}  
.cr{clear:rigth;}  
.vm{verticle-align:middle;}
.abs-right{position:absolute;right:0}  
.zoom{zoom:1;}  
.hidden{visiility:hidden;}  
.none{display:none;}  
```
**优点**  
	基于这些原子类，我们可以在项目中非常自由、灵活地组合使用，好处就是几乎不怎么需要你再写 CSS 代码了。  
**缺点**  
- 维护困难  
	试想，当你在很多个地方用了 .w100 ，如果要将这些宽度改为 150px，怎么做？  
- 代码冗余  
	经常会出现这样一种情况，在一个元素上添加好多个 class ，导致HTML代码很长。如很简单的一个按钮：  