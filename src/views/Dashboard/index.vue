<template>
  <div id="app">
    <v-app id="inspire">
      <v-app id="sandbox">
        <v-navigation-drawer
          v-model="primaryDrawer.model"
          :clipped="primaryDrawer.clipped"
          :floating="primaryDrawer.floating"
          :mini-variant="primaryDrawer.mini"
          :permanent="primaryDrawer.type === 'permanent'"
          :temporary="primaryDrawer.type === 'temporary'"
          app
          overflow
        ></v-navigation-drawer>

        <v-app-bar> </v-app-bar>

        <v-footer :inset="footer.inset" app>
          <span class="px-4">&copy; {{ new Date().getFullYear() }}</span>
        </v-footer>
      </v-app>
    </v-app>
  </div>
</template>

<script>
export default {
  name: "Dashboard",
  data() {
    return {
      drawers: ["Default (no property)", "Permanent", "Temporary"],
      primaryDrawer: {
        model: null,
        type: "default (no property",
        clipped: false,
        floating: false,
        mini: false,
      },
      footer: {
        inset: false,
      },
    };
  },
};
</script>

<style scoped></style>
