<template>
  <div class="footer_contain">
    <img class="down_arror" src="../../../assets/img/down_arror.png" alt="">
    <div class="img_contain">
      <img src="../../../assets/img/Email.png" alt="">
      <img src="../../../assets/img/Facebook.png" alt="">
      <img src="../../../assets/img/Twitter.png" alt="">
      <img src="../../../assets/img/WeChat.png" alt="">
      <img src="../../../assets/img/Weibo.png" alt="">
    </div>
    <p>Copyright  ©  2018  EosToken, All rights reserved</p>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .footer_contain {
    text-align: center;
    width: 100%;
    position: fixed;
    bottom: 3%;
    left: 0;
    .down_arror{
      width: 5%;
      height: auto;
    }
    .img_contain {
      width: 100%;
      margin-top: .3rem;
      img {
        width: auto;
        height: 10px;
        margin-left: 10%;
        &:first-child {
          margin: 0;
        }
      }
    }
    p {
      font-size: 12px;
      color: #ccc;
      margin-top: 5%;
    }
  }
</style>
