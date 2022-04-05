<!-- 用来写组件的结构    安装vetur组件，
并打开文件--首选项--设置中搜索Vetur，拉到最底部，把这三块的勾去掉。vetur.validation.template等-->
<template>
  <div class="demo">
    <h2>学校名称：{{ name }}</h2>
    <h2>学校地址：{{ address }}</h2>
    <button @click='schoolName'>点我提示学校名字</button>
  </div>
</template>
 

<script>
//用来写组件交互相关的代码(数据、方法等)
export default {
    name:'MySchool',
  data(){
    return {
      name: "山东拐大",
      address:'嘉里敦',
    };
  },
  methods: {
    showName() {
      alert(this.schoolName);
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