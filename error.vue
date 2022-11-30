<template>
  <div class="mt-7 max-w-sm mx-auto text-center card">
    <p class="mt-7 text-7xl font-bold">{{ error.statusCode }}</p>
    <p class="mt-7 text-6xl"></p>
    <p class="mt-7 notFound">{{ error.message }}</p>
    <button class="btn my-7" @click="handleClearError">Go Home...</button>
  </div>
</template>

<script setup>
  defineProps(['error'])

  const handleClearError = () => clearError({ redirect: '/' })
</script>

<style scoped>
  .card {
    background-color: #999;
    max-width: 25%;
    margin: auto;
    font-size: 4.5rem;
    margin-top: 28px;
  }
  .notFound {
    font-size: 2.5rem;
    margin-top: 28px;
  }
  .btn {
    font-size: 2rem;
    padding: 20px;
    background-color: black;
  }
  .btn:hover {
    background-color: white;
    color: black;
  }
</style>