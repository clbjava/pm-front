<template>
  <div id="login">
    <input type="text" v-model="username">
    <input type="password" v-model="password">
    <input type="button" value="登录" v-on:click="loginActive()">
  </div>
</template>

<script>
    export default {
      name: "login",
      data () {
        return {
          username: 'Welcome to Your Vue.js App',
          password:"******"
        }
      },
      // 点击菜单使用的函数
      methods: {
        loginActive: function(){
         var string= this.username+this.password;
         alert(string);
        }
      }
    }
</script>

<style scoped>

</style>
