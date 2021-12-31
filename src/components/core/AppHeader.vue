<template>
  <div>
    <v-app-bar dark>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>PWA VueJS</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn flat>
        <v-icon>mdi-login-variant</v-icon>
        &nbsp; Sign In
      </v-btn>

      <v-btn :to="{ name: 'Register' }" flat>
        <v-icon>mdi-account-plus-outline</v-icon>
        &nbsp; Sign Up
      </v-btn>

      <v-menu left bottom>
        <template v-slot:activator="{ on, attrs }">
          <v-btn icon v-bind="attrs" v-on="on">
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>

        <v-list>
          <v-list-item v-for="n in 5" :key="n" @click="() => {}">
            <v-list-item-title>Option {{ n }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>
  </div>
</template>

<script>
export default {};
</script>

<style scoped></style>
