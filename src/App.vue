<script setup>
import { RouterView } from 'vue-router'
</script>

<template>
  <div class="app">
    <RouterView />
  </div>
</template>
<style scoped>
.app {
  display: flex;
  flex-direction: column;
  /* height: 100vh; */
  /* overflow: hidden; */
  width: 100%;
  position: relative;
}
</style>
