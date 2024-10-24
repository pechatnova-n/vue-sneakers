<script setup>
  const props = defineProps({
    title: String,
    price: Number,
    isAdded: Boolean,
  })

</script>

<template>
  <div class="product">
    <h2>Товар: {{ props.title }}</h2>
    <h3>Цена: {{ props.price }}</h3>
    <h3>Добавлен: {{ isAdded }}</h3>
    <slot></slot>
  </div>
</template>

<style scoped>
  .product {
    border: 1px solid #000;
    padding: 10px;
    margin-bottom: 10px;
    margin-right: 10px;
  }
</style> 

