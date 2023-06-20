<template>
    <div>
        <h2>Fetch Data</h2>
  
        <div v-for="(product, index) in products">
            <table>
                <tr>
                    <td>{{ product.id }}</td>
                    <td>{{ product.title }}</td>
                </tr>
            </table>
        </div>
    </div>
</template>

<script setup>
const {data:products} = await useFetch('https://fakestoreapi.com/products', {
    method: 'GET'
})
</script>

<style lang="scss" scoped>

</style>