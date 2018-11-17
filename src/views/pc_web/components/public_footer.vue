<template>
  <div class="footer_contain">
    <span class="text">Copyright  ©  2018  EosToken, All rights reserved</span>
    <div class="img_contain">
      <img src="../../../assets/img/Email.png" alt="">
      <img src="../../../assets/img/Facebook.png" alt="">
      <img src="../../../assets/img/Twitter.png" alt="">
      <img src="../../../assets/img/WeChat.png" alt="">
      <img src="../../../assets/img/Weibo.png" alt="">
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .footer_contain {
    width: 100%;
    height: 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0% 3% 2% 3%;
    position: fixed;
    bottom: 0;
    left: 0;
    .text {
      color: #ccc;
    }
    .img_contain {
      height: 100%;
      img {
        width: auto;
        height: 10px;
        margin-left: 25px;
      }
    }
  }
</style>
