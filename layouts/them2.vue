<template>
    <v-app>
          <v-system-bar dark color="pink lighten-3">
      <v-spacer></v-spacer>
      <v-icon>mdi-wifi-strength-4</v-icon>
      <v-icon>mdi-signal-cellular-outline</v-icon>
      <v-icon>mdi-battery</v-icon>
      <span>12:30</span>
    </v-system-bar>
    <div>
         <v-app-bar
      color="#EC407A"
      dark
    >
<nuxt-link to="one">
     <v-btn icon>
        <v-icon>arrow_back</v-icon>
      </v-btn>
 </nuxt-link>

      <v-toolbar-title>Welcome</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-menu
        bottom
        left
      >
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            icon
            color="yellow"
            v-bind="attrs"
            v-on="on"
          >
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>
      </v-menu>

    </v-app-bar>
    <v-tabs
    fixed-tabs
    background-color="#EC407A"
    dark
    color="#FFFFFF"
  >
    <v-tab>
      SING UP
    </v-tab>
    <v-spacer></v-spacer>
    <v-tab>
      SING IN
    </v-tab>
  </v-tabs>
    </div>
    
        <v-main>
            <v-content>
                <nuxt/>
            </v-content>
        </v-main>
    </v-app>
</template>