<template>
  <v-container fluid class="fill-height">
    <v-row align="center" justify="center">
      <v-col cols="12" sm="8" md="4">
        <placeholder-card :card-title="cardTitle" />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import config from '~/nuxt.config'
export default {
  components: {
    PlaceholderCard: () =>
      import('~/components/placeholder/PlaceholderCard.vue')
  },
  data() {
    return {
      cardTitle: config.pwa.meta.name
    }
  }
}
</script>
