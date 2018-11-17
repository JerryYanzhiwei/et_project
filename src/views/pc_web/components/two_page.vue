<template>
  <swiper-slide>
    <div class="two_page">
      <div class="txt_contain">
        <p class="main_txt">开放开源</p>
        <p class="tip_txt">前端后台全部开源, 同事支持Android&IOS双平台</p>
      </div>
      <div class="img_cointain">
        <img src="../../../assets/img/right_main.png" alt="">
      </div>
    </div>
  </swiper-slide>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  .swiper-slide {
    .two_page {
      width: 100%;
      height: 100%;
      padding: 0 5vw 0 5vw;
      display: flex;
      justify-content: space-between;
      align-items: center;
      .txt_contain{
        padding-left: 3%;
        width: 50%;
        text-align: left;
        p {
          font-size: 12px;
        }
        .main_txt {
          margin-bottom: 8%;
          font-size: 24px;
        }
      }
      .img_cointain {
        width: 50%;
        img {
          width: 40%;
          height: auto;
        }
      }
    }
  }
</style>
