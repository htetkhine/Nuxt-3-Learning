<template>
    <div>    
        <header class="menu">
            <div class="container">
                <div class="row">
                    <div class="col-6 py-3">
                        <h3 class="pt-2">Nuxt Project</h3>
                    </div>
                    <div class="col-6 py-3">
                        <nav class="navbar navbar-expand-lg">
                            <div class="container-fluid">
                                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                                    <ul class="navbar-nav me-auto mb-2 mb-lg-0 mx-auto">
                                        <li class="nav-item">
                                            <nuxt-link to="/" class="nav-link active" aria-current="page">Home</nuxt-link>
                                        </li>
                                        <li class="nav-item">
                                            <nuxt-link to="/about" class="nav-link">About</nuxt-link>
                                        </li>
                                        <li class="nav-item">
                                            <nuxt-link to="/products" class="nav-link">Products</nuxt-link>
                                        </li>                             
                                    </ul>
                                </div>
                            </div>
                        </nav>
                    </div>
                </div>
            </div>            
        
        </header>       
        <slot />  
        
        <footer>
            <nav class="navbar navbar-expand-lg menu">
                <div class="container-fluid">
                    <div class="collapse navbar-collapse" id="navbarSupportedContent">
                        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                            <li class="nav-item">
                                <nuxt-link to="/" class="nav-link active" aria-current="page">Home</nuxt-link>
                            </li>
                            <li class="nav-item">
                                <nuxt-link to="/about" class="nav-link">About</nuxt-link>
                            </li>
                            <li class="nav-item">
                                <nuxt-link to="/products" class="nav-link">Products</nuxt-link>
                            </li>                             
                        </ul>
                    </div>
                </div>
            </nav>
        </footer>    
    </div>
</template>

<script setup>
 
</script>

<style scoped>
    .menu{
        background: linear-gradient(to right, #00C58E, #00AA77, #00AC72);
    }
    .router-link-exact-active{
        border-radius: 20%;
        padding: 10px 20px;
        background-color: white;
        color: green;
    }
</style>