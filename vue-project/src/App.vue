<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>

    <div class="wrapper">

      <nav>
        <RouterLink tag= "smth"to="/">Pick Toppings</RouterLink>
        <div></div>
        <RouterLink tag = "smth"to="/about">Shopping Cart</RouterLink>
      </nav>
    </div>
 

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
