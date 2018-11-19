<template>
  <div class="main_contain">
    <public-header v-on:change="changeSlide" v-on:showState="changeIndex"></public-header>
    <swiper ref="myswiper" :options="swiperOption">
      <first-page></first-page>
      <SecondPage></SecondPage>
      <ThreePage></ThreePage>
      <four-page></four-page>
      <FivePage></FivePage>
      <SixPage></SixPage>
      <SevenPage></SevenPage>
    </swiper>
    <public-footer :homeState=homeState></public-footer>
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
    let that = this
    return {
      homeState: 0,
      swiperOption: {
        direction: 'vertical',
        slidesPerView: 1,
        spaceBetween: 0,
        mousewheel: true,
        on: {
          init: function () {
            this.realIndex === 0 && (that.homeState = 0)
          },
          slideChange: function () {
            that.homeState = this.realIndex
            console.log(that.homeState)
          }
        }
      }
    }
  },
  computed: {
    swiper () {
      return this.$refs.myswiper.swiper
    }
  },
  methods: {
    changeSlide (index) {
      this.swiper.slideTo(index)
    },
    changeIndex (state) {
      console.log(state)
      if (state) {
        document.getElementsByClassName('swiper-container')[0].style.zIndex = -1
      } else {
        document.getElementsByClassName('swiper-container')[0].style.zIndex = 9999
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
  .main_contain .swiper-container {
    -webkit-tap-highlight-color:transparent;
  }
  .swiper-container {
      // z-index: -1;
    &.showNav {
      z-index: -1;
    }
  }
}
</style>
