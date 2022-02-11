<template>
  <div class="hero-section">
    <v-container>
      <v-row class="text-center my-14" justify="space-around">
        <v-col cols="12" sm="12" md="6" lg="4" xl="4">
          <v-card elevation="2" color="#1F7087" dark class="pa-8">
            <v-card-subtitle class="text-h5">Загрузить фото своего интерьера.</v-card-subtitle>
            <v-card-title class="justify-center my-8">
              <v-icon class="text-h2">mdi-image-plus</v-icon>
            </v-card-title>
            <v-card-actions>
              <v-btn text>
                Загрузить
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
        <v-col cols="12" sm="12" md="6" lg="4" xl="4">
          <v-card elevation="2" color="#1F7087" dark class="pa-8">
            <v-card-subtitle class="text-h5">Выбрать картину в свой интерьер.</v-card-subtitle>
            <v-card-title class="justify-center my-8">
              <v-icon class="text-h2">mdi-image</v-icon>
            </v-card-title>
            <v-card-actions>
              <v-btn text>
                В галерею
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
  export default {
    name: 'Home',

    data: () => ({

    }),
  }
</script>

<style scoped>
.hero-section {
  background-color: #ECEFF1;
}
</style>