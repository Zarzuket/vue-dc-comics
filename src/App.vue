<template>
  <div id="app">
    <Header/>
    <MainTop/>
    <ShopMenu/>
  </div>
</template>

<script>
import Header from "./components/Header.vue"
import MainTop from "./components/MainTop.vue"
import ShopMenu from "./components/ShopMenu.vue"
export default {
  name: 'App',
  components: {
    Header,
    MainTop,
    ShopMenu,
  }
}
</script>

<style lang="scss">
  @import "@/assets/style/common"
</style>
