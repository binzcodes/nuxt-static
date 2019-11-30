<template>
  <v-tooltip bottom>
    <template v-slot:activator="{ on }">
      <v-icon v-on="on" :color="skill.color" size="28">
        {{ skill.icon }}
      </v-icon>
    </template>
    <span>{{ skill.name }}</span>
  </v-tooltip>
</template>

<script>
export default {
  name: 'Skill',
  props: {
    skill: {
      type: Object,
      required: true
    }
  }
}
</script>
