<template>
    <div>
       
    <Home />
    <h2>{{ state.number }}</h2>
    <button @click="increment">Increment</button>
    <button @click="descrement" v-if="state.number > 1">Descrement</button>
    <button @click="descrement" v-else disabled>Descrement</button>
    </div>
</template>

<script setup>
    useHead({
        title: 'Home page'
    })

    const state = useState(() => ({
        number: 1
    }))

    const increment  = () => {
        state.value.number++
    }

    const descrement = () => {
        state.value.number--
    }

</script>

<style lang="scss" scoped>

</style>