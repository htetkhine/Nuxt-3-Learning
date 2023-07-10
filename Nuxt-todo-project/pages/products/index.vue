<template>
    <div class="my-5">
        <h3 class="text-center mb-5">Shop</h3>
        <div class="container">
            <div class="row">              
              <div class="col-md-3 col-sm-6 col-12" v-for="product in products" :key="product.id">
                  <productCard :product="product" />
              </div>
            </div>
        </div>
    </div>
</template>

<script setup>
    
    const { data:products} = await useFetch('https://fakestoreapi.com/products/');

</script>

<style lang="scss" scoped>

</style>