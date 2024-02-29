<template>
    <div class="shopping">
        <h1>In Cart</h1>
        <p>Count is: {{ counter }}</p>
    </div>       

</template>

<script setup>
const props = defineProps({
    Shopping : Object
})
import counter from './DestCard.vue'
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