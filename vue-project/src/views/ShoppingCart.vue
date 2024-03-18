<template>
  <div class="shopping">
    <h1>Shopping Cart</h1>
  </div>
  <!-- <div v-for="(ingredients) in checkout.cart":key="ingredients.name">
  <h2>{{ ingredient.name }}</h2>
  </div> -->
</template>
<script setup>
const checkout = [

];
const props = defineProps({
    cart: Array
})
console.log(cart)
</script>
<style>
*{
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}
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
    width: 100%;
}
.shopping{
    font-family: "Open Sans", sans-serif;
	display: flex;
	align-items: center;
 	flex-wrap: wrap;
  width: 100%;
  text-align: center;
}
img {
    display: block;
    height: 25vh;
    padding: 1rem;
}
button  {
    margin: 1rem;
}
</style>
