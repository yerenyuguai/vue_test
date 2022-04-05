<!--      安装vetur插件后  输入  <v   就可以快熟生成模板-->
<template>
<div>
    <MySchool></MySchool>
    <MyStudent></MyStudent>
</div>
</template>

<script>
//引入组件
import MySchool from '../';
import MyStudent from './Student.Vue';
export default {
    name:'App',
    components:{
        MySchool,
        MyStudent
    }
}
</script>

<style>

</style>