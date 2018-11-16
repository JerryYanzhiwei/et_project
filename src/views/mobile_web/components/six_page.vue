<template>
  <swiper-slide>
    <img class="img_earth" src="../../../assets/img/img_earth.png" alt="">
    <div class="txt_contain">
      <p class="title">我们的愿景:</p>
      <p class="detail">打造区块链最安全, 最高效的生态服务平台</p>
    </div>
    <div class="txt_contain">
      <p class="title">我们的使命:</p>
      <p class="detail">让每个人自由掌控自己的资产</p>
    </div>
    <div class="txt_contain">
      <p class="title">价值观:</p>
      <p class="detail">开源开放 共享未来 安全至上</p>
      <p class="detail">追求卓越 专业高效 创造价值</p>
    </div>
  </swiper-slide>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .swiper-slide {
    .img_earth {
      padding-top: 1rem;
      width: 3.5rem;
    }
    .txt_contain{
      margin-top: 0.2rem;
      &:first-child {
        margin: 0;
      }
      .title {
        font-size: .4rem;
      }
      .detail {
        margin-top: .1rem;
        font-size: 12px;
      }
    }
  }
</style>
