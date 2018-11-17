<template>
  <swiper-slide>
    <div class="first_page">
      <p class="page_title">钱包还是ET开源的好</p>
      <img class="main_img" src="../../../assets/img/first_page_main.png" alt="">
      <div class="link_contain">
        <a>开源地址</a>
        <span>下载EosToken</span>
      </div>
      <div class="btn_contain">
        <img @mouseover="show_ios = hov_ios" @mouseout="show_ios = nor_ios" :src="show_ios" alt="">
        <img @mouseover="show_and = hov_and" @mouseout="show_and = nor_and" :src="show_and" alt="">
      </div>
    </div>
  </swiper-slide>
</template>

<script>
export default {
  data () {
    return {
      show_ios: require('../../../assets/img/ios_btn.png'),
      show_and: require('../../../assets/img/ios_btn.png'),
      nor_ios: require('../../../assets/img/ios_btn.png'),
      hov_ios: require('../../../assets/img/hover_ios_btn.png'),
      nor_and: require('../../../assets/img/android_btn.png'),
      hov_and: require('../../../assets/img/hover_android_btn.png')
    }
  }
}
</script>

<style lang="scss">
  .swiper-slide {
    .first_page {
      padding-top: 20vh;
      .page_title {
        font-size: 30px;
      }
      .main_img{
        margin-top: 2vh;
        width: 40%;
        height: auto;
      }
      .link_contain {
        font-size: 12px;
        margin-top: 3vh;
        a {
          background-image:-webkit-linear-gradient(left,#3A7FF3,#3A7FF3,#353CE0);
          text-decoration: underline!important;
          -webkit-background-clip:text;
          -webkit-text-fill-color:transparent;
          border-bottom: 1px solid #3A7FF3;
          margin-right: 2vw;
        }
      }
      .btn_contain {
        margin-top: 3vh;
        img {
          cursor: pointer;
          width: 13%;
          height: auto;
          margin-left: 1vw;
          &:first-child {
            margin: 0;
          }
        }
      }
    }
  }
</style>
