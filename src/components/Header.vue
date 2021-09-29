<template>
  <div class="container">
      <div class="logo">
          <img src="@/assets/img/dc-logo.png" alt="xxx">
      </div>
      <nav>
          <ul>
                <li v-for="(link,index) in menu" :key="index">
                    <a :href="link.url" :class="{active : link.current}">{{link.text}}</a>
                </li>
          </ul>
      </nav>
  </div>
</template>

<script>
export default {
    name: "Header",
    data(){
        return{
            menu: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false
                },
                {
                    text: "TV",
                    url: "#",
                    current: false
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "@/assets/style/variables";

li{
    list-style: none;

    a{
        text-decoration: none;
        color: grey;
        font-size: 1.25rem;
        font-weight: bold;
        padding: 1.25rem;
    &.active{
        border-bottom: .1875rem solid $primarycolor;
        color: $primarycolor;
    }
    }
}
.container{
    display: flex;
    padding-top: 1.25rem;
    justify-content: space-between ;
    align-items: center;
    
}
img{
    width: 100%;
}
nav{
  ul{
      display: flex;
      justify-content: center;
    }
}
</style>