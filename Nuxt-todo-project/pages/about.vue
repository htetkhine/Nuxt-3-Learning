<template>    
    <div class="my-5">       
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h1>About Page</h1>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi voluptatibus rem doloremque et eos numquam reiciendis, in debitis laboriosam aspernatur? Fugiat alias, at nostrum amet nemo quia aliquid minima accusantium?</p>                               
                </div>
            </div>
        </div>      
    </div>
</template>

<script setup> 
    useSeoMeta({
    title: 'My Amazing Site',
    ogTitle: 'My Amazing Site',
    description: 'This is my amazing site, let me tell you all about it.',
    ogDescription: 'This is my amazing site, let me tell you all about it.',
    ogImage: 'https://example.com/image.png',
    twitterCard: 'summary_large_image',
    }) 
   definePageMeta({
        layout:'default'
   })
</script>

<style lang="scss" scoped>

</style>