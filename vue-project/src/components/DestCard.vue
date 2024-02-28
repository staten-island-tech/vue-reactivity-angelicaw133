<template>
    <div class="container">
        <h2>{{ item.name }}</h2>
        <img :src="item.image" alt="">
        <h3>{{ "$" + item.price }}</h3>
        <button @click="counter++">Add to Cart</button>
        <p>Count is: {{ counter }}</p>

    </div>
</template>

<script setup>
const counter = ref(0)
const props = defineProps({
    item : Object
    
})
import { ref } from 'vue'


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