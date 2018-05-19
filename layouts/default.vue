<template>
  <b-container fluid>
    <nav-bar/>
    <nuxt/>
  </b-container>
</template>

<script>

import NavBar from "~/components/NavBar.vue"

export default {
  components: {
    NavBar
  }
}
</script>
