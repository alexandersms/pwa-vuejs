<template>
  <div>
    <v-app-bar dark>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>PWA VueJS</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn>
        <v-icon>mdi-desktop-mac-dashboard</v-icon>
        &nbsp; Dashboard
      </v-btn>

      <v-btn>
        <v-icon>mdi-login-variant</v-icon>
        &nbsp; Sign In
      </v-btn>

      <v-btn :to="{ name: 'Register' }">
        <v-icon>mdi-account-plus-outline</v-icon>
        &nbsp; Sign Up
      </v-btn>

      <v-menu left bottom>
        <template v-slot:activator="{ on, attrs }">
          <v-btn icon v-bind="attrs" v-on="on">
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>
      </v-menu>
    </v-app-bar>
  </div>
</template>

<script>
export default {};
</script>

<style scoped></style>
