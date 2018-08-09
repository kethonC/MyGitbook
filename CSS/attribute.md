<h1>css 属性</h1>


<h2> box-sizing</h2>

+ content-box  是默认值。
如果你设置一个元素的宽为100px，那么这个元素的内容区会有100px宽，并且任何边框和内边距的宽度都会被增加到最后绘制出来的元素宽度中。  
+ border-box 告诉浏览器去理解你设置的边框和内边距的值是包含在width内的。
也就是说，如果你将一个元素的width设为100px,那么这100px会包含其它的border和padding，内容区的实际宽度会是width减去border + padding的计算值。大多数情况下这使得我们更容易的去设定一个元素的宽高。  

<h2> outline</h2>

+  outline 是针对链接、表单控件和ImageMap等元素设计。outline 的效果将随元素的 focus 而自动出现，相应的由 blur 而自动消失。这些都是浏览器的默认行为，无需JavaScript配合CSS来控制。

<h2>text-decoration</h2>

值|描述|
---|:--:
none | 默认。定义标准的文本。
underline| 定义文本下的一条线。
overline| 定义文本上的一条线。
line-through |定义穿过文本下的一条线。
blink |定义闪烁的文本。
inherit| 规定应该从父元素继承 text-decoration 属性的值。


<h2>display和visibility</h2>

+ 当visibility被设置为"hidden"的时候，元素虽然被隐藏了，但它仍然占据它原来所在的位置。

<h2>inline-block </h2>

+ 就是不独占一行的块级元素。  

<h2> vertical-align </h2>

值|描述|
---|:--:
baseline|	默认。元素放置在父元素的基线上。
sub |垂直对齐文本的下标。
super |	垂直对齐文本的上标
top |	把元素的顶端与行中最高元素的顶端对齐
text-top |	把元素的顶端与父元素字体的顶端对齐
middle |	把此元素放置在父元素的中部。
bottom |	把元素的顶端与行中最低的元素的顶端对齐。
text-bottom |	把元素的底端与父元素字体的底端对齐。
length | 	 
% |	使用 "line-height" 属性的百分比值来排列此元素。允许使用负值。
inherit |	规定应该从父元素继承 vertical-align 属性的值。

<h2> list-style</h2>

> 该属性是一个简写属性，涵盖了所有其他列表样式属性。由于它应用到所有 display 为 list-item 的元素，所以在普通的 HTML 和 XHTML 中只能用于 li 元素，不过实际上它可以应用到任何元素，并由 list-item 元素继承。
可以按顺序设置如下属性：
>+ list-style-type
>+ list-style-position
>+ list-style-image

<h2> border-collapse</h2>

> border-collapse 属性设置表格的边框是否被合并为一个单一的边框

值|描述|
---|:--:
separate |	默认值。边框会被分开。不会忽略 border-spacing 和 empty-cells 属性。
collapse |	如果可能，边框会合并为一个单一的边框。会忽略 border-spacing 和 empty-cells 属性。
inherit |	规定应该从父元素继承 border-collapse 属性的值。
+ border-spacing 属性设置相邻单元格的边框间的距离（仅用于“边框分离”模式）。

<h2> display:flex </h2>

[display:flex 布局教程](https://blog.csdn.net/linda_417/article/details/51507176)

> flex-direction属性

+ row（默认值）：主轴为水平方向，起点在左端。
+ row-reverse：主轴为水平方向，起点在右端。
+ column：主轴为垂直方向，起点在上沿。
+ column-reverse：主轴为垂直方向，起点在下沿。

> flex-wrap属性  
默认情况下，项目都排在一条线（又称"轴线"）上。flex-wrap属性定义，如果一条轴线排不下，如何换行。

+ nowrap（默认）：不换行。
+ wrap：换行，第一行在上方。
+ wrap-reverse：换行，第一行在下方。

> flex-flow

+ flex-flow属性是flex-direction属性和flex-wrap属性的简写形式，默认值为row nowrap。

> justify-content属性   

justify-content属性定义了项目在主轴上的对齐方式。
+ flex-start（默认值）：左对齐
+ flex-end：右对齐
+ center： 居中
+ space-between：两端对齐，项目之间的间隔都相等。
+ space-around：每个项目两侧的间隔相等。所以，项目之间的间隔比项目与边框的间隔大一倍。

> align-items属性  

align-items属性定义项目在交叉轴上如何对齐
+ flex-start：交叉轴的起点对齐。
+ flex-end：交叉轴的终点对齐。
+ center：交叉轴的中点对齐。
+ baseline: 项目的第一行文字的基线对齐。
+ stretch（默认值）：如果项目未设置高度或设为auto，将占满整个容器的高度。

> align-content属性  

align-content属性定义了多根轴线的对齐方式。如果项目只有一根轴线，该属性不起作用。
+ flex-start：与交叉轴的起点对齐。
+ flex-end：与交叉轴的终点对齐。
+ center：与交叉轴的中点对齐。
+ space-between：与交叉轴两端对齐，轴线之间的间隔平均分布。
+ space-around：每根轴线两侧的间隔都相等。所以，轴线之间的间隔比轴线与边框的间隔大一倍。
+ stretch（默认值）：轴线占满整个交叉轴。

<h2>transform</h2>

transform 属性向元素应用 2D 或 3D 转换。该属性允许我们对元素进行旋转、缩放、移动或倾斜。

值|描述|
---|:--:
none |	定义不进行转换。	
matrix(n,n,n,n,n,n) |	定义 2D 转换，使用六个值的矩阵。	
matrix3d(n,n,n,n,n,n,n,n,n,n,n,n,n,n,n,n) |	定义 3D 转换，使用 16 个值的 4x4 矩阵。	
translate(x,y) |	定义 2D 转换。	
translate3d(x,y,z) |	定义 3D 转换。	
translateX(x) |	定义转换，只是用 X 轴的值。	
translateY(y) |	定义转换，只是用 Y 轴的值。	
translateZ(z) |	定义 3D 转换，只是用 Z 轴的值。	
scale(x,y) |	定义 2D 缩放转换。	
scale3d(x,y,z) |	定义 3D 缩放转换。	
scaleX(x) |	通过设置 X 轴的值来定义缩放转换。	
scaleY(y) |	通过设置 Y 轴的值来定义缩放转换。	
scaleZ(z) |	通过设置 Z 轴的值来定义 3D 缩放转换。	
rotate(angle) |	定义 2D 旋转，在参数中规定角度。	
rotate3d(x,y,z,angle) |	定义 3D 旋转。	
rotateX(angle) |	定义沿着 X 轴的 3D 旋转。	
rotateY(angle) |	定义沿着 Y 轴的 3D 旋转。	
rotateZ(angle) |	定义沿着 Z 轴的 3D 旋转。	
skew(x-angle,y-angle) |	定义沿着 X 和 Y 轴的 2D 倾斜转换。	
skewX(angle) |	定义沿着 X 轴的 2D 倾斜转换。	
skewY(angle) |	定义沿着 Y 轴的 2D 倾斜转换。	
perspective(n) |	为 3D 转换元素定义透视视图。
