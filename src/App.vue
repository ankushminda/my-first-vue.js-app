<template>
  <div class="app">
    <h1>Vue Counter App 🔢</h1>
    
    <p>Current Count: <strong>{{ count }}</strong></p>
    
    <button @click="count++">➕ Increment</button>
    <button @click="count--">➖ Decrement</button>
    <button @click="reset">♻️ Reset</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)

function reset() {
  count.value = 0
}
</script>

<style>
.app {
  font-family: Arial, sans-serif;
  text-align: center;
  margin-top: 50px;
}
button {
  margin: 5px;
  padding: 10px 15px;
  font-size: 16px;
  cursor: pointer;
}
</style>
