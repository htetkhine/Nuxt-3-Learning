<template>
    <div>
        this is page {{ id }}
    </div>
</template>

<script setup>
    const {id} = useRoute().params
</script>

<style lang="scss" scoped>

</style>