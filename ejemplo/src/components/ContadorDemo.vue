<template>
  <div class="contenedor">
    <h2>Componente de prueba</h2>

    <p>Contador actual: {{ contador }}</p>

    <button @click="incrementar">Incrementar</button>
    <button @click="reiniciar">Reiniciar</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const contador = ref(0)

function incrementar() {
  contador.value++
}

function reiniciar() {
  contador.value = 0
}
</script>

<style scoped>
.contenedor{
  border:1px solid #ccc;
  padding:20px;
  margin-top:20px;
  border-radius:10px;
}
button{
  margin-right:10px;
}
</style>