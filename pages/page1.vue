<template lang="pug">
  transition(name="page")
    section.container
      div
        app-logo
        h1.title next-play
        h2.subtitle Nuxt.js project
        .links
          a(href="https://nuxtjs.org/"
            target="_blank"
            class="button--green") Documentation
          a(href="https://github.com/nuxt/nuxt.js"
            target="_blank"
            class="button--grey") GitHub
          nuxt-link(to="/page1") Page1
          nuxt-link(to="/page2") Page2
          nuxt-link(to="/page3") Page3
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
