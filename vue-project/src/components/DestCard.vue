<template>
    <div class="container">
        <h2>{{ item.name }}</h2>
        <img :src="item.image" alt="">
        <h3>{{ "$" + item.price }}</h3>
        <button @click="counter++">Add to Cart</button>
        

    </div>
</template>

<script setup>
import { ref } from 'vue'
const counter_ = ref(0)
const props = defineProps({
    item : Object
    
})
console.log(counter_)


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