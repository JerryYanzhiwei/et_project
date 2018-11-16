<template>
  <swiper-slide>
    <p class="top_txt">内置交易所</p>
    <div class="body">
      <p class="sm_txt">ET交易所是全球首个倡导完全去中心化的分布式交易所，旨在建立一个高效、透明的符合区块链精神的资产交易平台，ET交易所接口对所有钱包开放。</p>
    </div>
    <img class="img_main" src="../../../assets/img/main_four.png" alt="">
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
    padding-top: .8rem;
    .top_txt {
      font-size: .4rem;
    }
    .sm_txt {
      font-size: 12px;
      margin-top: .2rem;
      padding: 0 2%;
    }
    .sm_txt_a {
      font-size: 12px;
      margin-top: .1rem;
    }
    .img_main {
      margin-top: .4rem;
      width: 3rem;
      height: auto;
    }
    .body {
      font-size: 12px;
      height: 10%;
    }
  }
</style>
