<template>
  <v-row>
    <v-col class="d-flex justify-start">
      logo
    </v-col>
    <v-col class="d-flex justify-end">
      <span v-for="item in menuItems" :key="item.title" class="mx-3">
        <nuxt-link :to="item.path">{{ item.title }}</nuxt-link>
      </span>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data () {
    return {
      menuItems: [
        { title: 'Home', path: '/' }, { title: 'About', path: '/about' },
        { title: 'Skill', path: '/skill' }, { title: 'Project', path: '/project' },
        { title: 'Contact', path: '/contact' } ]
    }
  }
}
</script>

<style lang="scss" scoped>
  a {
    text-decoration: none;
  }
</style>
