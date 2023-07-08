<template>
    <div>    
        <header>
            <nuxt-link to="/">Home</nuxt-link>
            <nuxt-link to="/about">About</nuxt-link>
            <nuxt-link to="/products">Products</nuxt-link>
        </header>
        <div>
            <slot/>
        </div>        
    </div>
</template>

<script setup>
 
</script>

<style lang="scss" scoped>

</style>