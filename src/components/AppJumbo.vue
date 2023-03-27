<script>
  export default {
    data () {
      return {
       
      };
    },
    
  }
</script>


<template>
    <div class="container">
        <img src="/public/img/jumbotron.jpg" alt="jumbo">
    </div>
</template>


<style lang="scss" scoped>
    .container {
        height: 400px;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
            pointer-events: none;
        }
    }
</style>