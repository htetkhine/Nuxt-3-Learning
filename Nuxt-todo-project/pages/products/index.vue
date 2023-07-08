<template>
    <div>
<p>product index</p>
<layout :layout="layout">
    <!-- Content of the page -->
  </layout>
    </div>
</template>

<script setup>
   const layout = computed(() => 'products')
</script>

<style lang="scss" scoped>

</style>