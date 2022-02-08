<template>
  <v-app>
    <v-navigation-drawer
            v-model="drawer"
            absolute
            temporary
            app
    ></v-navigation-drawer>
    <v-app-bar
      app
      color="teal darken-2"
      dark
    >
      <v-container fluid class="mx-2 mx-sm-4 mx-md-6 mx-lg-8 mx-xl-10">
        <v-row>
          <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
          <div class="d-flex align-center ml-2 ml-sm-4 ml-md-6 ml-lg-8 ml-xl-10">
            <span class="text-h6 font-weight-bold">PhotoPrint</span>
          </div>
          <v-spacer></v-spacer>
        </v-row>
      </v-container>
    </v-app-bar>

    <v-main></v-main>
  </v-app>
</template>

<script>


export default {
  name: 'App',

  components: {
  },

  data: () => ({
    drawer: false
  }),
};
</script>
