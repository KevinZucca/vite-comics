<script>
  export default {
    data () {
      return {
        links: [
            {
                img: "/public/img/buy-comics-digital-comics.png",
                link: "digital comics"
            },
            {
                img: "/public/img/buy-comics-merchandise.png",
                link: "dc merchandise"
            },
            {
                img: "/public/img/buy-comics-subscriptions.png",
                link: "subscription"
            },
            {
                img: "/public/img/buy-comics-shop-locator.png",
                link: "comic shop locator"
            },
            {
                img: "/public/img/buy-dc-power-visa.svg",
                link: "dc power visa"
            },
        ]
      };
    },
    
  }
</script>


<template>
    <div class="container">
       <div class="container-centered">
            <ul id="shop-links">
                <li v-for="link in links">
                     <img :src="link.img" alt="">
                     <a>{{ link.link }}</a>
                </li>
            </ul>
       </div>
    </div>
</template>


<style lang="scss" scoped>
   .container {
        height: 120px;

        background-color: #0282f9;
        color: white;

        .container-centered {
            max-width: 1200px;
            justify-content: space-around;

            ul {
                display: flex;
                gap: 50px;
                text-transform: uppercase;

                li{
                    display: flex;
                    flex-flow: row nowrap;
                    align-items: center;
                    gap: 5px;
                }

                img {
                    height: 50px;
                    width: 40px ;
                }

            }
        }
   }
</style>