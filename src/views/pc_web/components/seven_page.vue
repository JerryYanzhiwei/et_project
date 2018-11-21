<template>
  <swiper-slide>
    <div class="seven_page">
      <ul>
        <li>
          <a>
            <img src="../../../assets/img/img_1.png" alt="">
          </a>
        </li>
        <li>
          <a>
            <img src="../../../assets/img/img_2.png" alt="">
          </a>
        </li>
        <li>
          <a>
            <img src="../../../assets/img/img_3.png" alt="">
          </a>
        </li>
        <li>
          <a>
            <img src="../../../assets/img/img_4.png" alt="">
          </a>
        </li>
        <li>
          <a>
            <img src="../../../assets/img/img_5.png" alt="">
          </a>
        </li>
        <li>
          <a>
            <img src="../../../assets/img/img_6.png" alt="">
          </a>
        </li>
        <li>
          <a>
            <img src="../../../assets/img/img_7.png" alt="">
          </a>
        </li>
        <li>
          <a>
            <img src="../../../assets/img/img_8.png" alt="">
          </a>
        </li>
        <li>
          <a>
            <img src="../../../assets/img/img_9.png" alt="">
          </a>
        </li>
        <li>
          <a>
            <img src="../../../assets/img/img_10.png" alt="">
          </a>
        </li>
        <li>
          <a>
            <img src="../../../assets/img/img_11.png" alt="">
          </a>
        </li>
        <li>
          <a>
            <img src="../../../assets/img/img_12.png" alt="">
          </a>
        </li>
      </ul>
    </div>
  </swiper-slide>
</template>

<script>
export default {
}
</script>

<style lang="scss">
  .swiper-slide {
    .seven_page {
      position: relative;
      z-index: 9999;
      width: 100%;
      height: 100%;
      padding: 0 5vw 0 5vw;
      display: flex;
      justify-content: space-between;
      align-items: center;
      ul {
        li {
          display: inline-block;
          font-size: 0;
          width: 25%;
          margin-top: 12vh;
          a {
            display: inline-block;
          }
          img {
            width: 50%;
            cursor: pointer;
          }
          img:hover {
            opacity: .6;
          }
          &:nth-child(1) {
            margin: 0;
          }
          &:nth-child(2) {
            margin: 0;
          }
          &:nth-child(3) {
            margin: 0;
          }
          &:nth-child(4) {
            margin: 0;
          }
        }
      }
    }
  }
</style>
