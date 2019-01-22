<template>
  <div class="login-container">
    <h1 class="title">登陆</h1>
    <el-form :label-position="labelPosition" label-width="80px">
      <el-form-item label="用户名">
        <el-input v-model="username"></el-input>
      </el-form-item>
      <el-form-item label="密码">
        <el-input @keydown.native.enter="login" type="password" v-model="password"></el-input>
      </el-form-item>
      <el-button type="primary" @click="login">登录</el-button>
    </el-form>
  </div>
</template>
<script>
export default {
  data() {
    return {
      labelPosition: "right",
       password:"",
       username:"",

    };
  },
  methods:{
     login(){
         
     }
  }
  
};
</script>


<style lang="less" scoped>
.container{
    width: 500px;
  margin: 100px auto;
  border: 1px solid #ccc;
  border-radius: 10px;
  padding: 30px;
  box-shadow: 0 0 10px #ccc;
}
</style>