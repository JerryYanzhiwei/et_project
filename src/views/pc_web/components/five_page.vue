<template>
  <swiper-slide>
    <div class="five_page">
      <div class="txt_contain">
        <p class="main_txt">内置交易所</p>
        <p class="tip_txt">ET交易所是全球首个倡导完全去中心化的分布式交易所，旨在建立一个高效、透明的</p>
        <p class="tip_txt1">符合区块链精神的资产交易平台，ET交易所接口对所有钱包开放</p>
      </div>
      <div class="img_cointain">
        <img src="../../../assets/img/main_four.png" alt="">
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
    .five_page {
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
        .tip_txt1 {
          margin-top: 1.5vh;
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
