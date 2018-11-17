<template>
  <swiper-slide>
    <div class="six_page">
      <div class="txt_contain">
        <div class="txt_area">
          <p class="main_txt">我们的愿景:</p>
          <p class="tip_txt">打造区块链最安全、最高效的生态服务平台</p>
        </div>
        <div class="txt_area">
          <p class="main_txt">我们的使命:</p>
          <p class="tip_txt">让每个人自由掌控自己的资产</p>
        </div>
        <div class="txt_area">
          <p class="main_txt">价值观:</p>
          <p class="tip_txt">开源开放 共享未来 安全至上</p>
          <p class="tip_txt">追求卓越 专业高效 创造价值</p>
        </div>
      </div>
      <div class="img_cointain">
        <img src="../../../assets/img/img_earth.png" alt="">
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
    .six_page {
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
        .txt_area {
          margin-top: 5vh;
          &:first-child {
            margin: 0;
          }
        }
        .main_txt {
          margin-bottom: 8%;
          font-size: 24px;
        }
        .tip_txt1 {
          margin-top: 1.5vh;
        }
        .tip_txt {
          font-size: 12px;
          margin-top: 1vh;
        }
      }
      .img_cointain {
        width: 60%;
        img {
          width: 100%;
          height: auto;
        }
      }
    }
  }
</style>
