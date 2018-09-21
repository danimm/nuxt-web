<template lang="pug">
  .containerr
    .card(v-for="(p, index) in projects")
      .card-image
        figure.image.is-4by1
          img(:src="p.src")
      .card-content
        .media-content
          p.title {{ p.title }}
          p.subtitle subtitulo
        .content {{ p.description }}


</template>

<script>
  export default {
    data() {
      return {
        projects: [
          {
            title: 'Vue Music',
            description: 'Proyecto final del curso de Vuejs en Platzi.com, en el cuál usamos la API de Spotify para crear un reproductor de música online.',
            src: './images/vuemusic.png',
            url: 'http://vue-music.now.sh'
          },
          {
            title: 'Last.fm',
            description: 'Este es un proyecto simple para mostrar una pequeña lista de artistas usando la API de last fm.',
            src: './images/vuebasic.png',
            url: 'http://vue-basic.surge.sh'
          },
          {
            title: 'Manipulando el DOM',
            description: 'Este es un proyecto usando el Local Storage para crear una lista de Tareas.',
            src: './images/vuelocalstorage.png',
            url: 'http://vue-local-storage.surge.sh'
          },
          {
            title: 'Juego de memoria',
            description: 'Este proyecto es un juego de memorizar letras usando sólo Javascript. Sólo para vista de escritorio.',
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

  figure {
  }
</style>