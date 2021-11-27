<template>
  <table class="table">
    <thead>
      <tr>
        <th scope="col">Descripcion</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="comida in comidas" :key="comida.id">
        <Card :comida="comida" />
      </tr>
    </tbody>
  </table>
</template>

<script>
import Card from "./Card.vue";

export default {
  name: "Tabla",
  components: {
    Card
  },
  props: {
    comidas: Array,
    default: () => {}
  }
};
</script>

<style scoped></style>
