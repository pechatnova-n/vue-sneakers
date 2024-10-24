<script>
export default {
  data() {
    return {
      count: 0,
    }
  },
  methods: {
    increment() {
      this.count++;
    }
  }
}
</script>

<template>
  <p>{{  count  }}</p>
  <button @click="increment">+</button>
  <input v-model="count" />
</template>

<style scoped>

</style> 

