<template>
  <div>
    <v-container>
      <v-row style="height: 150px">
        <v-col
          cols="12"
          sm="4"
          v-for="(character, index) in Personajes" :key="index"
        >
          <Card :Character="character" ></Card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import Personajes from "../personajes.js";

export default {
  name: "IndexPage",

  data() {
    return {
      Personajes: Personajes,
    };
  },
};
</script>
