<template>
  <div class="header_contain">
    <img class="logo_contain" src="../../../assets/img/logo.png" alt="">
    <img class="menu_contain" src="../../../assets/img/icon_menu.png" alt="">
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.header_contain {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 10%;
  display: flex;
  justify-content: space-between;
  .logo_contain {
    width: 1.5rem;
    height: 1.5rem;
  }
  .menu_contain {
    width: 8%;
    height: 30%;
    margin-top: 3%;
    margin-right: 3%;
  }
}
</style>
