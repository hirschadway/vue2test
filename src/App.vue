<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />
      </div>

      <v-spacer></v-spacer>
      <span>Created by Tesla</span>
      <v-spacer></v-spacer>

      <v-btn href="#" target="_blank" text>
        <span class="mr-2 hidden-sm-and-down">Technosun</span>
        <!-- <v-icon>mdi-open-in-new</v-icon> -->
      </v-btn>

      <v-img
        alt="Vuetify Name"
        class="shrink mt-1"
        contain
        min-width="100"
        src="./assets/technosun-logo-rebranding-50.png"
        width="120"
      />
    </v-app-bar>

    <v-main>
      <HelloWorld style="display: none" />
      <Home />
      <Profile />
      <v-autocomplete v-model="values" :items="items"> </v-autocomplete>
    </v-main>

    <v-footer app>
      <!-- -->
      <p>this is footer for testing</p>
      <hr />
      <p style="display: block">Cteated by Hirsch adway</p>
    </v-footer>
  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import Home from "./components/Home";
import Profile from "./components/Profile";
export default {
  name: "App",

  components: {
    HelloWorld,
    Home,
    Profile,
  },

  data: () => ({
    items: ["life", "good", "boo", "foo", "hirsch", "javad"],
  }),
};
</script>
