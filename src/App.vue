<script setup>
import MyHello from './components/MyHello.vue';
</script>

<template>
  <MyHello title="Кросовки Nike" :price="15000" :isAdded="true">
    <button>Добавить</button>
  </MyHello>

  <MyHello title="Кросовки Puma" :price="10000" :isAdded="false" />
  <MyHello>
    <h4>доп инфо</h4>
  </MyHello>
</template>

<style scoped>
</style>
