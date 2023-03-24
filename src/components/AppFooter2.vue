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
            }

            h4 {
                color: #176bdd;
            }

            #social-logos {
                display: flex;
                align-items: center;
                gap: 20px;

                cursor: pointer;
            }
        }
    }
</style>