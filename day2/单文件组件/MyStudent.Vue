<!-- 用来写组件的结构 -->
<template>
  <div class="demo">
    <h2>学生名称：{{ name }}</h2>
    <h2>学上年龄地址：{{ age }}</h2>
    <button @click='showName'>点我提示学生名字</button>
  </div>
</template>
 

<script>
//用来写组件交互相关的代码(数据、方法等)
export default {
    name:'MyStudent',
  data(){
    return {
      name: "拐子",
      age:20,
    };
  },
  methods: {
    showName() {
      alert(this.studentName);
    },
  },
};
</script>

<style>
/* 用来写组件的样式的 */
.demo {
  background-color: orange;
}
</style>