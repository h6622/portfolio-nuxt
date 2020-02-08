<template>
  <div class="navBar">
    <v-container>
      <v-row>
        <v-col>logo</v-col>
        <v-col class="d-flex justify-end">
          <span v-for="item in menuItems" :key="item.title" class="mx-3">
            <nuxt-link :to="item.path">{{ item.title }}</nuxt-link>
          </span>
        </v-col>
      </v-row>
    </v-container>
  </div>
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
.navBar {
  position: fixed;
  max-width: 960px;
  width: 100%;
  left: 50%;
  transform: translateX(-50%);
}
  a {
    text-decoration: none;
  }
</style>
