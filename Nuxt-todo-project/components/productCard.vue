<template>
    <div class="card">
        <img :src="product.image" alt="product thumb" srcset="thumb">
        <div class="card-body">
            <nuxt-link :to="`/products/${product.id}`">{{ product.title }}</nuxt-link>
        </div>
        <NuxtLink :to="`/products/${product.id}`"><p class="btn btn-success">View More</p></NuxtLink>       
    </div>
</template>

<script setup>
    const {product} = defineProps(['product'])  
</script>

<style lang="scss" scoped>

</style>