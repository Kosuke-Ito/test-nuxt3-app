<template>
  <nav>
    <NuxtLink class="nav-item" href="/">Home</NuxtLink>
    <NuxtLink class="nav-item" href="/about">About</NuxtLink>
    <NuxtLink class="nav-item" :to="{ name: 'users-list' }">User List</NuxtLink>
    <NuxtLink class="nav-item" to="https://google.com" target="_blank">Google</NuxtLink>
    <NuxtLink to="/posts">Post List</NuxtLink>
  </nav>
</template>

<style scoped>
a {margin-right: 1rem;}
</style>