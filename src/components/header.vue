<template>
  <header v-if="!isLogin">
    <template>
      <h1>Let's share</h1>
      <p>精品博客汇聚</p>
      <div class="btns">
        <el-button>立即登录</el-button>
        <el-button>注册账号</el-button>
      </div>
    </template>
    <template>
      <h1>Let's share</h1>
      <i class="edit el-icon-edit"></i>
      <img class="avatar" src="http://cn.gravatar.com/avatar/1?s=128&d=identicon" alt="">
    </template>
  </header>
</template>

<script>

  export default {
    data() {
      return {
        isLogin: true
      }
    }
  }

</script>

<style lang="less">

  @import "../assets/base.less";

  header {
    padding: 0 12% 30px 12%;
    background: @bgColor;
    display: grid;
    justify-items: center;

    h1 {
      color: #fff;
      font-size: 40px;
      margin: 60px 0 0 0;
      text-transform: uppercase;
    }

    p {
      margin: 15px 0 0 0;
      color: #fff;
    }

    .btns {
      margin-top: 20px ;
    }
  }

</style>
