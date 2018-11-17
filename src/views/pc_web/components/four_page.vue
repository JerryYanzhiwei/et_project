<template>
  <swiper-slide>
    <div class="four_page">
      <div class="txt_contain">
        <p class="main_txt">行情快讯</p>
        <p class="tip_txt">一站式行情快讯, 全天候关注行业动态, 精确把握资产行情。</p>
      </div>
      <div class="img_cointain">
        <img src="../../../assets/img/main_three.png" alt="">
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
    .four_page {
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
