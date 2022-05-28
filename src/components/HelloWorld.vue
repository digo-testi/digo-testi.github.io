<template>
  <v-container>
    <v-row class="text-center">
      <v-col class="mt-7">
        <h1 class="display-2 font-weight-bold">Samylla</h1>
      </v-col>
    </v-row>
    <div class="d-flex justify-center mt-2">
      <v-img
        :src="require('../assets/samy.jpg')"
        class="samyImage mt-2 rounded-circle"
        contain
        max-width="320"
      />
    </div>
    <v-row class="text-center mb-5">
      <v-col cols="12" class="mt-4">
        <div class="mr-2 ml-2">
          <h2 class="mb-3">Você conhece essa beldade?</h2>
          <p class="font-weight-bold">
            Ela entrou na minha vida de repende, no momento que eu menos
            esperava.
          </p>
          <p class="font-weight-bold">
            Logo de cara me encantou o seu jeito, não tinha medo de demonstrar o
            que estava sentindo.
          </p>
          <p class="font-weight-bold">
            Dava pra notar no seu olhar que estava se entregando de coração.
          </p>
          <p class="font-weight-bold">
            De repende já estava amando...
          </p>
        </div>
      </v-col>

      <v-col>
        <h2 class="mb-2">Quer namorar comigo?</h2>
        <v-btn @click="noButton = 'Vai sim'" color="primary" class="mr-2">
          <v-icon left>mdi-thumb-down</v-icon>
          {{ noButton }}
        </v-btn>
        <v-btn color="primary">
          <v-icon left>mdi-thumb-up</v-icon>
          Sim
        </v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "HelloWorld",

  data: () => ({
    noButton: "Não",
  }),
});
</script>

<style scoped>
.samyImage {
  width: 70%;
}
</style>
