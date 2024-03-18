<template>
  <div class="shopping">
    <h1>Shopping Cart</h1>
  </div>
</template>
<script setup>
const checkout = [

];
const props = defineProps({
    cart: Array
})
</script>
<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
h1 {
    text-align: center;
    font-size: 3rem;
}
.shopping{
    background-color: aqua;
    position: absolute;
    top: 0;
    right: 0;
    width: 40vw;
    height: 520vh;
}
</style>
