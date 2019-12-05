<template>
  <v-app>
    <!-- nav goes here -->
    <v-content>
      <nuxt />
    </v-content>
    <app-footer />
  </v-app>
</template>

<script>
export default {
  components: {
    AppFooter: () => import('~/components/layout/AppFooter.vue')
  }
}
</script>

<style></style>
