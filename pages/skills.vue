<template lang="pug">
  .grid
    .message.is-light
      .message-header.has-text-centered
        p.title.cen What can i do ?
      .message-body
        .content.progress-container
          .content(v-for="t in techs")
            p {{ t.title }}
            progress(class="progress is-success" :value="t.progress" max="100")
        p In the world of web development, you have to learn constantly! That's why I study daily to be always updated with the new frameworks and libraries. One of my favorite places to study is in Platzi. It is an online education platform with more than 500,000 students.
        br
        p You can check my profile here
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
        techs: [
          {
            title: 'HTML5',
            progress: 80
          },
          {
            title: 'CSS',
            progress: 60
          },
          {
            title: 'Javascript',
            progress: 50
          },
        ],
        Javascript: [
          {
            title: 'Javascript'
          },
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
            title: 'CSS3'
          },
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
            title: 'DevTools'
          },
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
            title: 'Backend'
          },
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
    grid-gap: 10px;
  }
  .contenedor {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(auto-fill, 2em);
    grid-gap: 10px;
    grid-row-start: 2;
    // justify-items: center;
  }
  .message {
    grid-column: 2 / span 2;
  }
  // .message p.title {
  //   color: white;
  // }
  .contenedor.hastext {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  .contenedor.hastext p {
    word-spacing: 20px;
  }
  .tag:nth-of-type(1) {
    grid-column: span 2;
    justify-self: stretch;
  }
  .progress-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 20px;
  }
</style>