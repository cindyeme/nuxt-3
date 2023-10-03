<template>
  <div>
    <h2>Product details for {{ id }}</h2>
    <p>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Iste fuga illo
      obcaecati voluptates dolorum adipisci nemo, praesentium saepe! Odio,
      aliquam.
    </p>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
definePageMeta({
  layout: "products",
});
</script>

<style scoped></style>
