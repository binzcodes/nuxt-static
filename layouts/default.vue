<template>
  <v-app>
    <!-- nav goes here -->
    <v-content>
      <nuxt />
    </v-content>
    <layout-footer />
  </v-app>
</template>

<script>
export default {
  components: {
    layoutFooter: () => import('~/components/layout/Footer.vue')
  }
}
</script>

<style></style>
