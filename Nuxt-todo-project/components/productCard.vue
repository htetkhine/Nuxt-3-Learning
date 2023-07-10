<template>
    <div class="card p-3 h-100 mt-3">
        <img :src="product.image" alt="product thumb" class="img-fluid">
        <div class="card-body">
            <nuxt-link :to="`/products/${product.id}`">{{ product.title }}</nuxt-link>
        </div>
        <NuxtLink :to="`/products/${product.id}`"><p class="btn btn-success">View More</p></NuxtLink>       
    </div>
</template>

<script setup>
    const {product} = defineProps(['product'])  
</script>

<style scoped>
    .card{
        text-align: center;   
    }
    .card img{
        width: 100px;
        max-width: 100%; 
        margin: 0 auto;       
    }
</style>