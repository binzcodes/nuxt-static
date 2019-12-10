<template>
  <v-card-actions v-if="stack.length > 0" class="d-flex justify-space-between">
    <div v-bind:key="stack.index" v-for="technology in stack">
      <app-technology v-bind:technology="technology"></app-technology>
    </div>
  </v-card-actions>
</template>

<script>
export default {
  name: 'Stack',
  components: {
    AppTechnology: () => import('~/components/placeholder/Technology.vue')
  },
  props: {
    stack: {
      type: [Object, Array],
      default: () => []
    }
  }
}
</script>
