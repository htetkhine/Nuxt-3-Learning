<template>
     <div class="container">
      <div class="gif">
        <img src="https://i.postimg.cc/2yrFyxKv/giphy.gif" alt="gif_ing" />
      </div>
      <div class="content">
        <h1 class="main-heading">{{ error.statusMessage }}</h1>
        <p>
          {{ error.message }}                   
        </p>        
        <button @click="handleClearError">Back to home  <i class="far fa-hand-point-right"></i></button>        
      </div>
    </div>
</template>

<script setup>
    defineProps(['error'])
    const handleClearError = ()=>clearError({redirect:'/'})
</script>

<style scoped>
.container {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.gif {
  display: flex;
  justify-content: center;
}

.content {
  text-align: center;
  margin: 3rem 0;
}

.content .main-heading {
  font-size: 2.5rem;
  font-weight: 700;
}
p {
  font-size: 1.3rem;
  padding: 0.7rem 0;
}

button {
  padding: 1rem;
  border-radius: 15px;
  outline: none;
  border: none;
  background: #0046d4;
  color: #fff;
  font-size: 1.3rem;
  cursor: pointer;
}
</style>