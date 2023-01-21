<template>
  <div>
    <h2>Abouts</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel, cumque magni
      facilis repellendus ratione dolorem nesciunt? Atque error non totam!
    </p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel, cumque magni
      facilis repellendus ratione dolorem nesciunt? Atque error non totam!
    </p>

    <p>{{ data }}</p>
  </div>
</template>

<script setup>
const { data } = await useFetch("/api/currency/NGN");
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
