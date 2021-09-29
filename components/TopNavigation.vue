<template>
<section v-html="content.content">
</section>
</template>
<script lang="ts">
import { Context } from '@nuxt/types'
export default {
  data () {
    return {
      content: ''
    }
  },
  activated() {
      // Call fetch again if last fetch more than 30 sec ago
  },
  async fetch() {
      this.content = await this.$nuxt.context.app.$libertyRepository.show('site.TopNavigation')
  },
}
</script>
