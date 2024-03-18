<template>
    <div class="container">
        <h2>{{ item.name }}</h2>
        <img :src="item.image" alt="">
        <h3>{{ "$" + item.price }}</h3>
        <button @click="add(item)">Add to Cart</button>
        

    </div>
</template>

<script setup>
import checkout from '@/views/ShoppingCart.vue'
function add(item_) {
    checkout.cart.push(item_);
    console.log(checkout+"");
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