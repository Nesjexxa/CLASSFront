<template>
<div id="studentCourseView" class="studentCourseView">
  <ul>
    <li v-for="item in courses" v-bind:key="item">
      <label>{{item}}</label>
    </li>
  </ul>
</div>
</template>

<script>
export default {
  name: 'studentCourseView',
  data () {
    return {
      courses: ['英语一单元一节', '数学第五章--小数乘法', '物理--牛顿第二定律']
    }
  }
}
</script>

<style scoped>
studentCourseView{
  text-align: left;
  position: absolute;
  top:10%;
  background-color: darkgoldenrod;
  width:100%;
  height:800px;
}
</style>
