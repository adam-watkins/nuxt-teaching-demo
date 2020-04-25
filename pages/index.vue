<template>
  <div class="display-4 font-weight-black">
    HOME PAGE
    <v-btn to="/register">Register</v-btn>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo
  }
}
</script>
