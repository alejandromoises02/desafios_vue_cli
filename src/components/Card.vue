<template>
  <div class="card">
        <td>{{ comida.name }}</td>
        <td>{{ comida.description }}</td>
        <td>{{ comida.price }}</td>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
      comida: Object,
      default: () => {}
  }
};
</script>

<style scoped></style>