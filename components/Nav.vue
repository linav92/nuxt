<template>
  <div>
    <v-app-bar color="#2E6859" dark>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>Rick & Morty</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn elevation="0" color="#2E6859"><nuxt-link to="/" class="link">Inicio</nuxt-link></v-btn>
        <v-btn elevation="0" color="#2E6859"><nuxt-link to="/buscar" class="link">Buscar</nuxt-link></v-btn>
        <v-btn elevation="0" color="#2E6859"><nuxt-link to="/acercaDe" class="link">Acerca de</nuxt-link></v-btn>
      </v-toolbar-items>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" absolute left temporary color="#2E6859">
      <v-list nav dense dark>
        <v-list-item-group
          active-class="teal--text text--darken-4"
        >
          <v-list-item>
            <v-list-item-title><nuxt-link to="/" class="link">Inicio</nuxt-link></v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title><nuxt-link to="/buscar" class="link">Buscar</nuxt-link></v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title><nuxt-link to="/acercaDe" class="link">Acerca de</nuxt-link></v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>


<script>
export default {
  data: () => ({
    drawer: false,
  }),
};
</script>

<style scoped>
.link{
  text-decoration: none;
  color: white;
}
</style>

