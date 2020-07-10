<template>
  <v-app>
      <br>
      <center>
    <v-card width="450" color="#88DDBB">
      <v-card-title-center>
        <h1>Login</h1> 
      </v-card-title-center>
      <v-card-text>

        <v-form>
          <v-text-field label="Username" prepend-icon="mdi-account-circle" />

          <v-text-field 
            :type="showPassword ? 'text' : 'password'" 
            label="Password"
            prepend-icon="mdi-lock"
            :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
            @click:append="showPassword = !showPassword"
          />
        </v-form>
      </v-card-text>

      <v-card-actions>
          <nuxt-link to="regis">
        <v-btn class="ma-2" tile color="success" dark>REGISTER</v-btn>
          </nuxt-link>
        <v-spacer></v-spacer>
        <v-btn class="ma-2" tile color="indigo" dark>LOGIN</v-btn>
      </v-card-actions>

    </v-card>
    </center>
  </v-app>
</template>
<script>
export default {
  name: 'App',
  data () {
    return {
      showPassword: false
    }
  }
}
</script>