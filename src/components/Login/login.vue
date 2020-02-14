<template>
  <div class="wrap"> 
    <el-form label-position="top" label-width="80px" :model="formLabelAlign" class="loginfrom">
      <h3>用户登录</h3>
      <el-form-item label="用户名">
        <el-input v-model="formLabelAlign.username"></el-input>
      </el-form-item>
      <el-form-item label="密码">
        <el-input v-model="formLabelAlign.password"></el-input>
      </el-form-item>
      <el-button type="primary" class="loginbtn">登录</el-button>
    </el-form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      formLabelAlign: {
        username: "",
        password: ""
      }
    };
  }
};
</script>

<style>
.wrap{
    background-color: aquamarine;
    height:100%;
    display: flex;
    justify-content: center;
    align-items: center;
}
.wrap .loginfrom{
    width:400px;
    background-color: #fff;
    padding:30px;

}
.wrap .loginbtn{
    width:100%;
}
</style>
