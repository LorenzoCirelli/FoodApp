<template>
  <h1 class="barra">
    {{ nomeApp }}
  </h1>
  <slot></slot>
</template>
<script setup lang="ts">
const nomeApp = import.meta.env.VITE_APP_NAME
</script>
<style scoped lang="scss">
.barra {
  padding: 10px;
  color: white;
  font-size: medium;
  position: fixed;
  top: 0;
  width: 100%;
  background-color: $verdeBase;
}
</style>
