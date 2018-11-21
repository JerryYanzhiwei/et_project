<template>
  <swiper-slide>
    <div class="img_contain">
      <a>
        <img src="../../../assets/img/img_1.png" alt="">
      </a>
      <a>
        <img src="../../../assets/img/img_2.png" alt="">
      </a>
      <a>
        <img src="../../../assets/img/img_3.png" alt="">
      </a>
      <a>
        <img src="../../../assets/img/img_4.png" alt="">
      </a>
      <a>
        <img src="../../../assets/img/img_5.png" alt="">
      </a>
      <a>
        <img src="../../../assets/img/img_6.png" alt="">
      </a>
      <a>
        <img src="../../../assets/img/img_7.png" alt="">
      </a>
      <a>
        <img src="../../../assets/img/img_8.png" alt="">
      </a>
      <a>
        <img src="../../../assets/img/img_9.png" alt="">
      </a>
      <a>
        <img src="../../../assets/img/img_10.png" alt="">
      </a>
      <a>
        <img src="../../../assets/img/img_11.png" alt="">
      </a>
      <a>
        <img src="../../../assets/img/img_12.png" alt="">
      </a>

    </div>
  </swiper-slide>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .swiper-slide {
    display: flex;
    align-items: center;
  }
  .img_contain {
    // padding-top: .6rem;
    // display: flex;
    // justify-content: center;
    // align-items: center;
    margin-top: -.8rem;
    a {
      display: inline-block;
      font-size: 0;
      margin-left: .3rem;
      margin-top: 1.2rem;
      &:nth-child(1) {
        margin-top: 0;
        margin-left: 0;
      }
      &:nth-child(2) {
        margin-top: 0;
      }
      &:nth-child(3) {
        margin-top: 0;
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
    img {
      font-size: 0;
      width: 2rem;
    }
  }
</style>
