<script>
  export default {
    data () {
      return {  
        footerLinks: [
            {
                title: "dc comics",
                links: [
                    "Characters",
                    "Comic",
                    "Movies",
                    "TV",
                    "Games",
                    "Videos",
                    "News"
                ]
            },
            {
                title: "shop",
                links: [
                    "Shop DC",
                    "Shop DC Collectibles",
                ]
            },
            {
                title: "dc",
                links: [
                    "Terms Of Use",
                    "Privacy policy (New)",
                    "Ad Choices",
                    "Advertising",
                    "Jobs",
                    "Subscriptions",
                    "Talent Workshops",
                    "CPSC Certificates",
                    "Ratings",
                    "Shop Help",
                    "Contact Us"
                ]
            },
            {
                title: "sites",
                links: [
                    "DC",
                    "MAD Magazine",
                    "DC Kids",
                    "DC Universe",
                    "DC Power Visa"
                ]
            }
        ]
      };
    },
    
  }
</script>


<template>
   <div class="container">
        <div class="container-centered">  
          <div id="columns-container">
            <ul v-for="column in footerLinks">
                <li>
                    <a href="#" id="title">
                        {{ column.title }}
                    </a>
                    <a id="links" href="#" v-for="link in column.links">
                        {{ link }}
                    </a>
                </li>
            </ul>
          </div>          
          <div id="big-logo">
            <img src="/public/img/dc-logo-bg.png" alt="big-logo">
          </div>
        </div>
   </div>
</template>


<style lang="scss" scoped>
    .container {
        height: 400px;
        background-image: url("/public/img/footer-bg.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        overflow: hidden;
           
        &-centered {
            display: flex;
            justify-content: space-between;


            #columns-container {
                display: flex;
                flex-flow: column wrap;
                height: 100%;
                width: 40%;

                padding: 20px 0;

                ul {

                    display: flex;
                    flex-flow: column wrap;
                    gap: 80px;


                    li {
                        width: 100%;
                        display: flex;
                        flex-flow: column;

                    #title {
                        text-transform: uppercase;
                        text-decoration: none;
                        font-size: 1.2em;
                        color: white;
                        padding-bottom: 10px;

                        &:hover {
                            text-shadow: 2px 1px 4px rgba($color: #d6d6d6, $alpha: 1.0);
                        }
                    }

                    #links {
                        color: #959595;
                        text-decoration: none;

                        &:hover {
                            text-shadow: 2px 1px 4px rgba($color: #d6d6d6, $alpha: 1.0);
                        }
                    }
                }
                }
            }

            #big-logo {
                pointer-events: none;
            }
        }

         


        }

</style>