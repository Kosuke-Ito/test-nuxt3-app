<template>
  <div>
    <h1>Main Page</h1>
    <h2>{{ data }}</h2>
  </div>
</template>

<script setup>
const { data } = useFetch('/api/hello');
</script>