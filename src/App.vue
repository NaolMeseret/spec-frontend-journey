<script setup>
import { ref } from "vue"

const count = ref(0)

const increase = () => {
  count.value++
}

const decrease = () => {
  if (count.value > 0) {
    count.value--
  }
}
</script>

<template>
  <div class="counter">
    <h1>COUNT</h1>
    <h2>{{ count }}</h2>

    <button @click="increase">+</button>

    <button @click="decrease" :disabled="count === 0">–</button>
  </div>
</template>

<style scoped>
.counter {
  text-align: center;
  margin-top: 50px;
}

button {
  font-size: 20px;
  margin: 5px;
  padding: 10px 20px;
}
</style>
