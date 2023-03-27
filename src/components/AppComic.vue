<script>
import { remove } from '@vue/shared';

  export default {
    data () {
      return {
       
      };
    },

    props: {
        img: String,
        title: String,
    },

    methods: {
        activateComic() {
            const comics = document.querySelectorAll(".comic-img")
            comics.forEach((comic) =>{
                comic.classList.remove("active")
            })
            event.target.classList.add("active")
        }
    }
    
  }
</script>


<template>
    <div class="comic-card">
        <img class="comic-img" @mouseover="activateComic" :src="img" alt="comic-img">
        <h4 class="title">{{ title }}</h4>
    </div>
</template>


<style lang="scss" scoped>    
    .comic-card {
        display: flex;
        flex-flow: column;
        justify-content: center;
        text-align: center;

        width: 180px;

        &:hover {
            scale: 1.2;
            cursor: pointer;
        }

        &:hover h4 {
            color: white;
        }

        img {
            height: 150px;
            width: 100%;
            object-fit: cover;
            object-position: top;
            box-shadow: 2px 2px 4px rgba($color: #000000, $alpha: 1.0);
            opacity: 0.7;
        }

        .active {
            opacity: 1.5;
        }


        h4 {
            color: #d5ccc5;
        }
    }
</style>