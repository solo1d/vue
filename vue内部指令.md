### 目录

- [v-if](#v-if)
- [v-show](#v-show)









## v-if

根据表达式的值在 DOM 中生成或移除一个元素， 销毁或重新渲染。

```vue
<template>
<!-- 当greeting 为true 时 会显示这个标签 -->
	<p v-if="greeting">Hello</p>
<!-- 当 ifPs() 函数返回值 为true 时 会显示这个标签 -->
	<p v-if="ifPs()">Hello</p>
</template>

<script>
	export default {
    data(){
      return {
        greeting:true
      }
    },
    methods:{
      ifPs(){
        return true;
      }
    }
  }
</script>
```

## v-show

显示或隐藏HTML元素，但是已经完成渲染了，会节省很多资源。

```vue
<template>
<!-- 当greeting 为true 时 会显示这个标签 -->
	<p v-if="greeting">Hello</p>
<!-- 当 ifPs() 函数返回值 为true 时 会显示这个标签 -->
	<p v-if="ifPs()">Hello</p>
</template>

<script>
	export default {
    data(){
      return {
        greeting:true
      }
    },
    methods:{
      ifPs(){
        return true;
      }
    }
  }
</script>
```





