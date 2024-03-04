<template>
  <v-app>
    <v-app-bar flat class="border-b">
      <app-bat-title>Meu App</app-bat-title>
    </v-app-bar>
    <v-main>
      <v-container>
        <h1>Dashboard</h1>

        <v-row>
          <v-col cols="12" md="4">
            <v-card flat class="border">
              <v-img class="align-end text-white" src="../src/img/img1.jpeg">
                <v-card-title>Top 10 Lugares no Mundo</v-card-title>
              </v-img>
              <v-card-subtitle class="pt-3">Brasil RJ</v-card-subtitle>
              <v-card-text>
                <div>Rio De Janeiro</div>
                <div>Lorem Ipsum</div>
              </v-card-text>
              <v-card-actions>
                <v-btn variant="outlined" color="primary">Ver mais</v-btn>
                <v-btn prepend-icon="mdi-cart" variant="tonal" color="blue">Comprar</v-btn>
                <v-btn icon="mdi-home" variant="tonal" color="black"></v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card flat class="border">
              <v-img class="align-end text-white" src="../src/img/img1.jpeg">
                <v-card-title>Top 10 Lugares no Mundo</v-card-title>
              </v-img>
              <v-card-subtitle class="pt-3">Brasil RJ</v-card-subtitle>
              <v-card-text>
                <div>Rio De Janeiro</div>
                <div>Lorem Ipsum</div>
              </v-card-text>
              <v-card-actions>
                <v-btn>Ver mais</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card flat class="border">
              <v-img class="align-end text-white" src="../src/img/img1.jpeg">
                <v-card-title>Top 10 Lugares no Mundo</v-card-title>
              </v-img>
              <v-card-subtitle class="pt-3">Brasil RJ</v-card-subtitle>
              <v-card-text>
                <div>Rio De Janeiro</div>
                <div>Lorem Ipsum</div>
              </v-card-text>
              <v-card-actions>
                <v-btn>Ver mais</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
      <HelloWorld />
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
