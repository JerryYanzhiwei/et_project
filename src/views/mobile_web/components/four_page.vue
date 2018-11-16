<template>
  <swiper-slide>
    <p class="top_txt">行情快讯</p>
    <div class="body">
      <p class="sm_txt">一站式行情快讯，全天候关注行业动态，精确把握资产行情。</p>
    </div>
    <img class="img_main" src="../../../assets/img/main_three.png" alt="">
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
