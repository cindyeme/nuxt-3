<template>
  <div>
    <h2 class="h2">About</h2>
    <p class="p">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum
      aspernatur ex voluptate illo voluptatum nisi quas ducimus laboriosam
      sapiente praesentium incidunt repellendus ipsum, hic laborum tenetur
      tempora facere quam quis!
    </p>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Impedit facilis,
      quia odio ab velit voluptates hic et quae esse sed.
    </p>
    <div>{{ data }}</div>
  </div>
</template>

<script setup>
const { data } = await useFetch(`/api/route`);
</script>

<style scoped>
.h2 {
  margin-bottom: 20px;
  font-size: 36px;
}
.p {
  margin: 20px 0;
}
</style>
