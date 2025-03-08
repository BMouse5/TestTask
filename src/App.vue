<template>
  <div class="container">
    <SquareComp></SquareComp>
  </div>
</template>
<script setup>
import SquareComp from './components/SquareComp.vue'
</script>
<style scoped>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 80vh;
}

.square {
  transition: background-color 0.3s;
}
</style>
