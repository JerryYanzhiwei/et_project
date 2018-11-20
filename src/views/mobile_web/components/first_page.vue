<template>
  <swiper-slide>
    <p class="page_title">{{get_txt.txt_title}}</p>
    <img class="img_main" src="../../../assets/img/first_page_main.png" alt="">
    <div class="link_contain">
      <a>{{get_txt.source_address}}</a>
      <span>{{get_txt.down_address}}</span>
    </div>
    <div class="btn_contain">
      <img src="../../../assets/img/ios_btn.png" alt="">
      <img src="../../../assets/img/android_btn.png" alt="">
    </div>
  </swiper-slide>
</template>

<script>
export default {
  computed: {
    get_txt () {
      return this.$t('first_page')
    }
  }
}
</script>

<style lang="scss" scoped>
  .swiper-slide {
    // padding-top: 1.5rem;
    display: flex;
    width: 100%;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    .page_title {
      padding-top: .12rem;
      font-size: .4rem;
    }
    .img_main{
      width: 100%;
      height: auto;
      margin-top: .5rem;
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
