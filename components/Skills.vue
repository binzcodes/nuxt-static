<template>
  <v-card-actions v-if="skills.length > 0" class="pb-8">
    <div v-bind:key="skill.index" v-for="skill in skills" class="mx-auto">
      <skill v-bind:skill="skill"></skill>
    </div>
  </v-card-actions>
</template>

<script>
export default {
  name: 'Skills',
  components: {
    Skill: () => import('~/components/Skill.vue')
  },
  props: {
    skills: {
      type: [Object, Array],
      default: () => []
    }
  }
}
</script>
