<script>
  export default {
    data () {
      return {
        links: [
            "characters",
            "comics",
            "movies",
            "tv",
            "games",
            "collectibles",
            "videos",
            "fans",
            "news",
            "shop"
        ]
      };
    },
    
  }
</script>


<template>
    <header>
        <div class="container-centered">
            <div id="logo">
                <img src="/public/img/dc-logo.png" alt="logo">
            </div>
            <div id="links" v-for="link in links">
                {{ link }}
            </div>
        </div>
    </header>
</template>


<style lang="scss" scoped>
    header {
        height: 120px;
        border: 1px solid black;
       

        .container-centered {
            
            #logo{
                flex-grow: 1;
            }


            #links {
                text-transform: uppercase;
                font-weight: bold;
                color: #464646;
                padding: 8px;
            }
        }
    }
</style>