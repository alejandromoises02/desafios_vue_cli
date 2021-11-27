<template>
  <div id="app" class="container">
    <h1>Platos Disponibles:</h1>
    <Tabla :comidas="data.comidas" />
    <h1>Bebidas:</h1>
    <Tabla :comidas="data.bebidas" />
    <h1>Postres</h1>
    <Tabla :comidas="data.postres" />
  </div>
</template>
<script>

import Tabla from "./components/Tabla.vue"

export default {
  name: 'App',
  components: {
    Tabla,
  },
  data() {
    return {
      data:{
      comidas: [
      { id: 0, name: "Pasta", description: "Acompañado de salsas", price: 500 },
      { id: 1, name: "Hamburguesa", description: "Pan, carne, lechuga, tomate", price: 300 },
      { id: 2, name: "Pizza", description: "salsa y mozzarella", price: 600 },
      { id: 3, name: "Milanesa", description: "Carne o Pollo", price: 300 }
    ],
    bebidas: [
      { id: 4, name: "Gaseosas", description: "Pepsi, Coca", price: 500 },
      { id: 5, name: "Jugos", description: "Limon, Naranja", price: 300 }
    ],
    postres: [
      { id: 6, name: "Pastel", description: "Chocolate, Vainilla", price: 500 },
      { id: 7, name: "Helados", description: "Americana, Choco, Frutilla", price: 300 }
    ]
    }}
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
