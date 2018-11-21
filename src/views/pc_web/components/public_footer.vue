<template>
  <div class="footer_contain">
    <span class="text">Copyright  ©  2018  EosToken, All rights reserved</span>
    <div class="img_contain">
      <img src="../../../assets/img/Email.png" alt="">
      <img src="../../../assets/img/Facebook.png" alt="">
      <img src="../../../assets/img/Twitter.png" alt="">
      <span class='WeChat'>
        <img @click='showQRCode' src="../../../assets/img/WeChat.png" alt="">
        <img v-show='QRCode' class='QR_Code' src="../../../assets/img/QR_Code.jpg" alt="">
      </span>
      <img src="../../../assets/img/Weibo.png" alt="">
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      QRCode: false
    }
  },
  methods: {
    showQRCode () {
      this.QRCode = !this.QRCode
    }
  }
}
</script>

<style lang="scss" scoped>
  .footer_contain {
    z-index: 9999;
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
        cursor: pointer;
        width: auto;
        height: 10px;
        margin-left: 25px;
      }
      img:hover {
        opacity: .5;
      }
    }
    .WeChat{
      position:relative;
      .QR_Code{
        position:absolute;
        top:-490%;
        left:-93%;
        height:80px;
        width:80px;
      }
      .QR_Code:hover{
        opacity: 1;
      }
    }
  }
</style>
