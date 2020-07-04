<template>
  <v-app>
    <v-app-bar app color="deep-purple darken-4" dark>
    <router-link to="/" style="color:white;text-decoration:none;"><span>MUSIC SEARCH</span></router-link>
      <div class="d-flex align-center">
</div>
      <v-spacer></v-spacer>
      <v-btn
        text
        to="/">
        <span class="mr-2">Home</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>
    <v-content>
      <router-view>
      <HelloWorld/>
      </router-view>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
