<template>
  <div>
    <h1>Usersページ</h1>
    <NuxtPage />
  </div>
</template>

<script setup>
const resetError = (error) => {
  error.value = null;
};
</script>