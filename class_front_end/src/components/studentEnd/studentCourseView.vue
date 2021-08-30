<template>
<div id="studentCourseView">
  <ul class="simpleBar">
    <li v-for="item in courses" v-bind:key="item" >{{item}}</li>
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

</style>
