<template>
  <div class="background">
    <div class="container">
        <div v-for="(single,index) in menu" :key="index" class="container_img">
            <img :src="'../img/' + single.text + '.png'" alt="">
            <div class="container_text">
                {{single.info}}
            </div>
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
                    text:"buy-comics-digital-comics",
                    info: "DIGITAL COMICS"   
                },
                {
                    text:"buy-comics-merchandise",
                    info: "DC MERCHANDISE"
                },
                {
                    text:"buy-comics-shop-locator",
                    info:"SUBSCRIPTION"
                },
                {
                    text:"buy-comics-subscriptions",
                    info:"COMIC SHOP LOCATOR"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables";
.background{
    background-color: $primaryColor;
    height: 12.5rem;
}
.container{
    display: flex;
    align-items: center;
    justify-content: space-around;
    height: 100%;
    .container_img{
        display: flex;
        padding: 0 1.25rem;
        img{
            width: 20%;
        }
    }
}
.container_text{
    display: flex;
    align-items: center;
    color: white;
    padding: 0 .625rem;
}
</style>