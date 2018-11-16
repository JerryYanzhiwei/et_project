<template>
  <div class="main_contain">
    <public-header></public-header>
    <swiper ref="swiper" :options="swiperOption">
      <first-page></first-page>
      <SecondPage></SecondPage>
      <ThreePage></ThreePage>
      <four-page></four-page>
      <FivePage></FivePage>
      <SixPage></SixPage>
      <SevenPage></SevenPage>
    </swiper>
    <public-footer></public-footer>
  </div>
</template>

<script>
import PublicHeader from './components/public_header.vue'
import FirstPage from './components/first_page'
import SecondPage from './components/second_page'
import ThreePage from './components/three_page'
import FourPage from './components/four_page'
import FivePage from './components/five_page'
import SixPage from './components/six_page'
import SevenPage from './components/seven_page'
import PublicFooter from './components/public_footer'
export default {
  components: {
    PublicHeader,
    FirstPage,
    SecondPage,
    ThreePage,
    FourPage,
    FivePage,
    SixPage,
    SevenPage,
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
    height: 100%;
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
