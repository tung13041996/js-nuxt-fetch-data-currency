<template>
  <div>
    <h2>About</h2>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quidem,
      doloremque?
    </p>
    <p>
      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quae facilis
      molestiae eligendi necessitatibus iure ea minus odio non hic sapiente!
    </p>
    <div>{{ data }}</div>
  </div>
</template>

<script setup>
const { data } = await useFetch("/api/currency/GBP");
</script>

<style scoped>
h2 {
  margin-bottom: 20px;
  font-size: 36px;
}
p {
  margin: 20px 0;
}
</style>
