<template>
  <v-app theme="dark">
    <v-navigation-drawer v-model="isDrawerOpen">
      <v-list>
        <v-list-subheader>Menu</v-list-subheader>
        <v-list-item prepend-icon="mdi-home"> Home </v-list-item>
        <v-list-item prepend-icon="mdi-account"> Usuários </v-list-item>

        <v-list-group value="Clientes">
          <template #activator="{ props }">
            <v-list-item v-bind="props" prepend-icon="mdi-account-circle"
              >Clientes</v-list-item
            >
          </template>

          <v-list-item prepend-icon="mdi-currency-usd">Faturamento</v-list-item>
          <v-list-item prepend-icon="mdi-chart-line">Relatório</v-list-item>
        </v-list-group>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar flat class="border-b">
      <v-app-bar-nav-icon
        @click="isDrawerOpen = isDrawerOpen = !isDrawerOpen"
      ></v-app-bar-nav-icon>
      <v-app-bar-title></v-app-bar-title>

      <template #append>
        <v-btn icon class="mr-1">
          <v-badge dot color="info">
            <v-icon icon="mdi-bell-outline"></v-icon>
          </v-badge>
        </v-btn>

        <v-menu>
          <template #activator="{ props }">
            <v-avatar v-bind="props">
              <v-img cover src="../src/img/portrait.png"></v-img>
            </v-avatar>
          </template>

          <v-card min-width="200px">
            <v-list :lines="false" density="compact" nav>
              <v-list-item prepend-icon="mdi-account-outline">
                <v-list-item-title>Meu Perfil</v-list-item-title>
              </v-list-item>

              <v-list-item prepend-icon="mdi-heart-outline">
                <v-list-item-title>Favoritos</v-list-item-title>
              </v-list-item>
            </v-list>
          </v-card>
        </v-menu>
      </template>
    </v-app-bar>
    <v-main>
      <v-container>
        <h1>Dashboard</h1>

        <v-card flat class="border" mg-4>
          <v-table density="compact">
            <tbody>
              <tr>
                <td>Teste</td>
              </tr>
              <tr>
                <td>Teste</td>
              </tr>
            </tbody>
          </v-table>
        </v-card>

        <v-row>
          <v-col cols="12" sm="6" md="4" lg="3">
            <v-card flat class="border">
              <v-img class="align-end text-white" src="../src/img/img1.jpeg">
                <v-card-title>Top 10 Lugares</v-card-title>
              </v-img>
              <v-card-subtitle class="pt-3">Brasil RJ</v-card-subtitle>
              <v-card-text>
                <div>Rio De Janeiro</div>
                <div>Lorem Ipsum</div>
              </v-card-text>
              <v-card-actions>
                <v-btn variant="outlined" color="primary">Ver mais</v-btn>
                <v-btn prepend-icon="mdi-cart" variant="tonal" color="blue"
                  >Comprar</v-btn
                >
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6" md="4" lg="3">
            <v-card flat class="border">
              <v-img class="align-end text-white" src="../src/img/img1.jpeg">
                <v-card-title>Top 10 Lugares</v-card-title>
              </v-img>
              <v-card-subtitle class="pt-3">Brasil RJ</v-card-subtitle>
              <v-card-text>
                <div>Rio De Janeiro</div>
                <div>Lorem Ipsum</div>
              </v-card-text>
              <v-card-actions>
                <v-btn variant="outlined" color="primary">Ver mais</v-btn>
                <v-btn prepend-icon="mdi-cart" variant="tonal" color="blue"
                  >Comprar</v-btn
                >
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6" md="4" lg="3">
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
                <v-btn prepend-icon="mdi-cart" variant="tonal" color="blue"
                  >Comprar</v-btn
                >
              </v-card-actions>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6" md="4" lg="3">
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
                <v-btn prepend-icon="mdi-cart" variant="tonal" color="blue"
                  >Comprar</v-btn
                >
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
    isDrawerOpen: false,
  }),
};
</script>
