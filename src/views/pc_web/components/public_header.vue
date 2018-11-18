<template>
  <div class="header_contain">
    <img class="logo" src="../../../assets/img/logo.png" alt="">
    <ul>
      <li :class="{'hover': curpage == 1}" @click="changeIndex(1)">{{get_txt.home}}</li>
      <li :class="{'hover': curpage == 2}" @click="changeIndex(2)">{{get_txt.highlight}}</li>
      <li :class="{'hover': curpage == 3}" @click="changeIndex(3)">{{get_txt.about_us}}</li>
      <li :class="{'hover': curpage == 4}" @click="changeIndex(4)">{{get_txt.Lingks}}</li>
      <li class="line"></li>
      <li class="zh" @click="select_lang('zh')">{{get_txt.zh}}</li>
      <li class="en" @click="select_lang('en')" >{{get_txt.en}}</li>
    </ul>
  </div>
</template>

<script>
import { setCookie } from '@/utils/cookies.js'
export default {
  data () {
    return {
      curpage: 1
    }
  },
  methods: {
    changeIndex (index) {
      this.curpage = index
    },
    select_lang (lang) {
      setCookie('lang', lang, 365)
      location.reload()
    }
  },
  computed: {
    get_txt () {
      return this.$t('header')
    }
  }
}
</script>

<style lang="scss" scoped>
  .header_contain {
    width: 100%;
    height: 80px;
    display: flex;
    padding: 0 3%;
    z-index: 9999;
    position: fixed;
    top: 0;
    left: 0;
    justify-content: space-between;
    align-items: center;
    .logo{
      width: 60px;
      height: 60px;
    }
    ul {
      display: flex;
      align-items: center;
      li {
        padding: 15px 0;
        border-bottom: 2px solid transparent;
        margin-left: 5vw;
        line-height: 20px;
        font-size: 14px;
        cursor: pointer;
        &:hover {
          border-image: linear-gradient(#3A7FF3,#353CE0) 1 1;
        }
        &.zh, &.en {
          border-image: none;
          margin-left: 2vw;
          font-size: 12px;
        }
        &.hover {
          border-image: linear-gradient(#3A7FF3,#353CE0) 1 1;
        }
        &.line {
          width: 2px;
          border-image: none;
          padding: 0;
          margin-left: 2vw;
          height: 15px;
          background: #e9e9e9;
        }
      }
    }
  }
</style>
