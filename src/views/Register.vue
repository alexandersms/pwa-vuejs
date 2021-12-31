<template>
  <v-app id="inspire">
    <v-content>
      <v-container fluid fill-height>
        <v-layout align-center justify-center>
          <v-flex xs12 sm8 md4>
            <v-card class="elevation-12">
              <v-toolbar dark color="primary">
                <v-toolbar-title>Sign-Up</v-toolbar-title>
                <v-spacer></v-spacer>
              </v-toolbar>
              <v-card-text>
                <v-form>
                  <v-row>
                    <v-col>
                      <v-text-field
                        prepend-icon="mdi-account"
                        name="firstname"
                        label="FirstName"
                        type="text"
                      ></v-text-field>
                    </v-col>
                    <v-col>
                      <v-text-field
                        prepend-icon="mdi-account-outline"
                        name="lasttname"
                        label="LastName"
                        type="text"
                      ></v-text-field>
                    </v-col>
                  </v-row>
                  <v-text-field
                    prepend-icon="mdi-email"
                    name="email"
                    label="Email"
                    type="text"
                  ></v-text-field>
                  <v-text-field
                    id="password"
                    prepend-icon="mdi-lock"
                    name="password"
                    label="Password"
                    type="password"
                  ></v-text-field>
                  <v-text-field
                    id="password_conf"
                    prepend-icon="mdi-lock-outline"
                    name="password_conf"
                    label="Confirm Password"
                    type="password"
                  ></v-text-field>

                  <v-autocomplete
                    v-model="value"
                    :items="items"
                    dense
                    filled
                    label="Select your status"
                  ></v-autocomplete>
                </v-form>
              </v-card-text>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn color="primary">Register</v-btn>
              </v-card-actions>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      items: ["Teacher", "Student"],
      value: null,
    };
  },
};
</script>
