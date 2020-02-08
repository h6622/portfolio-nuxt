<template>
  <div :style="{backgroundImage: `url(${bgUrl})`}" class="bg">
    <v-layout align-content-center row fill-height>
      <v-flex xs12 class="d-flex justify-center">
        h662
      </v-flex>
      <v-flex xs12 class="d-flex justify-center">
        h662
      </v-flex>
      <v-flex xs12 class="d-flex justify-center">
        h662
      </v-flex>
    </v-layout>
  </div>
</template>

<script>
import bgUrl from '@/assets/images/bg.jpg'

export default {
  data () {
    return { bgUrl }
  }
}
</script>

<style lang="scss" scoped>
  .bg {
    background-size: cover;
    width: 100%;
    height: 100%;
  }
</style>
