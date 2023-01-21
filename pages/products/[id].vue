<template>
  <div>
    <p>product id for {{ id }}</p>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusamus sint
      sequi ducimus animi beatae distinctio quisquam. Rerum autem fugit
      reprehenderit.
    </p>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
</script>

<style scoped></style>
