<template>
  <div>
    <button @click="enableCustomLayout">Update layout</button>
  </div>
</template>
<script setup>
const title = ref('Aboutページ');
const description = ref('Aboutページ');

useHead({
  title,
  meta: [
    {
      name: description,
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