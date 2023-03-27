<script>
  import AppHeader from "./components/AppHeader.vue"
  import AppJumbo from "./components/AppJumbo.vue"
  import AppMain1 from "./components/AppMain1.vue"
  import AppMain2 from "./components/AppMain2.vue"
  import AppFooter1 from "./components/AppFooter1.vue"
  import AppFooter2 from "./components/AppFooter2.vue"




  export default {
    data() {
      return {

      };
    },
    components: {
      AppHeader,
      AppJumbo,
      AppMain1,
      AppMain2,
      AppFooter1,
      AppFooter2,      
    },

    methods: {}

  }
</script>

<template>
  <AppHeader></AppHeader>
  <AppJumbo></AppJumbo>
  <AppMain1></AppMain1>
  <AppMain2></AppMain2>
  <AppFooter1></AppFooter1>
  <AppFooter2></AppFooter2>

</template>

<style>
  
</style>
