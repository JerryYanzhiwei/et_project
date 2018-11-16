<template>
  <swiper-slide>
    <p class="page_title">钱包还是ET开源的好</p>
    <img class="img_main" src="../../../assets/img/first_page_main.png" alt="">
    <div class="link_contain">
      <a>开源地址</a>
      <span>下载EosToken钱包</span>
    </div>
    <div class="btn_contain">
      <img src="../../../assets/img/ios_btn.png" alt="">
      <img src="../../../assets/img/android_btn.png" alt="">
    </div>
  </swiper-slide>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .swiper-slide {
    padding-top: 1.5rem;
    .page_title {
      padding-top: .12rem;
      font-size: .4rem;
    }
    .img_main{
      width: 100%;
      height: auto;
      margin-top: .15rem;
    }
    .link_contain{
      margin-top: .7rem;
      a {
        font-size: 12px;
        color: #3A7FF3;
        margin-right: .5rem;
      }
      span {
        font-size: 12px;
      }
    }
    .btn_contain{
      width: 100%;
      margin-top: .7rem;
      img {
        width: 3rem;
        height: auto;
      }
    }
  }
</style>
