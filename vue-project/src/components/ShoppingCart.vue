<template>
    <div class="shopping">
        <h1>In Cart</h1>
        <p> class = "item_number">Count is: {{ counter_ }}</p>

    </div>       

</template>

<script setup>
import {ref} from 'vue'
import counter_ from './DestCard.vue'
// import counter from './DestCard.vue'
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