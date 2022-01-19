<template>
  <div class="app-container">
    <Nav />
    <div class="app-content">
      <Nuxt />
    </div>
  </div>
</template>

<script>
import Nav from "../components/Nav.vue";

export default {
  components: {
    Nav,
  },
};
</script>

<style>
body {
  margin: 0;
  height: 100%;
  width: 100%;
  background: rgb(243,243,155);
background: linear-gradient(90deg, rgba(243,243,155,1) 0%, rgba(199,201,103,1) 35%, rgba(139,165,92,1) 100%);
  

  font-family: Arial, Helvetica, sans-serif;
}

</style>
