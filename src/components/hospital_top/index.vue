<template>
  <div class="top">
    <div class="content">
      <div class="left" @click="gohome">
        <img src="@/static/images/logo.png" alt="" >
        <p>尚医通 预约挂号统一平台</p>
      </div>
      <div class="right">
        <p class="help">帮助中心</p>
        <p class="login">登录/注册</p>
    </div>
  </div>
  </div>
</template>
<script setup lang="ts">
import{useRouter} from "vue-router";
const router = useRouter();
function gohome(){
  router.push({path:'/home'});
}
</script>
<style scoped lang="scss">
.top{
  position: fixed;
  z-index: 999;
  width: 100%;
  background-color: #ffffff;
  display: flex;
  justify-content: center;
  .content{
    width:1200px;
    height:70px;
    background-color: #ffffff;
    display: flex;
    justify-content: space-between;
    .left{
      display: flex;
      justify-content: center;
      align-items:center ;
      img{
        width:50px;
        height:50px;
        margin: 10px;
      }
      p{
        font-size: 20px;
        color: skyblue;
      }
    }
    .right{
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 14px;
      color:#bbb;
      .help{
        margin-right: 10px;
      }
    }
  }
}

</style>