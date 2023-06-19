<template>
    <div>
        <h2>This is product details page</h2>
        <h2>{{ route}}</h2>
    </div>
</template>

<script setup>
    const route = useRoute().params.id
</script>

<style lang="scss" scoped>

</style>