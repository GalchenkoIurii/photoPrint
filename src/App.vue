<template>
  <v-app>
    <v-navigation-drawer
            v-model="drawer"
            absolute
            temporary
            app
    >
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-h6">
            PhotoPrint
          </v-list-item-title>
          <v-list-item-subtitle>
            Сервис примерки фотографий
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list
              dense
              nav
      >
        <v-list-item
                v-for="(item, i) in navItems"
                :key="i"
                link
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-divider></v-divider>
      <v-list
              dense
              nav
      >
        <v-list-item
                link
        >
          <v-list-item-icon>
            <v-icon>mdi-login</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Вход</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item
                link
        >
          <v-list-item-icon>
            <v-icon>mdi-account-plus</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Регистрация</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item
                link
        >
          <v-list-item-icon>
            <v-icon>mdi-logout</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Выход</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
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
    drawer: false,
    navItems: [
        {
            title: 'Загрузить фото',
            icon: 'mdi-image-plus'
        },
        {
            title: 'Выбрать фото',
            icon: 'mdi-image'
        },
        {
            title: 'Категории фото',
            icon: 'mdi-image-multiple'
        },
        {
            title: 'О сервисе',
            icon: 'mdi-help-box'
        }
    ]
  }),
};
</script>
