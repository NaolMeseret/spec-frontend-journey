<script setup>
import UserCard from "./components/UserCard.vue"
</script>

<template>
  <div class="container">
    <UserCard name="Alemayew" role="Frontend Developer" />
    <UserCard name="Naol" role="Vue.js Learner" />
    <UserCard name="Natnael" role="UI Designer" />
  </div>
</template>

<style scoped>
.container {
  display: flex;
  gap: 20px;
  justify-content: center;
  margin-top: 40px;
}
</style>
