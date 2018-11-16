<template>
  <div class="main_contain">
    <public-header></public-header>
    <swiper ref="swiper" :options="swiperOption">
      <first-page></first-page>
      <swiper-slide>2</swiper-slide>
      <swiper-slide>3</swiper-slide>
    </swiper>
    <public-footer></public-footer>
  </div>
</template>

<script>
import PublicHeader from './components/public_header.vue'
import FirstPage from './components/first_page'
import PublicFooter from './components/public_footer'
export default {
  components: {
    PublicHeader,
    FirstPage,
    PublicFooter
  },
  data () {
    // let data = this
    return {
      swiperOption: {
        direction: 'vertical',
        slidesPerView: 1,
        spaceBetween: 0,
        mousewheel: true
      }
    }
  }
}
</script>

<style lang="scss" type="text/css">
.main_contain {
  width: 100%;
  height: 100%;
  padding: 5% 5%;
  .swiper-container {
    width: 100%;
    height: 70%;
    overflow: hidden;
    // background-color: #eee;
    .swiper-slide{
      width: 100%;
      height: 100%;
    }
  }
  .swiper-container-vertical > .swiper-wrapper {
    height: 100%;
  }
}
</style>
