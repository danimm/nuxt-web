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
          p If you have any questions write me to: in@danimm.com
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
    
  }
</script>

<style scoped>
  table {
    background-color: transparent;
  }
</style>