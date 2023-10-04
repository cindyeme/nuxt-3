<template>
  <div
    class="mt-7 max-w-sm mx-auto text-center flex flex-col items-center justify-center h-screen"
  >
    <p class="mt-7 text-7xl font-bold">{{ error.statusCode }}</p>
    <p class="mt-7 text-4xl">Ooops.</p>
    <p class="mt-7 text-xl">{{ error.message }}</p>
    <button class="btn mt-7" @click="handleError">Go Home</button>
  </div>
</template>

<script setup>
const error = useError();

const handleError = () => {
  clearError({
    redirect: "/",
  });
};
</script>

<style scoped></style>
