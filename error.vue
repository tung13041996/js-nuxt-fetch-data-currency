<template>
  <div>
    <div class="mt-7 max-w-sm mx-auto txt-center card text-center">
      <p class="mt-7 font-bold">{{ error.statusCode }}</p>
      <p class="mt-7">Ooops.</p>
      <p>{{ error.message }}</p>
      <button class="btn" @click="handleClick">Go home</button>
    </div>
  </div>
</template>

<script setup>
defineProps(["error"]);

const handleClick = () => {
  clearError({
    redirect: "/",
  });
};
</script>

<style scoped></style>
