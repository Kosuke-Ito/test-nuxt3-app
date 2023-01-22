<template>
  <nav>
    <NuxtLink href="/">Home</NuxtLink>
    <NuxtLink href="/about">About</NuxtLink>
    <NuxtLink :to="{ name: 'users-list' }">User List</NuxtLink>
    <NuxtLink to="https://google.com" target="_blank">Google</NuxtLink>
  </nav>
</template>
