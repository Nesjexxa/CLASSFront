<template>
  <div class="index">
<span id="indexTop" class="indexTop">
<HEAD></HEAD>
</span>
<span id="indexUnder" class="indexUnder">
  <span id="indexLeft" class="indexLeft">
    <indexLeftInfoBar></indexLeftInfoBar>
  </span>
  <span id="indexRight" class="indexRight">
      <studentCourseView></studentCourseView>
  </span>
</span>
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
  min-height: 100vh;
  flex-direction: column;
}

.indexTop,
footer {
  flex: 1;
}

.indexUnder {
  display: flex;
  flex: 1;
}

.indexRight {
  dispay: flex;
  flex: 1;
}

.indexLeft {
  /* 两个边栏的宽度设为12em */
  display: flex;
  flex: 0 0 12em;
  width: 200px;
}

.indexLeft {
  /* 导航放到最左边 */
  order: -1;
}
</style>
