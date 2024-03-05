<template>
    <div class="container">
        <h2>{{ item.name }}</h2>
        <img :src="item.image" alt="">
        <h3>{{ "$" + item.price }}</h3>
        <button @click="add(item)">Add to Cart</button>
        

    </div>
</template>

<script setup>
import {checkout} from '@/stores/CheckOut'
function add(item) {
    checkout.cart.push(item);
}
const props = defineProps({
    item : Object
})


</script>

<style scoped>
.container {
    font-family: "Open Sans", sans-serif;
	display: flex;
	align-items: center;
 	flex-wrap: wrap;
    flex-direction: row;
    width: 100vw;
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