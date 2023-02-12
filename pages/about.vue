<template>
  <div>
    <button @click="enableCustomLayout">Update layout</button>
  </div>
</template>
<script setup>
useHead({
  title: 'Aboutページ',
  meta: [
    {
      name: 'description',
      content: 'Aboutページ',
    },
  ],
});

function enableCustomLayout() {
  setPageLayout('default');
}
definePageMeta({
  middleware: 'auth',
});
</script>