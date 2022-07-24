<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <v-toolbar-title>Vuetify Dashboard</v-toolbar-title>
      <v-spacer></v-spacer>

      <router-link to="/">
        <v-btn text> Home </v-btn>
      </router-link>
      <router-link to="/login">
        <v-btn text> Login </v-btn>
      </router-link>
    </v-app-bar>
    <!-- Login Module -->
    <v-main> <router-view></router-view> </v-main>
    <v-footer dark padless>
      <v-card class="flex" flat tile>
        <v-card-text class="py-2 white--text text-center">
          {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "App",
  components: {},
  data: () => ({}),
};
</script>
