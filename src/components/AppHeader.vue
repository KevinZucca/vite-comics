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
            <a id="links" v-for="link in links">
                {{ link }}
            </a>
        </div>
    </header>
</template>


<style lang="scss" scoped>
    header {
        height: 120px;

        background-color: #fff;
        border: 1px solid black;
       

        .container-centered {

            padding-bottom: 0;
            padding-top: 0;
            
            #logo{
                flex-grow: 1;
                cursor: pointer;
            }


            #links {
                display: flex;
                align-items: center;
                height: 100%;          


                text-transform: uppercase;
                font-weight: bold;
                color: #464646;
                padding: 8px;
                padding-bottom: 0;

                cursor: pointer;

                &:hover {
                    text-shadow: 1px 1px 6px rgba($color: #3b7ad861, $alpha: 1.0);
                    border-bottom: 6px solid #0282f9;
                    color: #0282f9;
                }
            }
        }
    }
</style>