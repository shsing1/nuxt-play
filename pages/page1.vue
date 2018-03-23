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
          nuxt-link(to="/login") login
          nuxt-link(to="/page1") Page1
          nuxt-link(to="/page2") Page2
          nuxt-link(to="/page3") Page3
</template>

<script>
export default {

}
</script>

<style>

</style>
