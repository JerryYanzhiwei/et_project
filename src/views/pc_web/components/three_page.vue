<template>
  <swiper-slide>
    <div class="three_page">
      <div class="txt_contain">
        <p class="main_txt">DApp生态</p>
        <p class="tip_txt">联合数百家DApp开发团队打造DApp超级入口，促进EOS（柚子）生态共建共享。</p>
      </div>
      <div class="img_cointain">
        <img src="../../../assets/img/main_two.png" alt="">
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
    .three_page {
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
