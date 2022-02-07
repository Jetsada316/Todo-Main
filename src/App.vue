<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="http://3.bp.blogspot.com/-tUfCqpLuMMI/Vl-mHSIAzqI/AAAAAAAAAJk/YWKjEsSgP5g/s1600/d7401ad0a9f0b32582bbbeb283d236df-d4zln7u.png"
          transition="scale-transition"
          width="60"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn to="/"  text>
        <span class="mr-2">Home</span>
      </v-btn>
       <v-btn to="/about"  text>
        <span class="mr-2">about</span>
      </v-btn>
       <v-btn to="/Todo"  text>
        <span class="mr-2">Todo</span>
      </v-btn>
    </v-app-bar>
    

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    //
  }),
};
</script>
