<template>
  <div>
      <div class="background">
        <div class="container">
            <div class="container_button">
              <button class="btn">SIGN-UP NOW!</button>
            </div>
            <div class="Follow_us">
                FOLLOW US
            </div>
            <div class="container_ico">
                <ul>
                    <li v-for="(ico,index) in icos" :key="index">
                        <img :src="'/img/' + ico.name + '.png'" alt="">
                    </li>
                </ul>              
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"FooterBot",
    data(){
        return{
            icos:[
                {
                    name:"footer-facebook"
                },
                {
                    name:"footer-periscope"
                },
                {
                    name:"footer-pinterest"
                },
                {
                    name:"footer-twitter"
                },
                {
                    name:"footer-youtube"
                }
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
@import "@/assets/style/variables";

.background{
    background-color: #303030;
    height: 5.5rem;
}
.container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
}
.Follow_us{
    margin-left: auto;
    color: $primarycolor;
    font-size: 1.25rem;
    font-weight:bold;
}
.btn{
    padding: 10px;
    border:3px solid $primarycolor;
    background-color: #303030;
    color: white;
    font-size: 1.25rem;
}
ul{
    display: flex;
    li{
        list-style: none;
        padding: 0 .625rem;
    }
}
</style>