<template>
<div id="studentCourseView">
  <div id="courseChoose">
    <ul class="simpleBar">
    <li @click="courseClicked" v-for="item in courses" v-bind:key="item" style="margin: 10px;border: dashed;cursor: pointer">
    {{item}}
    </li>
    </ul>
  </div>
</div>
</template>

<script>
export default {
  name: 'studentCourseView',
  data () {
    return {
      courses: ['英语一单元一节', '数学第五章--小数乘法', '物理--牛顿第二定律', '英语一单元一节', '数学第五章--小数乘法', '物理--牛顿第二定律']
    }
  },
  methods: {
    courseClicked () {
      this.$router.push('../login')
    }
  }
}
</script>

<style scoped>
.simpleBar{
  list-style-type: none;
}
</style>
