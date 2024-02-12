<template>
    <div class="container">
        <h2>{{ item.name }}</h2>
        <img :src="item.image" alt="">
        <h3>{{ "$" + item.price }}</h3>
        <button></button>

    </div>
</template>

<script setup>
const props = defineProps({
    item : Object
})
</script>

<style scoped>
.container {
    font-family: "Open Sans", sans-serif;
	display: flex;
	flex-direction: row;
	align-items: center;
 	flex-wrap: wrap;

}
img {
    display: block;
    height: 25vh;
  padding: 1rem;
}
</style>