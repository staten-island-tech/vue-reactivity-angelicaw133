<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>

    <div class="wrapper">

      <nav>
        <RouterLink to="/">Pick Toppings     </RouterLink>
        <RouterLink to="/about">Shopping Cart</RouterLink>
      </nav>
    </div>
 

  <RouterView />
</template>

<style scoped>
  
</style>
