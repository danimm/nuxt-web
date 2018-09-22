<template lang="pug">
  footer.footer
    .content
      .columns
        .column
          //- p
          //-   strong Daniel Muñoz
          //-   |  by 
          //-   a(href='https://jgthms.com') Jeremy Thomas
          //-   | . The source code is licensed
          //-   a(href='http://opensource.org/licenses/mit-license.php') MIT
          //-   | . The website content
          //-   |         is licensed 
          //-   a(href='http://creativecommons.org/licenses/by-nc-sa/4.0/') CC BY NC SA 4.0
          //-   | .
          h4.subtitle Thank you for your visit!
          p The purpose of this website is to have all my personal projects and knowledge in one place.
          p If you have any questions write me to: 
            a(:href="`mailto:${mail}`") info@danimm.com
          a.is-link(href="https://www.linkedin.com/in/daniel-mm/" target="_blank")
            img(src="~/static/footer-icons/linkedin.svg")
          a.is-link(href="https://github.com/danimm" target="_blank")
            img(src="~/static/footer-icons/github-logo.svg")
          a.is-link(href="https://twitter.com/Danimm_dev" target="_blank")
            img(src="~/static/footer-icons/twitter-logo.svg")
            
        .column
          table.table
            tbody
              tr
                td.has-text-centered-mobile
                  nuxt-link(to="/") Home
              tr
                td.has-text-centered-mobile
                  nuxt-link(to="about") About
              tr
                td.has-text-centered-mobile
                  nuxt-link(to="portfolio") Portfolio
              tr
                td.has-text-centered-mobile
                  nuxt-link(to="skills") Skills

      .content.has-text-centered
        p Created by Daniel Muñoz Martín
</template>

<script>
  export default {
    data() {
      return {
        mail: 'info@danimm.com'
      }
    }
  }
</script>

<style scoped>
  table {
    background-color: transparent;
  }
  a.is-link {
    /* display: inline-block; */
    padding-right: 20px;
    /* height: 50px;
    width: 50px; */
  }
  a.is-link img {
    height: 40px;
  }
</style>