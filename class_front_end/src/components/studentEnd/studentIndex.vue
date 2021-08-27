<template>
<div id="indexTop" class="indexTop">
<HEAD></HEAD>
</div>
<div id="indexUnder" class="indexUnder">
  <div id="indexLeft" class="indexLeft">
    <indexLeftInfoBar></indexLeftInfoBar>
  </div>
  <div id="indexRight" class="indexRight">
      <studentCourseView></studentCourseView>
  </div>
</div>
</template>

<script>
import HEAD from './head.vue'
import indexLeftInfoBar from '@/components/studentEnd/indexLeftInfoBar'
import studentCourseView from '@/components/studentEnd/studentCourseView'
export default {
  name: 'studentIndex',
  components: {
    HEAD,
    indexLeftInfoBar,
    studentCourseView
  }
}
</script>

<style scoped>
.indexTop{
  position: relative;
  height: 100px;
}
.indexUnder{
  position: relative;
}
.indexLeft{
  left: 0;
  position:absolute;
  width:40%;
  height: 800px;
  float: left;
  background-color: antiquewhite;
}
.indexRight{
  background-color: darkgoldenrod;
  position:absolute;
  left: 40%;
  width:60%;
  height: 800px;
  float: right;
}
</style>
