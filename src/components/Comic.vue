<template>
    <div class="card">
      <img class="card_img" :src="com.thumb" alt="com.series">
      <div class="card_title">
        {{com.series}}
      </div>
  </div>
</template>

<script>
export default {
  name:"Comic",
  props:["com"]
}
</script>

<style lang="scss" scoped>
.card{
    width: calc(100% / 6);
    padding: 5px;
		&_title{
			color: white;
		}
		&_img{
			height: 9.5rem;
      width: 9.5rem;
      padding: .3125rem;
      object-fit: cover;
      object-position: top;
		}
}
</style>