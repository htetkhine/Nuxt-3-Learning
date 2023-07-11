<template>
    <div>
        <Head>
            <title>{{ product.title }}</title>
            <meta name="description" :content="product.description">
        </Head>    
        <div class="productDetail py-5">
            <div class="container">
                <div class="row">
                    <div class="col-6 text-center">
                        <img :src="product.image" alt="image thumb" class="img-fluid">
                    </div>
                    <div class="col-6">
                        <h3>{{ product.title }}</h3>
                        <p>$ {{ product.price }}</p>
                        <hr>
                        <p>{{ product.description }}</p>
                    </div>
                </div>
            </div>        
        </div>
    </div>
</template>

<script setup>
    const {id} = useRoute().params
    const url = 'https://fakestoreapi.com/products/' + id
    const { data:product} = await useFetch(url);

    if(!product.value){
        throw createError({statusCode:404,statusMessage:"This page is gone.",message:"...maybe the page you're looking for is not found or never existed."})
    }
</script>

<style scoped>
        
    .productDetail img{
        width: 200px;
        max-width: 100%; 
        margin: 0 auto;       
    }
</style>