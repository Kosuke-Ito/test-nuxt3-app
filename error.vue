<template>
  <NuxtLayout>
    <p>{{ error }}</p>
    <button @click="clearError({ redirect: '/' })">Clear Error</button>
    
    <button @click="clearError">Clear Error2</button>
  </NuxtLayout>
</template>

<script setup>
const error = useError();
const props = defineProps({
  error: Object,
});
</script>