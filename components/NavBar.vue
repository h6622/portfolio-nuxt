<template>
  <v-container class="ma-0">
    <v-row>
      <v-col class="d-flex justify-center">
        logo
      </v-col>
      <v-col :cols="10" class="d-flex justify-center">
        <span v-for="item in menuItems" :key="item.title" class="mx-9">
          <nuxt-link :to="item.path">{{ item.title }}</nuxt-link>
        </span>
      </v-col>
    </v-row>
  </v-container>
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
  .container{
    background: #1D976C;
    background: -webkit-linear-gradient(to right, #93F9B9, #1D976C);
    background: linear-gradient(to right, #93F9B9, #1D976C);
  }
  a {
    text-decoration: none;
    color: white !important;
  }
</style>
