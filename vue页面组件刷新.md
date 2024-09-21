## 目录

- [vue页面组件刷新](#vue页面组件刷新)



## vue页面组件刷新

```vue
<template>
	<button @click="refresButton">
    刷新列表页面
  </button>
	<table v-if="tableShowFlage">
    <tr>
  	   <th>硬件名称</th>
	  </tr>
    <tr>
      <td>数据成员</td>
  	</tr>
  </table>
</template>
<script>
export default {
  data(){
    return {
      // 默认显示列表
      tableShowFlage:true,
    }
  },
  methods:{
    refresButton(){
        // 通过 nextTick() 方法，在 DOM 更新之后再执行代码
      // tableShowFlage 是 v-if 绑定的
      this.tableShowFlage = false
      this.$nextTick(() => {
        this.tableShowFlage = true
      })
    }
  }
}
</script>
```

