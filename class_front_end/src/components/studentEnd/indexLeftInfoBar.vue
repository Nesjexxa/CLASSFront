<template>
<div id="leftInfoBar" class="leftInfoBar">
    <img src='../../assets/headimg.png' class="headImag">
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
.leftInfoBar{
  position: relative;
  top: 10%;
  left: 0%;
  width: 88%;
  height:600px;
  background-color: cornflowerblue;
}
.headImag{
  position: absolute;
  left:40%;
  top: 20%;
  height: 90px;
  width: 90px;
  border-radius: 50%;
  overflow: hidden;
}
.info{
  text-decoration: underline;
  text-align: left;
  font-size: 24px;
  border:solid 2px cornflowerblue;
  border-radius:20px;
  -moz-border-radius:20px;
  padding:20px;
  margin:0 auto auto auto;
  width:80%;
  height:250px;
  clear:both;
  background-color: cornflowerblue;
  position:absolute;
  left:5%;
  top:50%;
}
</style>
