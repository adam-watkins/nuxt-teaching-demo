<template>
  <v-card :elevation="eval">
    <v-card-title>{{ title }}</v-card-title>
    <v-card-text>PLS use my awesome app</v-card-text>
    <v-card-actions>
      <v-spacer />
      <v-btn to="/" light>Login</v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  name: "LoginCard",
  props: {
    title: {
      type: String,
      default: 'I LOVE TITS'
    },
    eval: {
      type: Number,
      default: 0
    }
  }
}
</script>
