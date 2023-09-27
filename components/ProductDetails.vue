<template>
  <div class="card p-10">
    <div class="grid grid-cols-2 gap-10">
      <div>
        <img
          :src="product.image"
          alt="product image"
          class="mx-auto my-7 max-w-[400px]"
        />
      </div>
      <div class="p-7">
        <p class="font-bold text-3xl mb-2">{{ product.title }}</p>
        <p class="text-xl text-red-300">${{ product.price }}</p>
        <p class="text-base mt-5">{{ product.description }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
const { product } = defineProps(['product']);
</script>

<style scoped></style>
