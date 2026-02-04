<script setup>
import { ref } from "vue"

const name = ref("")
</script>

<template>
  <div>
    <input type="text" v-model="name" placeholder="Enter your name" />

    <h2 v-if="name">Hello {{ name }}</h2>
  </div>
</template>
