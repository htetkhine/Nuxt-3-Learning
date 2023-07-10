<template>
    <div class="py-5">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h3>{{ product.title }}</h3>
                    <p>{{ product.price }}</p>
                    <p>{{ product.id }}</p>
                </div>
            </div>
        </div>        
    </div>
</template>

<script setup>
    const {id} = useRoute().params
    const url = 'https://fakestoreapi.com/products/' + id
    const { data:product} = await useFetch(url);
</script>

<style lang="scss" scoped>

</style>