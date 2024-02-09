<template>
    <div class="container">
        <h2>{{ item.name }}</h2>
        <img :src="item.image" alt="">
        <h3>{{ "$" + item.price }}</h3>

    </div>
</template>

<script setup>
const props = defineProps({
    item : Object
})
</script>

<style scoped>
.container {
    
}
</style>