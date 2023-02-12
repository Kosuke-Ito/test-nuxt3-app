<script setup>
const { data: posts, error } = await useFetch(
  'https://jsonplaceholder.typicode.com/posts/'
);
console.log(('error', error.value));
</script>

<template>
  <div>
    <h1>Posts一覧</h1>
    <ul>
      <li v-for="post in posts" :key="post.id">{{ post.title }}</li>
    </ul>
  </div>
</template>