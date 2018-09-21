<template lang="pug">
  .grid
    .contenedor
      span.tag.is-danger.is-medium(
        v-for="i in General"
      ) {{ i.title }}
    .contenedor
      span.tag.is-info.is-medium(
        v-for="i in Javascript"
      ) {{ i.title }}
    .contenedor
      span.tag.is-primary.is-medium(
        v-for="i in CSS3"
      ) {{ i.title }}
    .contenedor
      span.tag.is-link.is-medium(
        v-for="i in DevTools"
      ) {{ i.title }}
    .contenedor
      span.tag.is-warning.is-medium(
        v-for="i in Backend"
      ) {{ i.title }}
</template>

<script>
  export default {
    data() {
      return {
        General: [
          {
            title: 'HTML5'
          },
          {
            title: 'CSS'
          },
          {
            title: 'Javascript'
          },
        ],
        Javascript: [
          {
            title: 'ECMAScript 6'
          },
          {
            title: 'Babel'
          },
          {
            title: 'Vue'
          },
          {
            title: 'Nuxt(SSR)'
          },
          {
            title: 'React'
          },
          {
            title: 'JSX'
          },
          {
            title: 'NextJS(SSR)'
          },
        ],
        CSS3: [
          {
            title: 'Responsive Design'
          },
          {
            title: 'Bootstrap'
          },
          {
            title: 'Foundation'
          },
          {
            title: 'Bulma'
          },
          {
            title: 'MaterializeCSS'
          },
          {
            title: 'Pug(Jade)'
          },
          {
            title: 'SASS'
          },
          {
            title: 'PostCSS'
          },
          {
            title: 'Style JSX'
          },
          {
            title: 'CSS Grid'
          },
          {
            title: 'Transition'
          },
          {
            title: 'Animation'
          },
        ],
        DevTools: [
          {
            title: 'Webpack'
          },
          {
            title: 'Git/GitHub'
          },
          {
            title: 'Sketch'
          },
          {
            title: 'NPM/Yarn'
          },
          {
            title: 'ESLint'
          },
          {
            title: 'Now'
          },
        ],
        Backend: [
          {
            title: 'Firebase'
          },
          {
            title: 'Node'
          },
          {
            title: 'Express'
          },
          {
            title: 'MongoDB'
          },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>
  .grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    margin: 20px;
  }
  .contenedor {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(auto-fill, 1fr);
    grid-gap: 10px;
    justify-items: start;
  }
  .tag:nth-of-type(2),
  .tag:nth-of-type(5),
  .tag:nth-of-type(8),
  .tag:nth-of-type(11), {
    justify-self: center;
  }
  .tag:nth-of-type(3),
  .tag:nth-of-type(6),
  .tag:nth-of-type(9),
  .tag:nth-of-type(12), {
    justify-self: center;
  }
</style>