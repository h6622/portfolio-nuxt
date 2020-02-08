<template>
  <v-app>
    <v-container>
      <nav-bar />
      <nuxt />
    </v-container>
  </v-app>
</template>

<script>
import NavBar from '@/components/NavBar'

export default {
  components: {
    NavBar
  }
}
</script>

<style lang="scss" scoped>
  .container{
    max-width: 960px;
  }
</style>
