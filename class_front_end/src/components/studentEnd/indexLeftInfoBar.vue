<template>
<div id="leftInfoBar">
    <img src='../../assets/headimg.png'>
  <div id="info" class="info">
    <ul>
      <li>姓名:{{name}}</li>
      <li>学号:{{stuID}}</li>
    </ul>
</div>
</div>
</template>

<script>
export default {
  name: 'indexLeftInfoBar',
  data () {
    return {
      name: '张三',
      stuID: 'SA20218888'
    }
  }
}
</script>

<style scoped>

</style>
