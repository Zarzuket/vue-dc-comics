<template>
  <div id="app">
    <Header/>
    <Jumbo/>
    <MainTop/>
    <ShopMenu/>
    <FooterTop/>
    <FooterBot/>
  </div>
</template>

<script>
import Header from "./components/Header.vue"
import MainTop from "./components/MainTop.vue"
import ShopMenu from "./components/ShopMenu.vue"
import FooterTop from "./components/FooterTop.vue"
import FooterBot from "./components/FooterBot.vue"
import Jumbo from "./components/Jumbo.vue"
export default {
  name: 'App',
  components: {
    Header,
    MainTop,
    ShopMenu,
    FooterTop,
    FooterBot,
    Jumbo,
  }
}
</script>

<style lang="scss">
  @import "@/assets/style/common"
</style>
