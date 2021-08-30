<template>
  <div  style="background-color: #454545; width:100%;height:100%">
<div id='login' class="whole">
  <h1 >账号: <input name="userId" id="userId" type="text" placeholder="请输入你的账号"></h1>
  <h1 >密码: <input name="userPwd" id="userPwd" type="password" placeholder="请输入密码"></h1>
  <button  v-on:click="match_Pwd" style="display:block;margin:0 auto">登录</button>
</div>
  </div>
</template>

<script>
// defineComponent最重要的是：在TypeScript下，给予了组件 正确的参数类型推断 。
import { defineComponent } from 'vue'
import studentIndex from '@/components/studentEnd/studentIndex'

export default defineComponent({
  name: 'L',
  data () {
    return {
      inform: '请登陆'
    }
  },
  methods: {
    match_Pwd () {
      return (-1)
    }
  },
  components: {
  }
})
</script>

<style scoped>
h1{
  color:#454545;
  text-align: center;
  left:20%;
  top: 30%;
}
.whole{
  border:solid 5px #454545;
  border-radius:20px;
  -moz-border-radius:20px;
  padding:20px;
  margin:0 auto auto auto;
  width:350px;
  height:250px;
  clear:both;
  background-color: #E4E4E4;
  position:absolute;
  left:30%;
  top:30%;
}
</style>
