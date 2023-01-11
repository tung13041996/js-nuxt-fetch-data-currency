<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container mx-auto p-4 flex">
        <NuxtLink to="/products" class="font-bold">Bach to Home page</NuxtLink>
      </nav>
    </header>

    <!-- Input content page -->
    <div class="container">
      <slot />
    </div>

    <footer class="container mx-auto p-4 flex justify-between border-t-2">
      <ul class="flex gap-4">
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li><NuxtLink to="/products">Products</NuxtLink></li>
      </ul>
    </footer>
  </div>
</template>

<script setup></script>

<style scoped>
header ul li a {
  text-decoration: none;
  color: #000;
  font-size: 18px;
}
.router-link-exact-active {
  color: green;
}
</style>
