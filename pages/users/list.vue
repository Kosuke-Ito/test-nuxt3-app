<template>
  <div>
    <h1>ユーザリスト</h1>
    <ul>
      <li v-for="user in users" :key="user.id">{{ user.name }}</li>
    </ul>
  </div>
</template>

<script setup>
const { data: users } = await useFetch(
  'https://jsonplaceholder.typicode.com/user/'
);
console.log('process');
if (!users.value) {
  throw createError({ statusCode: 404, statusMessage: 'Page Not Found' });
}
</script>