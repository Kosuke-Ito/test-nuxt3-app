<template>
  <div>
    <h1>Main Page</h1>
    <h2>{{ $hello('World') }}</h2>
    <button @click="handleClick">Coupon Get</button>
    <LazyCoupon v-if="show" />
    <div>
      <img src="~/assets/icon.png" alt="Nuxt3 Icon" />
    </div>
    <div>
      <img src="/icon.png" alt="Nuxt3 Icon" />
    </div>
    <div>Count:{{ count }}</div>
    <div>
      <button @click="() => inc()">increase</button>
      <button @click="() => dec()">decrease</button>
    </div>
  </div>
</template>
<script setup>
const show = ref(false);
const { count, inc, dec } = useCounter(100);
const { $hello } = useNuxtApp();

const handleClick = () => {
  show.value = true;
};
</script>