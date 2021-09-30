<template>
  <div>
    <div class="card">
      <img class="card_img" :src="com.thumb" alt="com.series">
      <div class="card_title">
        {{com.series}}
      </div>
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
    padding: 5px;
    width: calc(100% / 6);
		&_title{
			text-align: center;
			color: white;
		}
		&_img{
			width: 100%;
		}
}
</style>