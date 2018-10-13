# CSS总结


### 1. 原子类
``` css?linenums
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
	基于这些原子类，在项目自由、灵活地组合使用，  避免重复书写如：弹性盒布局、容器居中等
	
**缺点**  
- 维护困难  
	在很多个地方用了 .w100 ，如果要将这些宽度改为 150px，就不可避免的导致改动麻烦
- 代码冗余  
	在一个元素上添加好多个 class ，导致HTML代码很长
	
### 2. 组件Css增加嵌套class
```css?linenums
.wrapClass .el{
	display:-webkit-box;
}
```
  
	避免组件样式影响到主体，导致主体增加不必要的清除操作
	
### 3.主入口文件避免引入非主体样式
如：Vue项目中，app.js引入除默认清理样式外，还引入了部分组件的样式		
       小程序的主文件亦然

### 4.针对CSS的默认属性无需重复声明以及排列顺序