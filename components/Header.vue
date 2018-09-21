<template lang="pug">
  nav(class="navbar is-light"
      role="navigation"
      arial-label="main navigation")
    .navbar-brand
      nuxt-link.navbar-item(to="/")
        img(src="~/static/logo/Logo_largo.svg")
      a.navbar-burger(
        :class="{ 'is-active': isOpen }"
        role="button"
        arial-label="menu"
        aria-expanded="flase"
        @click="openMenu"
        )
        span(aria-hidden="true")
        span(aria-hidden="true")
        span(aria-hidden="true")
    .navbar-menu(
      :class="{ 'is-active': isOpen === true }"
      @focusout="closeMenu")
      .navbar-end(@click="closeMenu")
        nuxt-link.navbar-item(to="/") Home
        nuxt-link.navbar-item(
          @click="closeMenu" 
          to="about") About
        nuxt-link.navbar-item(
          @click="closeMenu"
          to="portfolio") Portfolio
        nuxt-link.navbar-item(to="skills") Skills
        .navbar-item.has-dropdown.is-hoverable
          a.navbar-link(href="#") Languages
          .navbar-dropdown.is-boxed
            a.navbar-item(href="#") English
            a.navbar-item(href="#") Spanish


    
</template>

<script>
  export default {
    data() {
      return {
        isOpen: false
      }
    },
    methods: {
      openMenu() {
        this.isOpen = true
      },
      closeMenu() {
        this.isOpen = false
      }
    }
  }
</script>

<style lang="scss" scoped>

  // a.navbar-item img {
  //   max-height: 50px;
  // }

</style>