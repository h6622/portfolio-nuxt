<template>
  <div :style="{backgroundImage: `url(${bgUrl})`}" class="bg">
    <v-layout row wrap>
      <v-flex xs12>
        h662
      </v-flex>
      <v-flex>H662</v-flex>
      <v-flex>H662</v-flex>
    </v-layout>
  </div>
</template>

<script>
import bgUrl from '@/assets/images/notebook.jpg'

export default {
  data () {
    return { bgUrl }
  }
}
</script>

<style lang="scss" scoped>
  .bg {
    height: 1000px;
  }
</style>
