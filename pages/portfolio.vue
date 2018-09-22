<template lang="pug">
  .containerr
    .card(v-for="(p, index) in projects")
      .card-image
        figure.image.is-4by1
          img(:src="p.src")
      .card-content
        .media-content
          p.title {{ p.title }}
        .content {{ p.description }}


</template>

<script>
  export default {
    data() {
      return {
        projects: [
          {
            title: 'Vue Music',
            description: 'Final project of the Vue.js course in Platzi.com, in which we use the Spotify API to make an online music player.',
            src: './images/vuemusic.png',
            url: 'http://vue-music.now.sh'
          },
          {
            title: 'Last.fm',
            description: 'In this simple project to show a small list of artists using the last fm API.',
            src: './images/vuebasic.png',
            url: 'http://vue-basic.surge.sh'
          },
          {
            title: 'Memory game',
            description: 'This is a project using the local storage to create a list of tasks.',
            src: './images/vuelocalstorage.png',
            url: 'http://vue-local-storage.surge.sh'
          },
          {
            title: 'Memory game',
            description: 'This project is a game to memorize letters using only Javascript. Only for desktop.',
            src: './images/vuememory.png',
            url: 'http://vue-memory.surge.sh'
          }
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  .containerr {
    display: grid;
    grid-template-columns: repeat(4, minmax(300px, 1fr));
    align-items: flex-start;
  }
  .card {
    margin: 20px;
  }


</style>