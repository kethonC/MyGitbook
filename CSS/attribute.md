##### box-sizing
+ content-box  是默认值。
如果你设置一个元素的宽为100px，那么这个元素的内容区会有100px宽，并且任何边框和内边距的宽度都会被增加到最后绘制出来的元素宽度中。  
+ border-box 告诉浏览器去理解你设置的边框和内边距的值是包含在width内的。
也就是说，如果你将一个元素的width设为100px,那么这100px会包含其它的border和padding，内容区的实际宽度会是width减去border + padding的计算值。大多数情况下这使得我们更容易的去设定一个元素的宽高。  

##### outline
+  outline 是针对链接、表单控件和ImageMap等元素设计。outline 的效果将随元素的 focus 而自动出现，相应的由 blur 而自动消失。这些都是浏览器的默认行为，无需JavaScript配合CSS来控制。

##### text-decoration
值|描述|
---|:--:
none | 默认。定义标准的文本。
underline| 定义文本下的一条线。
overline| 定义文本上的一条线。
line-through |定义穿过文本下的一条线。
blink |定义闪烁的文本。
inherit| 规定应该从父元素继承 text-decoration 属性的值。

##### display和visibility
+ 当visibility被设置为"hidden"的时候，元素虽然被隐藏了，但它仍然占据它原来所在的位置。

##### inline-block 
+ 就是不独占一行的块级元素。  

#####  vertical-align 
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

##### list-style
> 该属性是一个简写属性，涵盖了所有其他列表样式属性。由于它应用到所有 display 为 list-item 的元素，所以在普通的 HTML 和 XHTML 中只能用于 li 元素，不过实际上它可以应用到任何元素，并由 list-item 元素继承。
可以按顺序设置如下属性：
>+ list-style-type
>+ list-style-position
>+ list-style-image

##### border-collapse
> border-collapse 属性设置表格的边框是否被合并为一个单一的边框

值|描述|
---|:--:
separate |	默认值。边框会被分开。不会忽略 border-spacing 和 empty-cells 属性。
collapse |	如果可能，边框会合并为一个单一的边框。会忽略 border-spacing 和 empty-cells 属性。
inherit |	规定应该从父元素继承 border-collapse 属性的值。
+ border-spacing 属性设置相邻单元格的边框间的距离（仅用于“边框分离”模式）。
