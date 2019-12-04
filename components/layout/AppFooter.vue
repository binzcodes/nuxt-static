<template>
  <v-hover v-slot:default="{ hover }">
    <v-footer
      :class="{ 'grey lighten-3': hover }"
      absolute
      class="font-weight-medium"
      padless
    >
      <v-col
        @click="openSite()"
        :class="{ isHover: hover, 'text--darken-2': hover }"
        class="text-center grey--text hover"
        cols="12"
      >
        <strong>rbi.nz</strong>
      </v-col>
    </v-footer>
  </v-hover>
</template>

<script scoped>
export default {
  name: 'Footer',
  methods: {
    openSite() {
      window.open('https://rbi.nz', '_blank')
    }
  }
}
</script>

<style>
.isHover {
  cursor: pointer;
}
</style>
