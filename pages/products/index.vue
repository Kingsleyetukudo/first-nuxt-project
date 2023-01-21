<template>
  <div>
    <div class="grid grid-cols-4 gap-5">
      <div v-for="p in products" :key="p.id">
        <ProductCard :product="p" />
      </div>
    </div>
    <p>Products</p>
  </div>
</template>

<script setup>
definePageMeta({
  layout: "products",
});

const { data: products } = await useFetch("https://fakestoreapi.com/products");

// how to add meta and head title in a page

useHead({
  title: "Nuxt 3 | products",
  meta: [{ name: "description", content: "Nuxt products page" }],
});
</script>

<style scoped></style>
