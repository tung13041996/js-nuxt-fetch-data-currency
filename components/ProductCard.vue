<template>
  <div v-if="product" class="card text-center">
    <NuxtLink :to="`/products/${product.id}`">
      <img :src="`${product.image}`" alt="Product image" class="thumb" />
      <p class="font-bold text-gray/500 m4 truncate">{{ product.title }}</p>
      <p class="btn">View more</p>
    </NuxtLink>
  </div>
</template>

<script setup>
const { product } = defineProps(["product"]);
</script>

<style scoped>
.thumb {
  max-height: 120px;
  height: 100%;
  max-width: 70%;
  margin: 0 auto;
  object-fit: contain;
}
</style>
