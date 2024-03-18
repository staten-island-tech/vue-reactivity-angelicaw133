<template>
    <div class="container2">
        <h1>Checkout</h1>
        <h2>Add an Item to Cart</h2>
    </div>
</template>

<script setup>
import {checkout} from "@/stores/checkout.js"
const props = defineProps({
    cart:Array
})
</script>

<style>

</style>