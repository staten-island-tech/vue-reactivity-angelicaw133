<script setup>
import { RouterView } from 'vue-router'
</script>

<template>

  <RouterView />
</template>

<style scoped>
nav {
  align-items: center;
  width: 100%;
  text-align: center;
  position: absolute;
  left: auto;
  margin-top: 6rem;
 

}
nav smth:hover,
nav smth:active {
  background-color: lightpink;
  cursor: pointer;
}


</style>
