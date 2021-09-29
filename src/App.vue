<template>
  <div id="app">
    <HeaderTop/>
  </div>
</template>

<script>
import HeaderTop from "./components/HeaderTop.vue"
export default {
  name: 'App',
  components: {
    HeaderTop,
  }
}
</script>

<style lang="scss">
  @import "@/assets/style/common"
</style>
