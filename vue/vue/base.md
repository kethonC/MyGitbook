<h1>基础知识</h1>

<h2>$emit</h2>

1、父组件可以使用 props 把数据传给子组件。  
2、子组件可以使用 $emit 触发父组件的自定义事件。  

vm.$emit( event, arg ) //触发当前实例上的事件  

vm.$on( event, fn );//监听event事件后运行 fn;

<h2>class</h2>

```
:class="{'item-selected':item.selected}"
```

<h2>v-for</h2>

```javascript
<div v-for="(index, item) in items"></div>
```

<h2>watch 对象</h2>

```javascript
    obj: {
      handler: function(val, oldVal){
          
      },
      deep: true,
      immediate:true,
    },
```

