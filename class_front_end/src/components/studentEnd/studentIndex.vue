<template>
  <div class="index">
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

.index {
  display: flex;
  flex-direction: column;
}

.indexTop{
  flex:1;
  height: 3px;
}

.indexUnder {
  display: flex;
  flex: 1;
  height: 500px;
  border: outset;
  border-color: #42b983;
}

.indexRight {
  flex: 1;
  border: outset;
  border-color: #42b983;
}

.indexLeft {
  flex: 0 0 12em;
  width: 200px;
}

.indexLeft {
  /* 导航放到最左边 */
  order: -1;
}
</style>
