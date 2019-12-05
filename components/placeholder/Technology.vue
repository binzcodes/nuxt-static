<template>
  <v-tooltip bottom>
    <template v-slot:activator="{ on }">
      <v-icon v-on="on" :color="technology.color" size="28">
        {{ technology.icon }}
      </v-icon>
    </template>
    <span>{{ technology.name }}</span>
  </v-tooltip>
</template>

<script>
export default {
  name: 'Technology',
  props: {
    technology: {
      type: Object,
      required: true
    }
  }
}
</script>
