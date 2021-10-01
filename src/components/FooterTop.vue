<template>
  <div class="background">
    <div class="container">
        <div class="container_list">
            <ul>
                <li v-for="(name,index) in menuF" :key="index">
                    {{name.name}}
                </li>
            </ul>
            <ul>
                <li v-for="(name,index) in menuS" :key="index">
                    {{name.name}}
                </li>
            </ul>
        </div>
        <div class="container_list">
            <ul>
                <li v-for="(name,index) in menuT" :key="index">
                    {{name.name}}
                </li>
            </ul>
        </div>
        <div class="container_list">
            <ul>
                <li v-for="(name,index) in menuFourth" :key="index">
                    {{name.name}}
                </li>
            </ul>    
        </div>
        <!-- <div class="container_jumbo_bot">
            <img src="/img/dc-logo-bg.png" alt="">
        </div> -->
    </div>
  </div>
</template>

<script>
export default {
    name: "FooterTop",
    data(){
        return{
            menuF:[
            {

                name:"DC COMICS"
            },
            {
                name:"Characters"
            },
            {
                name:"Comics"
            },
            {
                name:"Movies"
            },
            {
                name:"TV"
            },
            {
                name:"Games"
            },
            {
                name:"Videos"
            },
            {
                name:"News"
            },

            ],
            menuS:[
                {
                    name:"SHOP"
                },
                {
                    name:"Shop DC"
                },
                {
                    name:"Shop DC collectables"
                },
            ],
            menuT:[
                {
                    name:"DC"
                },
                {
                    name:"Terms Of Use"
                },
                {
                    name:"Privacy policy (New)"
                },
                {
                    name:"Ad choices"
                },
                {
                    name:"Advertising"
                },
                {
                    name:"Jobs"
                },
                {
                    name:"Subscriptions"
                },
                {
                    name:"Talent Workshops"
                },
                {
                    name:"CPSC Certificates"
                },
                {
                    name:"Ratings"
                },
                {
                    name:"Shop Help"
                },
                {
                    name:"Contact Us"
                },
            ],
            menuFourth:[
                {
                    name:"SITES"
                },
                {
                    name:"DC"
                },
                {
                    name:"MAD Magazine"
                },
                {
                    name:"DC Kids"
                },
                {
                    name:"DC universe"
                },
                {
                    name:"DC Power Visa"
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.background{
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    background-color: black;
    color: white;
    padding: 2.25rem 0;
}
ul{
    padding: .625rem .625rem;
    list-style: none;
    li{
        color: grey;
        font-size: .875rem;
    }
    li:first-child{
        color: white;
        font-weight: bold;
        font-size: 1.125rem;
        padding-bottom: .9375rem;
    }
}
.container{
    display: flex;
} 
.container_list:not(:first-child){
    padding: 0 .9375rem;
}

</style>