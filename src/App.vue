<script setup>
import { ref } from 'vue'

const contador = ref(0)
function incrementar() {
  contador.value++
}
function decrementar() {
  contador.value--
}
function zero() {
    contador.value -= contador.value;
}

</script>

<template>
  <h1>Meu contador</h1>
  <p>Valor do contador: {{ contador }}</p>
  <button v-on:click="incrementar">+</button>
  <button @click="decrementar">-</button>
  <button @click="zero">zerar</button>
</template>

<style scoped>

</style>
