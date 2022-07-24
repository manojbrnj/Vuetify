<template>
  <div>
    <v-card width="400px" class="mx-auto mt-5">
      <v-card-title><h1>HelloWorld</h1> </v-card-title>
      <v-card-text>
        <v-form>
          <v-text-field
            label="username"
            prepend-icon="mdi-account"
            background-color="white"
          ></v-text-field>
          <v-text-field
            label="password"
            :type="showPass ? 'text' : 'password'"
            prepend-icon="mdi-lock"
            :append-icon="showPass ? 'mdi-eye' : 'mdi-eye-off'"
            background-color="white"
            @click:append="showPass = !showPass"
          ></v-text-field>
          <v-card-actions>
            <v-btn x-small color="success">Login</v-btn>
            <v-spacer></v-spacer>
            <v-btn x-small color="success">Register</v-btn>
          </v-card-actions>
        </v-form>
      </v-card-text>
    </v-card>
  </div>
</template>
<script>
export default {
  name: "Login",
  components: {},
  data: () => ({
    showPass: false,
    username: "",
    password: "",
    links: ["Home", "Login"],
  }),
};
</script>
<style lang=""></style>
