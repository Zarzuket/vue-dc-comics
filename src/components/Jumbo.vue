<template>
    <div class="background" :style="`background-image: url(${bgImage})`"></div>
</template>

<script>
export default {
  name:"Jumbo",
  props:[
    "bgImage"
  ]
}
</script>

<style lang="scss" scoped>
.background{
    height: 25rem;
    background-position: top;
    background-position: cover;
}
</style>