<template>
  <div>
      <div class="background">
        <div class="container">
              <button class="btn">SIGN-UP NOW!</button>
            <div class="container_ico">
                <ul>
                    <li v-for="(ico,index) in icos" :key="index">
                        <img :src="'../img/' + ico.name + '.png'" alt="">
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
                    name:"footer-persicope"
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
    height: 12.5rem;
}
.btn{
    padding: 10px;
    border:3px solid $primarycolor;
    background-color: #303030;
    color: white;
    font-size: 1.25rem;
}
</style>