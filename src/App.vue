<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0)

  function increment() {
    count.value++
  }

  function decrement() {
    count.value--
  }
</script>

<template>
  <h1>Counter</h1>
  <div class="app">
    <button id="resultat">{{ count }}</button><br />
    <button id="increment" @click="increment">+</button><br />
    <button id="decrement" @click="decrement">-</button>
  </div>
</template>

<style scoped>
.app {
  text-align: center;
}

#resultat {
  font-size: 100px;
  width: 140px;
  padding: 5px;
} 
#increment, #decrement {
  color: white;
  font-size: 100px;
  width: 140px;
  padding: 5px; 
}
#increment {
  background-color: green;
}
#decrement {
  background-color: red;
  
}
</style>
