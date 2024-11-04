<script setup>
import Card from './Card.vue';

defineProps({
  items: Array
})

const onClickAdd = () => {
  alert(111)
}

const onClickFavourite = () => {
  alert(222)
}

</script>
<template>
  <div class="grid grid-cols-4 gap-5">

    <Card 
    v-for="item in items"
    :key="item.id"
    :title=item.title
    :price=item.price
    :imageUrl=item.imageUrl 
    isAdded='false' 
    isFavirite="false" 
    :onClickAdd="onClickAdd"
    :onClickFavourite="onClickFavourite"
    />
  </div>
</template>
