<template>
  <div class="background">
    <div class="container">
        <div v-for="(single,index) in menu" :key="index" class="container_img">
            <img :src="single.text" alt="">
        </div>
        <div>
            
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name:"ShopMenu",
    data(){
        return{
            menu: [
                {
                    text:"../../public/img/buy-comics-digital-comics.png",
                    info: "DIGITAL COMICS"   
                },
                {
                    text:"../assets/img/buy-comics-merchandise.png",
                    info: "DC MERCHANDISE"
                },
                {
                    text:"../assets/img/buy-comics-shop-locator.png",
                    info:"SUBSCRIPTION"
                },
                {
                    text:"../assets/img/buy-comics-subscriptions.png",
                    info:"COMIC SHOP LOCATOR"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "@/assets/style/variables";
.background{
    background-color: $primarycolor;
    height: 12.5rem;
}
.container{
    display: flex;
    align-items: center;
    height: 100%;
    .container_img{
        height: 100%;
        img{
            height: 12.5rem;
            width: 12.5rem;
        }
    }
}
</style>