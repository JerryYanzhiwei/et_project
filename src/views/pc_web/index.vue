<template>
  <div class="contain">
    <PublicHeader></PublicHeader>
    <swiper ref="swiper" :options="swiperOption">
      <FirstPage></FirstPage>
      <TwoPage></TwoPage>
      <ThreePage></ThreePage>
      <FourPage></FourPage>
      <FivePage></FivePage>
      <SixPage></SixPage>
      <SevenPage></SevenPage>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
    <PublicFooter></PublicFooter>
  </div>
</template>

<script>
import PublicHeader from './components/public_header.vue'
import PublicFooter from './components/public_footer.vue'
import FirstPage from './components/first_page.vue'
import TwoPage from './components/two_page.vue'
import ThreePage from './components/three_page.vue'
import FourPage from './components/four_page.vue'
import FivePage from './components/five_page.vue'
import SixPage from './components/six_page.vue'
import SevenPage from './components/seven_page.vue'
export default {
  components: {
    PublicHeader,
    PublicFooter,
    FirstPage,
    TwoPage,
    ThreePage,
    FourPage,
    FivePage,
    SixPage,
    SevenPage
  },
  data () {
    return {
      swiperOption: {
        direction: 'vertical',
        slidesPerView: 1,
        spaceBetween: 0,
        mousewheel: true,
        pagination: {
          el: '.swiper-pagination',
          clickable: true
        }
      }
    }
  }
}
</script>

<style lang="scss" scoped>
  .contain {
    width: 100%;
    height: 100%;
    padding: 0 3% 0 3%;
    overflow: hidden;
  }
  .swiper-container,
  .swiper-container-vertical > .swiper-wrapper {
    height: 100%;
  }
</style>
