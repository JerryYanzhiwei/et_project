<template>
  <swiper-slide>
    <p class="top_txt">开放开源</p>
    <div class="body">
      <p class="sm_txt">前端后台全部开源，同时支持Android&IOS双平台。</p>
    </div>
    <img class="img_main" src="../../../assets/img/right_main.png" alt="">
  </swiper-slide>
</template>

<script>
export default {

}
</script>

<style lang='scss' scoped>
  .swiper-slide {
    width: 100%;
    height: 100%;
    padding-top: 1rem;
    .top_txt {
      font-size: .4rem;
    }
    .sm_txt {
      font-size: 12px;
      margin-top: .3rem;
    }
    .img_main {
      margin-top: .2rem;
      width: 3rem;
      height: auto;
    }
    .body {
      font-size: 12px;
      height: 10%;
    }
  }
</style>
