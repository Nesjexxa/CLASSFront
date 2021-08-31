<template>
<div id="leftInfoBar">
    <img id="headImg" src='../../assets/headimg.png'>
  <div id="info" class="info">
    <ul>
      <li>姓名:{{name}}</li>
      <li>学号:{{stuID}}</li>
    </ul>
</div>
  <button style="margin: auto" @click="rebackClicked">返回</button>
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
  },
  methods: {
    rebackClicked () {
      this.$router.push('../login')
    }
  }
}
</script>

<style scoped>
#headImg{
  height: 50px;
  width: 50px;
  border-radius: 25%;
  margin: auto;
}
#leftInfoBar{
  display: flex;
  flex-direction: column;
  text-align: left;
}
#info{
  display: flex;
  flex-direction: column;
}
</style>
