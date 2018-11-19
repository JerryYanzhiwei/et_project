<template>
  <swiper-slide>
    <div class="first_page">
      <p class="page_title">{{get_txt.txt_title}}</p>
      <img class="main_img" src="../../../assets/img/first_page_main.png" alt="">
      <div class="link_contain">
        <a class="open_address">{{get_txt.source_address}}</a>
        <a class="down_token">{{get_txt.down_address}}</a>
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
  },
  computed: {
    get_txt () {
      return this.$t('first_page')
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
        a.open_address {
          background-image:-webkit-linear-gradient(left,#3A7FF3,#3A7FF3,#353CE0);
          text-decoration: underline!important;
          -webkit-background-clip:text;
          -webkit-text-fill-color:transparent;
          border-bottom: 1px solid #3A7FF3;
          margin-right: 2vw;
          cursor: pointer;
        }
        a.down_token {
          color: #000;
          cursor: pointer;
        }
        a:hover {
          opacity: .5;
        }
      }
      .btn_contain {
        margin-top: 3vh;
        img {
          cursor: pointer;
          width: 12vw;
          // height: 8vh;
          margin-left: 1vw;
          &:first-child {
            margin: 0;
          }
        }
      }
    }
  }
</style>
