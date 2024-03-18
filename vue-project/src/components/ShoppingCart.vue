<template>
    <div class="shopping">
        <h1>In Cart</h1>
     

    </div>       

</template>

<script setup>
const checkout = [

];
console.log(checkout);
const props = defineProps({
    cart: Array
})
</script>

<style scoped>

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