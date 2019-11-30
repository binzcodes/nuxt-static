<template>
  <v-app>
    <v-container fluid class="fill-height">
      <v-row align="center" justify="center">
        <v-col cols="12" sm="6" md="4">
          <v-card class="mx-auto">
            <v-img
              class="white--text align-end"
              aspect-ratio="2"
              src="/background.svg"
            >
              <v-card-title v-text="error.statusCode" />
            </v-img>
            <v-card-subtitle v-text="error.message" class="pb-0" />
            <v-card-actions>
              <v-btn text color="primary" nuxt to="/">Back</v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
export default {
  layout: 'default',
  props: {
    error: {
      type: Object,
      default: null
    }
  },
  head() {
    return {
      title: this.message
    }
  },
  computed: {
    statusCode() {
      return (this.error && this.error.statusCode) || 500
    },
    message() {
      return this.error.message || 'An error occurred'
    }
  }
}
</script>
