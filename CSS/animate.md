<h1>动画</h1>

<h2>animate属性</h2>

animation 属性是一个简写属性，用于设置六个动画属性：

值|描述|
---|:--:
animation-name |	规定需要绑定到选择器的 keyframe 名称。。
animation-duration |	规定完成动画所花费的时间，以秒或毫秒计。 
animation-timing-function |	规定动画的速度曲线。
animation-delay |	规定在动画开始之前的延迟。
animation-iteration-count |	规定动画应该播放的次数。
animation-direction |	规定是否应该轮流反向播放动画。

> animation-timing-function

值|描述|
---|:--:
linear | 动画从头到尾的速度是相同的。	
ease |	默认。动画以低速开始，然后加快，在结束前变慢。	
ease-in |	动画以低速开始。	
ease-out |	动画以低速结束。	
ease-in-out |	动画以低速开始和结束。	
cubic-bezier(n,n,n,n) |	在 cubic-bezier 函数中自己的值。可能的值是从 0 到 1 的数值。

> animation-direction

值|描述|
---|:--:
normal |	默认值。动画应该正常播放。
alternate |	动画应该轮流反向播放。	

