<template>
  <v-app>
    <app-header />
    <router-view></router-view>
  </v-app>
</template>

<script>
import AppHeader from "@/components/core/AppHeader.vue";

export default {
  name: "App",
  components: {
    AppHeader,
  },
};
</script>
