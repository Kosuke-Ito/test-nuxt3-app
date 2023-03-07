<template>
  <div>
    <Head>
      <Title>Aboutページ</Title>
      <Meta name="description" content="Aboutページ" />
    </Head>
    <h1>About Page</h1>
    <h2>Counter</h2>
    <p>Count: {{ counter }}</p>
    <div>
      <button @click= "counter++">+</button>
    </div>
  </div>
</template>

<script setup>
const title = ref('Aboutページ');
const description = ref('Aboutページ');
const counter = useCounter();

useHead({
  title,
  meta: [
    {
      name: description,
      content: 'Aboutページ',
    },
  ],
});

definePageMeta({
  middleware: 'auth',
});
</script>