<template>
    <div class="container">
        <h2>{{ ingredient.name }}</h2>
        <img :src="ingredient.image" alt="">
        <h3>{{ "$"+ ingredient.price }}</h3>
        <button>Add to Cart!</button>
    </div>
</template>

<script setup>
import {checkout} from '@/stores/checkout.js'
const props = defineProps({
    ingredient: Object
})
</script>

<style>
.container {
    font-family: "Open Sans", sans-serif;
	display: flex;
	flex-direction: row;
	align-items: center;
 	flex-wrap: wrap;
}
img {
    display: block;
    width: 30vw;
  padding: 1rem;
}
button{
    margin: 1rem;
}
</style>