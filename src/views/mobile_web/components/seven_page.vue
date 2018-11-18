<template>
  <swiper-slide>
    <div class="img_contain">
      <img src="../../../assets/img/img_1.png" alt="">
      <img src="../../../assets/img/img_2.png" alt="">
      <img src="../../../assets/img/img_3.png" alt="">
      <img src="../../../assets/img/img_4.png" alt="">
      <img src="../../../assets/img/img_5.png" alt="">
      <img src="../../../assets/img/img_6.png" alt="">
      <img src="../../../assets/img/img_7.png" alt="">
      <img src="../../../assets/img/img_8.png" alt="">
      <img src="../../../assets/img/img_9.png" alt="">
      <img src="../../../assets/img/img_10.png" alt="">
      <img src="../../../assets/img/img_11.png" alt="">
      <img src="../../../assets/img/img_12.png" alt="">
    </div>
  </swiper-slide>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .img_contain {
    padding-top: .6rem;
    img {
      font-size: 0;
      width: 2rem;
      margin-left: .3rem;
      margin-top: 1.2rem;
      &:nth-child(1) {
        margin-left: 0;
      }
      &:nth-child(4) {
        margin-left: 0;
      }
      &:nth-child(7) {
        margin-left: 0;
      }
      &:nth-child(10) {
        margin-left: 0;
      }
    }
  }
</style>
