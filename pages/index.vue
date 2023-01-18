<template>
  <div>
    <h1>Main Page</h1>
    <button @click="handleClick">Coupon Get</button>
    <LazyCoupon v-if="show" />
    <div>
      <img src="~/assets/icon.png" alt="Nuxt3 Icon" />
    </div>
  </div>
</template>
<script setup>
const show = ref(false);

const handleClick = () => {
  show.value = true;
};
</script>