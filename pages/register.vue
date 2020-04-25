<template>
  <div>
    <v-row justify="center">
      <v-col cols="4">
        Hi am at register page
        <LoginCard title="Vue" class="my-8" :eval="elevation" />
      </v-col>
    </v-row>
    <v-btn @click="toggle" dark>{{ clicks }}</v-btn>
  </div>
</template>

<script>
import LoginCard from "~/components/LoginCard";
export default {
  name: "register",
  components: {LoginCard},
  data() {
    return {
      is_end: true,
      clicks: 0
    }
  },
  computed: {
    elevation() {
      if (this.is_end === true) return 20;
      else return 0
    }
  },
  methods: {
    toggle() {
      this.is_end = !this.is_end;
      this.clicks++
    }
  }
}
</script>
