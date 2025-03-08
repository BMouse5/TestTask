<template>
  <div class="square" @click="switchTheme" :class="{light: isDark, dark: !isDark}"></div>
</template>

<script setup>
import { ref } from 'vue';

const isDark = ref(false)

const switchTheme = () => {
  isDark.value = !isDark.value
  document.body.classList.toggle('dark', isDark.value)
}
</script>

<style>
.square {
    width: 20vw;
    height: 20vw;
    background-color: black;
    transition: all 0.3;
}

.square.light {
  background: white;
}

.square:hover {
  background-color: rgb(64, 64, 64);
}

body.dark {
  background: black;
}

</style>