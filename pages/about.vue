<template lang="pug">
  .container.is-fluid
    .content
      .columns
        .column
          figure.image
            img(src="~/static/daniel.jpg")
        .column
          h3 About me
          p I am passionate about technology. I am a technician in Systems Administration, but the las years i am directing my career to the Web development.
          p I love learning the new technologies of modern web development and creating personal projects to put my knowledge into practice.
          p You can find all my personal projects in personal Portfolio
          h3 Front end development
          p I'm specializing in Frontend Web Development, with the current Web standards and always looking for new front-end frameworks to add to my development stack.
          h3 Responsive Design
          p Always looking for the best user experience using responsive designs, with frameworks like Bootstrap, Materialize-css (used in this website), Foundation... It doesn't matter the device or the resolution, you will always have a good user experience.
          h3 100% Self-taught
          p In the world of web development, you have to learn constantly! That's why I study daily to be always updated with the new frameworks and libraries. One of my favorite places to study is in Platzi. It is an online education platform with more than 500,000 students. You can check my profile here
</template>

<script>
  export default {
    
  }
</script>

<style scoped>
  .container {
    padding: 20px;
  }
  figure {
    max-width: 60%;
  }
  figure img {
    border-radius: 50%;
    border: 4px solid #374f75;
  }
  .column:nth-child(1) {
    display: flex;
    justify-content: center;
  }
</style>