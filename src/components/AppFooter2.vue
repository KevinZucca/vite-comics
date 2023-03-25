<script>
  export default {
    data () {
      return {
        logos: [
            "/public/img/footer-facebook.png",
            "/public/img/footer-twitter.png",
            "/public/img/footer-youtube.png",
            "/public/img/footer-pinterest.png",
            "/public/img/footer-periscope.png",
        ]   
      };
    },
    
  }
</script>


<template>
    <div class="container">
        <div class="container-centered">
            <div id="left-button">
                <button>SIGN-UP-NOW</button>
            </div>
            <div id="social-logos">
                <h4>FOLLOW US</h4>
                <img v-for="logo in logos" :src="logo" alt="logo-social">
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
    .container {
        height: 120px;
        background-color: #303030;

        &-centered {
            justify-content: space-between;

            button {
                padding: 15px;

                border: 3px solid #176bdd;
                background-color: #303030;

                &:hover {
                    border: 3px solid #ff585883;
                    filter: brightness(120%);
                    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
                }
            }

            h4 {
                color: #176bdd;

                &:hover {
                    text-shadow: 2px 1px 4px rgba($color: #27409c44, $alpha: 1.0);
                    scale: 1.1;
                    color: #5295f2;

                }
            }

            #social-logos {
                display: flex;
                align-items: center;
                gap: 20px;

                cursor: pointer;

                img:hover {
                    scale: 1.2;
                    filter: brightness(200%);
                }

            }
        }
    }
</style>