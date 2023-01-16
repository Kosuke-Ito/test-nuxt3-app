<template>
  <div>
    <NuxtLayout name="default">
      <template #header>ヘッダー</template>
      <h1>Main Page</h1>
    </NuxtLayout>
  </div>
</template>
<script setup>
definePageMeta({
  layout: true,
});
</script>